🎓 MCP-Enriched Faculty Assistant for Timetable and Room Queries

A Generative AI-Powered Smart Campus Assistant

📌 Project Overview

The MCP-Enriched Faculty Assistant for Timetable and Room Queries is a Generative AI-based application designed to help faculty members access academic timetable and classroom information through natural language conversations.

In traditional educational institutions, faculty members often depend on spreadsheets, documents, or institutional portals to check their daily schedules, lecture timings, classroom allocations, and room availability. Searching through these resources manually can be time-consuming.

To overcome these challenges, this project introduces an intelligent AI-powered chatbot that allows faculty members to ask questions in simple English and receive relevant answers instantly.

The system integrates Large Language Models (LLMs) with the Model Context Protocol (MCP) to connect the AI application with external tools and academic databases. The MCP server provides predefined tools to retrieve faculty timetables, check classroom allocations, and identify available rooms.

🎯 Objectives

Develop an intelligent AI-powered faculty assistant.

Enable faculty members to retrieve timetable information using natural language queries.

Provide classroom allocation and room availability details.

Integrate Generative AI with the Model Context Protocol.

Connect AI applications with structured academic databases.

Reduce manual timetable searching and improve information accessibility.

Provide a simple and interactive chatbot experience.

✨ Key Features

1. AI-Powered Chatbot

Allows faculty members to interact with the system using natural language instead of predefined commands.

2. Faculty Timetable Retrieval

Retrieves daily and weekly faculty schedules, including subjects, lecture timings, and classroom details.

3. Room Availability Checking

Checks whether a particular classroom is available or occupied during a specified time slot.

4. Room Allocation Details

Provides information about allocated classrooms and the faculty members or subjects associated with them.

5. MCP Integration

Uses the Model Context Protocol to connect the AI application with external tools and databases.

6. Intelligent Responses

Uses Generative AI to convert retrieved database information into clear and understandable responses.

🛠️ Technologies Used

Technology

Purpose

Python

Backend development

Generative AI / LLM

Natural language understanding and response generation

MCP

Communication between AI applications and external tools

FastMCP

MCP server development

SQLite / MySQL

Academic information storage

Streamlit

Interactive chatbot interface

FastAPI

Backend API development (if required)

Pandas

Timetable data processing

The technology stack can be adjusted according to the actual implementation.

🏗️ System Architecture

The application consists of the following components:

User Interface: Allows faculty members to enter timetable and room-related queries.

LLM: Understands user questions and generates responses.

MCP Client: Connects the AI application to the MCP server.

MCP Server: Exposes predefined tools for accessing academic information.

Database: Stores faculty details, subjects, timetable records, and classroom allocations.

Response Generator: Converts retrieved information into natural language responses.

Architecture Workflow

       Faculty User
            |
            v
      Chatbot Interface
            |
            v
      Generative AI / LLM
            |
            v
        MCP Client
            |
            v
        MCP Server
            |
      -----------------
      |       |       |
      v       v       v
   Faculty  Timetable Room
    Tool      Tool    Tool
      |       |       |
      -----------------
            |
            v
       Academic Database
            |
            v
      Retrieved Results
            |
            v
       Generative AI
            |
            v
      Natural Language
          Response

⚙️ How the System Works

The working process begins when a faculty member enters a question into the chatbot interface.

The faculty member enters a natural language query, such as "What is my timetable today?"

The LLM processes the query and identifies the user's intention.

The AI application selects the appropriate MCP tool.

The MCP client communicates with the MCP server.

The MCP server executes the requested tool and retrieves information from the academic database.

The retrieved information is returned to the AI application.

The LLM generates a meaningful response and displays it to the faculty member.

Example Queries

Faculty Query:

What is my timetable today?

Where is my next lecture?

Show my weekly timetable.

Which faculty is assigned to Room 205?

Room Availability Query:

Which rooms are available at 10 AM?

Is Room 203 free at 2 PM?

Show all allocated rooms.

Find an available classroom for the next lecture.

🗄️ Database Information

The database maintains structured academic information required by the assistant.

Suggested database tables:

Table

Information Stored

Faculty

Faculty ID, name, department

Subjects

Subject ID, subject name

Rooms

Room number, room capacity

Timetable

Faculty, subject, room, day, start time, end time

The system uses these records to retrieve timetable details and calculate room availability for requested time slots.


🚀 Installation and Setup

Step 1: Clone the Repository

git clone <your-repository-url>

Step 2: Navigate to the Project Directory

cd faculty-assistant

Step 3: Create a Virtual Environment

python -m venv venv

Activate the environment:

Windows:

venv\Scripts\activate

Linux / macOS:

source venv/bin/activate

Step 4: Install Dependencies

pip install -r requirements.txt

Step 5: Configure Environment Variables

Create a .env file and add the required model API credentials and configuration.

LLM_API_KEY=your_api_key
DATABASE_PATH=database/timetable.db

Use the actual environment variable names required by your implementation. Never commit real API keys to GitHub.

Step 6: Initialize the Database

Run the database initialization script provided in your project to create the required tables and insert sample timetable records.

Step 7: Start the Application

For a Streamlit application:

streamlit run app/main.py

For an MCP server, run the server using the appropriate command configured in your application.

Note: The commands above are example setup instructions. Adjust them according to your actual project files and MCP client configuration.

📊 Existing System vs Proposed System

Existing System

Proposed System

Manual timetable searching

AI-powered timetable retrieval

Traditional documents and spreadsheets

Conversational chatbot

Manual room availability checking

Automated database-based checking

No natural language interaction

Natural language queries

Limited external tool integration

MCP-based tool integration

More manual effort

Reduced manual effort

🌟 Advantages

Saves time and reduces manual work.

Provides quick access to faculty schedules.

Simplifies classroom allocation lookup.

Helps identify available and occupied rooms.

Supports natural language communication.

Integrates AI with external academic data sources.

Provides opportunities for future smart campus development.

🔮 Future Enhancements

The project can be extended with additional academic management features, including:

Student timetable assistance.

Attendance information retrieval.

Examination timetable management.

Faculty substitution and leave management.

Automated schedule change notifications.

Voice-based chatbot interaction.

Mobile application integration.

Real-time synchronization with institutional databases.

🔐 Security and Reliability

Protect API credentials using environment variables.

Validate user inputs before database operations.

Implement role-based access for faculty-specific information.

Restrict database operations to approved tools.

Return appropriate messages when requested information is unavailable.

Ensure that room availability is calculated using actual timetable records.

🎯 Conclusion

The MCP-Enriched Faculty Assistant demonstrates how Generative AI and the Model Context Protocol can be combined to simplify academic information retrieval. By connecting an intelligent chatbot with structured timetable and classroom databases, the system allows faculty members to access important information through simple conversational queries.

The project reduces manual effort, improves accessibility, and provides a foundation for developing intelligent academic management solutions in educational institutions.

👨‍💻 Project Information

Project Name: MCP-Enriched Faculty Assistant for Timetable and Room Queries

Domain: Generative AI / Artificial Intelligence

Category: Academic / Smart Campus Application

**Developed By: **

2520030189-A.Akshaya

2520030026-B.Pranavi

2520030140-V.Charishma



Department: Your Department

Institution: Your College Name
