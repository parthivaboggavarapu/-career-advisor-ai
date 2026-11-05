# Career Advisor AI Agent

An AI-powered career guidance assistant built with **n8n**. It helps students and fresh graduates explore career paths, research job-market trends, understand skill requirements, and create personalized learning roadmaps.

## Features

- **Personalized career guidance** based on education, interests, skills, experience, and location
- **Current job-market research** using web search
- **Salary research and career comparisons**
- **Skill-gap identification** for target roles
- **Personalized learning roadmaps** with learning phases and project ideas
- **Conversational guidance** for students and fresh graduates

## Tech Stack

- **n8n** — AI agent and workflow automation
- **Claude Sonnet 5** — AI model (configured in the n8n Agent Builder)
- **Web Search** — Retrieves current job trends, salary information, and skill requirements
- **n8n Agent Builder** — Agent instructions and chat interface

> The exact search provider and available integrations depend on the tools configured in the n8n agent.

## How It Works

1. The user shares their education, skills, interests, career goals, and preferred location.
2. The AI agent identifies relevant career paths.
3. When current information is needed, the agent uses web search to research job trends, salaries, and skill requirements.
4. The agent compares options and explains its recommendations.
5. It provides a practical learning roadmap, including skills, projects, and resources.

## Example Prompt

> I'm a first-year CSE student in India interested in AI and web development. Compare current job trends and entry-level salary information for AI Engineer and Full Stack Developer roles. Recommend a suitable career path and create a personalized six-month learning roadmap based on my current skills.

## Setup

1. Create or open an n8n AI Agent.
2. Configure an AI model (this project currently uses Claude Sonnet 5).
3. Add and configure a web-search tool.
4. Paste the system prompt from [`system-prompt.md`](./system-prompt.md) into the agent's Instructions/System Message field.
5. Test the agent with questions about career paths, job trends, salaries, skills, and learning roadmaps.

## Repository Structure

```text
career-advisor-ai/
├── README.md
└── system-prompt.md
```

You can add workflow exports and demo screenshots after reviewing them for sensitive information.

## Example Test Questions

1. I'm a first-year CSE student interested in AI and web development. Which career paths should I explore?
2. What skills are currently required for entry-level machine learning engineer roles in India?
3. Compare AI Engineer and Full Stack Developer careers, including typical skills and salary ranges.
4. I know basic Python. Create a six-month roadmap to prepare for AI engineering internships.
5. What projects should I build to strengthen my frontend developer portfolio?

## Important Notes

- Job trends and salary figures vary by country, city, company, experience, and source.
- The agent should cite or link sources when available and indicate when salary figures are estimates.
- AI-generated career guidance is informational and should not be treated as a guarantee of employment or salary.
- **Never publish API keys, passwords, private credentials, or sensitive personal information.** Review exported workflow JSON before uploading it to a public repository.

## Author

**Parthiva Aneesh**

## License

Add a license if you want others to reuse or modify this project. For example, you may choose the MIT License.
