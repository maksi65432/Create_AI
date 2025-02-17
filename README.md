# Create_AI: Custom AI Configuration Toolkit  
*A toolkit to generate and configure AI project files rapidly. Simplify setup and focus on building AI models.*  

---

### **📌 Table of Contents**  
- [Features](#-features)  
- [Installation](#-installation)  
- [Configuration](#-configuration)  
- [Usage](#-usage)
- [Contributing](#-contributing)  
- [License](#-license)  

---

### **✨ Features**  
- **Rapid Setup**: Generate AI file in minutes with proper settings.
- **Customizable Configs**: Modify settings via a simple built-in json file. 
- **Multi-Platform Support**: Compatible with GitHub, GitLab, and local directories.  
- **High-end technologies**: You can make your LLM in minutes in LLM style with deep NLP proccesing and GRPO reasoning.  
- **Easy to use**: Based on Lake-1 architecture model creation with GRPO reasoning with powew of deep NLP proccesing.  
- **Fast and unbelievable**: With power of tiktoken tokenizer and advanced Lake architecture with a lot of other advanteges you can make your Ai that can beat any AI what you want if you can.

---

### **🚀 Installation**  
1. **Clone the repository**:  
   ```bash
   git clone https://github.com/maksi65432/Create_AI.git
   cd Create_AI
   ```  
2. **Install dependencies**: 
   1. **Installing main components**
        ```bash
        pip install tiktoken 
        ```
   2. **Installing torch**
         Please check the site:
         ```url
         https://pytorch.org/
         ```

---

### **⚙️ Configuration**  
Modify `Built-in json file` to tailor your AI project:  
```json
{
    "vocab_size": 32000, # number of unique tokens (words, subwords, or characters) a model can recognize and process.
    "emb_dim": 1024, # Size of the vector representation for each token or input feature
    "hidden_dim": 2048, # Neurons per layer
    "n_layers": 8, # hidden layers of minding adjust by hardware
    "n_experts": 2, # Adjust only as integer that is multiplied without a remainder on 8 or 12 from n_layers, if you wanna make model more fast on some inference
    "dtype": "float16", # Tensor type (for cpu only or and ROCm use available: float16, float32, float64.)
    "seq_len": 512, # How much tokens in the batch can be handled
    "batch_size": 4, # Adjust on your hardware and needs
    "checkpoint_interval": 1, # How much file creation will be paused to save the state if somethign fail like not enoug resources and then will be paused until enoug resources
    "tokenizer_file": "tokenizer.json" # Do not modify if using global tools
}

```  

---

### **📋 Usage**  
Generate a project using the CLI:  
```bash
python Create_AI.py
```

---

### **🤝 Contributing**  
1. Fork the repository.  
2. Create a feature branch:  
   ```bash
   git checkout -b feature/new-template
   ```  
3. Submit a pull request.  

---

### **📜 License**  
MIT License. See [LICENSE](https://github.com/maksi65432/Create_AI/blob/main/LICENSE).  

---
