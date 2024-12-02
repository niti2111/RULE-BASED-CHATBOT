# RULE-BASED-CHATBOT

This is a simple **rule-based chatbot** where you define specific outputs based on user inputs. The chatbot responds to queries based on pre-defined patterns and keywords.

---

## Features

- **Greeting Interaction**: The chatbot asks for the user's name and offers assistance.
- **Pattern Matching**: Matches user inputs with specific keywords using regular expressions.
- **Predefined Intents**:
  - **Customer Requirements**: Responds to requests related to customer needs.
  - **Answer Requirements**: Provides solutions or updates on queries.
  - **Product Details**: Offers product-specific information.
- **Exit Commands**: Recognizes commands like "quit," "bye," or "thanks" to end the conversation.
- **Random Starter Questions**: Initiates conversations with randomized questions for a natural flow.

---

## Key Functionalities

- **Negative Responses Handling**: 
  - Recognizes responses like "no," "nah," or "not interested" and gracefully ends assistance.
- **Exit Command Detection**:
  - Detects phrases like "quit" or "exit" to terminate the chatbot session.
- **Customizable Responses**:
  - Tailored responses for each intent category (e.g., product details, requirements).

---

## Code Overview

- **Class: `Chatbot`**
  - Defines the core logic and functionality of the chatbot.
  - Implements regular expression-based intent matching (`self.allienable`).
- **Key Methods**:
  - `greet()`: Initiates the conversation.
  - `chat()`: Engages with the user in an interactive session.
  - `match_reply(reply)`: Matches user input with defined patterns.
  - Response methods for specific intents:
    - `customer_requirement()`
    - `answer_requirement()`
    - `product_details()`
  - `make_exit(reply)`: Detects exit commands.
  - `no_match_intent()`: Handles unrecognized inputs.

---

## How to Use

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/rule-based-chatbot.git
