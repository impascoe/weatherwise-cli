# AI Interaction Documentation

This document details how AI tools were used intentionally and strategically throughout the WeatherWise project. It includes prompting strategies, before/after examples, and a summary of the six-step methodology, referencing actual AI conversations and code improvements.

---

## 1. Overview of AI Tools Used

- **GitHub Copilot**: Used for code suggestions, function scaffolding, and error correction.
- **ChatGPT**: Utilised for brainstorming, debugging, and refining prompts.
- **hands-on-ai**: Integrated for natural language parsing and AI-driven responses within the application.

---

## 2. Intentional Prompting Techniques Demonstrated

- **🎯 Concept Exploration Prompts**: Explored best practices, e.g., how to securely store API keys in a Python notebook using environment variables and `python-dotenv`.
- **🛠️ Implementation Prompts**: Asked for concrete code solutions, such as how to prompt a user for a location with a default fallback, and how to convert JSON responses to Python dicts.
- **🔍 Debugging Prompts**: Troubleshot issues, e.g., why an API key was not being found in the environment, how to ensure `.env` files are loaded correctly, and how to handle overlapping x-axis labels in matplotlib.
- **🖼️ Visual Refinement Prompts**: Iteratively improved graph appearance by asking for solutions to label crowding and requesting advanced styling to match a visual target (e.g., ASCII art representation).
- **Challenge Prompts**: Questioned initial AI solutions, such as why the `days` parameter did not work as expected in the wttr.in API, and explored alternatives.
- **Before/After Comparisons**: Documented code improvements resulting from targeted prompts (see `resources/before-after-example.md`).

---

## 3. Example AI Conversations

### Example 1: Secure API Key Storage
- **Prompt**: "What is the correct way to store an API key securely for a Python notebook?"
- **AI Response**: Recommended using environment variables and the `python-dotenv` package, with code examples and best practices.
- **Follow-up**: Debugged why the key was not found, leading to the use of `load_dotenv()` at the top of the notebook.

### Example 2: User Input with Default Value
- **Prompt**: "How do I get a location from a user if they choose not to put any in?"
- **AI Response**: Provided code using `input()` and `pyinputplus` to prompt for a location and use a default if blank.

### Example 3: Multiple Query Parameters in API Calls
- **Prompt**: "How would you have multiple query params?"
- **AI Response**: Explained URL query parameter syntax and provided an example for wttr.in with `?days=5&format=j1`.

### Example 4: Converting JSON Responses
- **Prompt**: "How do I convert the resulting JSON response into a Python dict?"
- **AI Response**: Provided examples using `json.loads()` and `response.json()` from the `requests` library.

### Example 5: Debugging API Key Not Found
- **Prompt**: "This says that it cannot find the key."
- **AI Response**: Diagnosed the issue as the `.env` file not being loaded, and recommended using `python-dotenv` and `load_dotenv()`.

### Example 6: Handling API Parameter Limitations
- **Prompt**: "It seems like setting the number of days does not do anything."
- **AI Response**: Researched and explained the limitations of the `days` parameter in the wttr.in API, clarifying the difference between CLI and web usage.

### Example 7: Visualisation with Matplotlib - Basic Bar Graph
- **Prompt**: "How do I make a bar graph of the min max temperatures using matplotlib?"
- **AI Response**: Provided a code example for a grouped bar chart using `matplotlib` and `numpy`.

### Example 8: Matplotlib X-axis Label Disambiguation and Formatting
- **Prompt**: "In matplotlib, is it possible to have repeating x labels that dont get grouped together? For example the weather in the notebook overlays points that have the same hourly time but are on separate days. What can be done?"
- **AI Response**: Advised using unique labels by combining date and time (e.g., "YYYY-MM-DD HH:MM") and provided a code example.
- **Follow-up Prompt**: "however this gets all of the labels squished together, how can i make it look nicer?"
- **AI Response**: Suggested label rotation, `AutoDateLocator`, and `DateFormatter` for improved readability, with a code example.

### Example 9: Advanced Graph Styling in Matplotlib
- **Prompt**: "How can I use matplotlib to create a better styled graph like: [ASCII art example provided by user]?"
- **AI Response**: Outlined techniques like subplots, `gridspec`, custom tick formatting, annotations for icons/wind, background shading, and provided a comprehensive Python code example using `matplotlib.dates` and `numpy` to achieve a similar style. Suggested `plotext` for terminal-based plots.

---

## 4. Prompting Foundations Demonstrated

- **INPUT**: Handling user input robustly, including validation and default values.
- **STORE**: Securely storing and retrieving sensitive data (API keys) using environment variables and `.env` files.
- **OUTPUT & VISUALIZATION**: Formatting data for display, creating clear and informative graphs (e.g., temperature trends, precipitation bars), and refining visual elements for readability and aesthetic appeal.
- **DEBUG**: Diagnosing and resolving issues with environment configuration, API usage, and visual output (e.g., label overlaps, crowded text).

---

## 5. Before/After Examples

See `resources/before-after-example.md` for detailed before/after code comparisons and prompting strategies, including:
- Initial basic function for weather retrieval
- Prompting for improvements (error handling, validation, documentation)
- Final robust function with all requested features

---

## 6. Six-Step Methodology Example

A full prompting journey using the six-step methodology is documented in `resources/sample-prompting-journey.md`, including:
- Restating the problem
- Identifying input/output
- Manual solution sketch
- Pseudocode generation
- Implementation and refinement
- Testing and edge case handling

---

## 7. AI Conversation Log Files

- All significant AI conversations are saved in the `ai-conversations/` folder.
- Each file documents the prompt, AI response, and resulting code changes or decisions.

---

## 8. Additional Prompting Examples

- See `resources/prompt-by-method-step.md` for a guide to effective prompts for each programming foundation.
- The notebook's "AI Prompting Log" section includes further prompt/response summaries.

---

## 9. Summary

Intentional prompting and iterative collaboration with AI tools were central to the development of WeatherWise. The documentation and conversation logs demonstrate a thoughtful, strategic approach to leveraging AI for software engineering tasks. This approach resulted in more robust, user-friendly, and maintainable code, as well as a deeper understanding of both programming and AI-assisted development.
