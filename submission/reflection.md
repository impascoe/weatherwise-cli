✍️ Project Reflection

# AI Tools Utilized

There were two AI tools that were used in this project:

GitHub Copilot: This tool was instrumental for real-time code suggestions, auto-completing boilerplate code (for example, in widget setup), and scaffolding new functions like the initial versions of get_weather_data and create_temperature_visualisation. It sped up the  process of making the app by reducing manual typing and offering quick and easy solutions to common programming boilerplate and common use cases between many codebases. GitHub Copilot also assisted in diagnosing error handling blocks (try-except).

ChatGPT was used for broader brainstorming, such as providing different approaches for the UI structure and for debugging more complex issues that Copilot alone couldn't figure out itself. It was particularly helpful in refining prompts for the hands-on-ai integration and exploring advanced Matplotlib styling options.

# Prompting Techniques

- Several intentional prompting strategies were applied throughout the project, as documented in PROMPTING.md and the ai-conversations/ logs:

- Concept Exploration Prompts: Used to understand best practices, such as secure API key management with .env files and python-dotenv, and to compare different API query structures.

- Implementation Prompts: Leveraged to obtain concrete code for specific features, including the ipywidgets-based UI, data fetching from the OpenWeatherMap API, and JSON parsing logic.

- Challenge Prompts: Applied when initial AI suggestions were not what was wanted, and then later pushing the AI for alternatives or detailed explanations.

- Before/After Comparisons: Documenting these (as seen in ai-conversations/) helped in reflecting on and refining prompting strategies for future interactions.

# What Worked Well?

I am particularly proud of the user interface created by the create_weather_app function. It successfully integrates two distinct modes of operation: a widget-based forecast generator and an AI-powered query mode. It was satisfying to see ipywidgets come together to create an interactive experience, allowing users to select locations, forecast days, and graph types (temperature, precipitation). The AI mode, which uses the hands-on-ai package to parse natural language and then dynamically generate and display Matplotlib visualizations within the widget output area, felt like a big success in creating a responsive and intelligent application. The easy, smooth transitions between these modes and the clear output of graphs within the UI worked out very well.

# What Would You Do Differently?

If I had more time, I would try to improve on the natural language understanding sections of the parse_weather_question function and its integration with the hands-on-ai model. Currently, it handles basic locations, a few predefined time periods ("today", "tomorrow", "this week"), and primary attributes ("temperature", "rain"). I would have liked to expand its ability to understand more subtle queries, such as "What will the wind speed be in Sydney the day after tomorrow?". This would involve more prompt engineering for the LLM and potentially more complex logic in generate_weather_response to handle a wider array of parsed intents, entities, and units. Additionally, implementing more robust error handling for ambiguous user queries or unsupported weather attributes would be a priority.

# Final Thoughts

This project was an important and great experience, effectively showing me how to integrate various Python libraries (requests, Matplotlib, ipywidgets, python-dotenv) and AI tools (Copilot, ChatGPT, hands-on-ai) to build a functional and interactive app. The process of intentionally prompting AI, evaluating its suggestions, and  refining the code showed the collaborative nature of modern software development. Managing API keys securely, fetching and processing external data, creating user-friendly visualizations of data, and building an interactive UI provided an interesting view of a small-scale development lifecycle. It was slightly challenging but worth it to see all the components come together and working.