# 🌦️ WeatherWise Template

Welcome to the **WeatherWise Assignment Starter Template**! This repository helps you kickstart your project by combining Python, weather APIs, data visualisation, and AI-assisted development. 🤖📊

![Build With AI](https://img.shields.io/badge/Built_with-AI-blueviolet?logo=openai)
![Python](https://img.shields.io/badge/Made_with-Python-3776AB?logo=python)
![Visualisation](https://img.shields.io/badge/Includes-Visualisations-orange?logo=plotly)

---

### Running the Notebook

To run the `starter_notebook.ipynb`:

1.  **Ensure you have a Python environment** with Jupyter Notebook or JupyterLab installed.
2.  **Install project dependencies**:
    ```bash
    pip install -r requirements.txt
    ```
3.  **Set up your OpenWeatherMap API Key**: You will need to obtain a free API key from [OpenWeatherMap](https://openweathermap.org/appid) and add it to the notebook where prompted, or set it as an environment variable.
4.  **Ensure Ollama is running (for AI features)**: If you plan to use the AI-assisted features within the notebook, make sure your local Ollama instance is running.
5.  **Launch Jupyter**:
    ```bash
    jupyter notebook starter_notebook.ipynb
    ```
    Or, if you prefer JupyterLab:
    ```bash
    jupyter lab starter_notebook.ipynb
    ```
6.  Follow the instructions and execute the cells within the notebook.

#### Running on Google Colab

1.  **Upload the notebook to Google Colab**:
    *   Open Google Colab: [https://colab.research.google.com/](https://colab.research.google.com/)
    *   Click on `File > Upload notebook...` and select the `starter_notebook.ipynb` file.
2.  **Install Dependencies**
3.  **Set up your OpenWeatherMap API Key**:
    *   You will need to add your OpenWeatherMap API key directly in the notebook. You can do this by creating a new code cell and setting the environment variable:
        ```python
        # Uncomment and replace with your actual API key if you don't want to use .env file
        # os.environ['OPENWEATHER_API_KEY'] = 'your_api_key_here'
        ```
5.  **Execute Cells**: Run the notebook cells sequentially.

---

## 📁 Folder Structure

- `starter_notebook.ipynb` — Main notebook to build your project.
- `ASSIGNMENT.md` — Full assignment specification.
- `ai-conversations/` — Save your `.txt` AI conversations here.
- `resources/` — Guides, prompting tips, and AI technique examples.
- `submission/` — Files to help you finalise your submission:
  - `checklist-md.md` — Submission checklist
  - `reflection.md` — Write your 300–500 word project reflection
  - `one-page-summary.md` — (Optional) Your own summary of key ideas or process

---


## 📓 Submission Checklist

✅ Complete all required functions  
✅ Include at least 5 AI conversations in `ai-conversations/`  
✅ Document your intentional prompting  
✅ Fill in your project reflection in `submission/reflection-template.md`  
✅ Zip your project and upload it to the LMS  

---

🧠 AI Conversations  
Save your AI interactions in the `ai-conversations/` folder.  
See `ai-conversations/how-to-log-ai-conversations.md` for details.

---

## 🧠 Need Help with AI Prompts?

Check out:
- `resources/ai-tips-tricks.md` — Prompting tips and pitfalls
- `resources/sample-prompting-journey.md` — Full example of AI-enhanced development
- `resources/prompts-by-method-step.md` — Prompts aligned with the 6-step dev process
- `resources/before-after-example.md` — Required: Show how your prompting improved AI-generated code

Good luck and have fun! 💡🌤️
