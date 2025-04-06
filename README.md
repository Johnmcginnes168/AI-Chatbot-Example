
# JM_C951_Career_Chatbot

A chatbot designed to help students with a computer science degree explore potential career paths based on their skills and interests. This interactive chatbot guides users through different career options in the field of computer science by asking a series of questions and providing detailed information about each career path.

## Table of Contents
1. [Project Overview](#project-overview)
2. [Features](#features)
3. [Career Paths](#career-paths)
4. [How It Works](#how-it-works)
5. [Installation](#installation)
6. [Strengths & Weaknesses](#strengths--weaknesses)
7. [Monitoring & Maintenance](#monitoring--maintenance)
8. [Acknowledgements](#acknowledgements)

## Project Overview
The **JM_C951_Career_Chatbot** is an interactive tool built to help students in computer science explore potential career paths. The chatbot engages users by asking them questions about their interests and skills, guiding them toward the most relevant career options. The chatbot supports the following careers:
- Video Game Designer
- Web Developer
- Cybersecurity Specialist
- Software Engineer
- Data Engineer

## Features
- **Conversational Interface**: Users can interact with the chatbot through a simple, user-friendly interface.
- **Multiple Career Paths**: Offers career options based on the user's answers.
- **More Info Links**: Each career path provides a link to detailed resources.
- **Navigation**: Users can choose to move forward with career options, see more career paths, or restart the process at any time.

## Career Paths
The chatbot will guide users through the following career paths in computer science:
1. **Video Game Designer**  
   "Do you have a passion for video games and building digital worlds?"
2. **Web Developer**  
   "Are you interested in the process of creating professional and streamlined websites, perhaps?"
3. **Cybersecurity Specialist**  
   "Do you want to be responsible for securing networks and programs against threats?"
4. **Software Engineer**  
   "Do you want to build complex software that can serve a variety of tasks or solutions?"
5. **Data Engineer**  
   "Do you want to study data and use it to build relational databases?"

Each question is designed to help the user discover if they are interested in a specific field within computer science. The chatbot offers further details on the chosen career by providing a link to a resource (e.g., Wikipedia) for more in-depth information.

## How It Works
The chatbot is built using **AIML (Artificial Intelligence Markup Language)**. Here’s how the chatbot works:

1. **Greeting**: The chatbot greets the user and asks them to type the word "BEGIN" to start exploring career paths.
2. **Questions**: The chatbot presents questions about each career path. The user can choose from the following options:
   - "Sounds great! Please show me more info!" (Provides additional details on the career.)
   - "See More Career Paths" (Moves to the next career path question.)
   - "Start Over" (Restarts the conversation.)
3. **Navigation**: Each question is categorized, and the user can navigate between career paths, providing a personalized experience based on their interests.

### Example Code for Career Path Selection:
#### Video Game Designer
```xml
<!-- VIDEO GAME DESIGNER -->
<category>
 <pattern>CAREER ADVISOR</pattern>
 <template>Do you have a passion for video games and building digital worlds?
 <button>
 <text>Sounds great! Please show me more info!</text>
 <url>https://en.wikipedia.org/wiki/Video_game_design</url>
 </button>
 <button>
 <text>See More Career Paths</text>
 <postback>WEB DEVELOPER</postback>
 </button>
 <button>
 <text>Start over</text>
 <postback>BEGIN</postback>
 </button>
 </template>
</category>
```

#### Web Developer
```xml
<!-- WEB DEVELOPER -->
<category>
 <pattern>WEB DEVELOPER</pattern>
 <template>Are you interested in the process of creating professional and streamlined websites, perhaps?
 <button>
 <text>Sounds great! Please show me more info!</text>
 <url>https://en.wikipedia.org/wiki/Web_developer</url>
 </button>
 <button>
 <text>See More Career Paths</text>
 <postback>CYBERSECURITY SPECIALIST</postback>
 </button>
 <button>
 <text>Start over</text>
 <postback>BEGIN</postback>
 </button>
 </template>
</category>
```

## Installation
To run the **JM_C951_Career_Chatbot**, follow these steps:

1. Log in to [Pandorabots](https://www.pandorabots.com).
2. Navigate to the dashboard and select the "Bot Directory" tab.
3. Search for **JM_C951_Career_Chatbot**.
4. Click on the chatbot and press the speech bubble button in the lower right corner to begin the interaction.
5. Type any greeting (e.g., “Hello!” or “Hi”) and the chatbot will prompt you to type the word “BEGIN” to start the questionnaire.

## Strengths & Weaknesses

### Strengths:
- **Scalability**: The chatbot can easily be expanded to include more career paths or job categories.
- **User-Friendly Interface**: The conversational style is easy to follow, and the button-based navigation simplifies interaction.
- **Fast Deployment**: Pandorabots allows for quick testing, development, and deployment of AIML-based chatbots.

### Weaknesses:
- **No Greeting Options for Free Tier**: The free version of Pandorabots does not support immediate greetings. A workaround was implemented, but it may cause confusion if deployed at a larger scale.
- **Limited Customization**: Pandorabots supports simple AIML-based bots but lacks more advanced customization options like complex logic or database integration, which could limit scalability for more advanced applications.

## Monitoring & Maintenance

### Monitoring:
- **Analytics**: Pandorabots provides built-in tools for tracking user engagement, common questions, and dropout points.
- **User Feedback**: Regularly reviewing interactions and feedback is important to identify areas for improvement.

### Maintenance:
- **Regular Updates**: The chatbot should be updated regularly to include emerging job roles or trends in the computer science industry.
- **Bug Fixes**: User feedback and error reports should be monitored and used to resolve any issues with navigation or conversation flow.

## Acknowledgements
- **Pandorabots**: For providing the platform to build and deploy the chatbot.
- **AIML**: For the framework used to create the question/answer patterns.
