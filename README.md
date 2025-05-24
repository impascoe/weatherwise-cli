# 🌦️ WeatherWise Template

Welcome to the **WeatherWise Assignment Starter Template**! This repository helps you kickstart your project by
combining Python, weather APIs, data visualisation, and AI-assisted development. 🤖📊

![Build With AI](https://img.shields.io/badge/Built_with-AI-blueviolet?logo=openai)
![Python](https://img.shields.io/badge/Made_with-Python-3776AB?logo=python)
![Visualisation](https://img.shields.io/badge/Includes-Visualisations-orange?logo=plotly)

---

### Running the Notebook

To run the `starter_notebook.ipynb`:
1. **Ensure Ollama is running (for AI features)**: If you plan to use the AI-assisted features within the notebook, make
   sure your local Ollama instance is running.
2. **Ensure you have a Python environment** with Jupyter Notebook or JupyterLab installed.
3. **Install project dependencies**:
   ```bash
   pip install -r requirements.txt
   ```
4. **Set up your OpenWeatherMap API Key**: You will need to obtain a free API key
   from [OpenWeatherMap](https://openweathermap.org/appid) and add it to the notebook where prompted, or set it as an
   environment variable.

5. **Launch Jupyter**:
   ```bash
   jupyter notebook starter_notebook.ipynb
   ```
   Or, if you prefer JupyterLab:
   ```bash
   jupyter lab starter_notebook.ipynb
   ```
6. Follow the instructions and execute the cells within the notebook.

#### Running on Google Colab

1. **Upload the notebook to Google Colab**:
    * Open Google Colab: [https://colab.research.google.com/](https://colab.research.google.com/)
    * Click on `File > Upload notebook...` and select the `starter_notebook.ipynb` file.
2. **Install Dependencies**
3. **Set up your OpenWeatherMap API Key**:
    * You will need to add your OpenWeatherMap API key directly in the notebook. You can do this by creating a new code
      cell and setting the environment variable:
      ```python
      # Uncomment and replace with your actual API key if you don't want to use .env file
      # os.environ['OPENWEATHER_API_KEY'] = 'your_api_key_here'
      ```
4. **Execute Cells**: Run the notebook cells sequentially.

---

## 📁 Folder Structure

- `starter_notebook.ipynb` — Main notebook to build your project.
- `ASSIGNMENT.md` — Full assignment specification.
- `ai-conversations/` — Save your `.txt` AI conversations here.
- `submission/` — Files to help you finalise your submission:
    - `reflection.md` — Write your 300–500 word project reflection

---

