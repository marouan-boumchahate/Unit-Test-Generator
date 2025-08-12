# 🧪 Unit Tests Generator

An AI-powered tool that automatically generates comprehensive unit tests for your code using OpenAI's GPT-4. Simply paste your code and get a detailed test case table with various input scenarios, including edge cases designed to test your code's robustness.

## ✨ Features

- 🤖 **AI-Powered Analysis**: Uses GPT-4 to understand your code and generate relevant test cases
- 📊 **Structured Output**: Returns test cases in a clean markdown table format
- 🎯 **Edge Case Detection**: Focuses on generating inputs that could potentially break your code
- 🌐 **Web Interface**: Easy-to-use Gradio interface with beautiful styling
- 🔄 **Real-time Streaming**: See test cases generated in real-time
- 💻 **Multi-language Support**: Works with code written in any programming language

## 🚀 Quick Start

### Prerequisites

- Python 3.7+
- OpenAI API key

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/unit-tests-generator.git
   cd unit-tests-generator
   ```

2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Set up environment variables**
   
   Create a `.env` file in the project root:
   ```env
   OPENAI_API_KEY=your_openai_api_key_here
   ```

4. **Run the application**
   ```bash
   jupyter notebook Unit_Tests_Generator.ipynb
   ```
   
   Or run all cells and the Gradio interface will launch automatically.

## 🎯 How It Works

1. **Code Analysis**: The AI reads and understands your code line by line
2. **Test Generation**: Creates comprehensive test cases including:
   - ✅ Normal/valid inputs
   - ❌ Edge cases and boundary conditions  
   - 🔥 Invalid inputs that might cause failures
   - 🚫 Error conditions and exception scenarios

3. **Structured Results**: Outputs a markdown table with:
   - **ID**: Test case identifier
   - **Input Values**: Specific inputs for the test
   - **Test Purpose**: What the test is checking
   - **Result**: Expected outcome (Pass/Fail)

## 💡 Example Output

| ID  | Input Values                                                                                  | Test Purpose                                      | Result  |
|-----|-----------------------------------------------------------------------------------------------|---------------------------------------------------|---------|
|  1  | emp_id=101, name='John Doe', email='john@company.com', department='Engineering', salary=75000 | ✅ Validate normal registration and display       | Pass    |
|  2  | emp_id=104, name='Alice', email='alice@company.com', department='Finance', salary=80000       | ✅ Validate registration of new employee          | Pass    |
|  3  | emp_id=-1, name='', email='invalid-email', department='', salary=-1000                        | ❌ Test handling of invalid inputs                | Fail    |

## 🎨 Interface Features

- **Modern UI**: Gradient buttons with hover effects
- **Glassmorphism Design**: Translucent cards with backdrop blur
- **Responsive Layout**: Works on different screen sizes
- **Real-time Updates**: Streaming responses for immediate feedback

## 🔧 Configuration

### System Prompt Customization

You can modify the `system_message` variable to customize how the AI generates test cases:

```python
system_message = "You are an assistant that writes and executes all possible unit tests..."
```

### Model Selection

Currently uses GPT-4. You can change the model by modifying:

```python
OPENAI_MODEL = "gpt-4o"  # or "gpt-3.5-turbo", etc.
```

## 🙏 Acknowledgments

- OpenAI for providing the powerful GPT-4 API
- Gradio team for the excellent web interface framework
- The open-source community for inspiration and support

## 📞 Support

If you encounter any issues or have questions:

1. Check the [Issues](https://github.com/yourusername/unit-tests-generator/issues) page
2. Create a new issue with detailed information
3. Join our discussions in the [Discussions](https://github.com/yourusername/unit-tests-generator/discussions) tab

---

⭐ If you find this project helpful, please give it a star!
