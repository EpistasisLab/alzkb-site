# Design
## Backend Framework
- Flask
## Database scheme
### Database Engine
- PostgreSQL
### Tables
- users
- messages (chat_history)
- chats
- etc.
## APIs
### Tech
- Flask-RESTful extention
### Endpoints
- `/users`
- `/chats`
- `/messages`
- `/models`
### Web Socket Events
#### Tech
- Flask-SocketIO
#### Events
- `connect`: Establish connection and authenticate user.
- `disconnect`: Close connection and clean up resources.
- `join_room`: Join a chat session with a specific LLM.
- `leave_room`: Leave a chat session.
- `send_message`: Send message from the user to the LLM.
- `receive_message`: Receive message from LLM to the user.
### API Wrapper
Use locally deployed models.
Explore the possiblity of using API Wrappers, such as:
- OpenAI
- Hugging Face

## LLM Deployement
- Register for API keys and configure API settings
- Define model parameters, such as: temperature, top-p, frequency penalty, etc.
- Define a chat context, such as personality, tone, style, etc.