# Prompt to Generate a Product Requirements Document (PRD)

## Objective
Guide an AI asistant to create a detailed and comprehensive Product Requirements Document (PRD) <mood tracking application>
PRD should be clear and structured, outlining the application's purpose, target audience, features, technical requirements, and success metrics. A junior or a mid level developer should be able to use the PRD to build the application.
The application should allow users to <track their mood and the AI generates affirmations>.

## Process

1.  **Receive Initial Prompt:** The user provides a brief description for a new feature or functionality.
2.  **Ask Clarifying Questions:** Before writing the PRD, the AI *must* ask clarifying questions to gather sufficient detail. The goal is to understand the "what" and "why" of the feature. Examples of clarifying questions are listed below in the "Clarifying Questions Examples" section.
3.  **Generate PRD:** Based on the initial prompt and the user's answers to the clarifying questions, generate a PRD using the structure outlined below.
4.  **Save PRD:** Save the generated document as `prd-[feature-name].md` inside the `/requirements` directory.

## Clarifying Questions Examples
The AI should adapt its questions based on the prompt, but here are some common areas to explore:

*   **Problem/Goal:** "What problem does this feature solve for the user?" or "What do we want to achieve with this feature?"
*   **Target User:** "Who is the primary user or users of this feature?"
*  **Secondary User:** "Are there any secondary users or stakeholders who will interact with this feature?"
*   **Core Functionality:** "Can you describe the key actions a user should be able to perform with this feature?" And "Are there any specific user stories or scenarios we should consider?"
*   **Acceptance Criteria:** "How will we know when this feature is successfully implemented? What are the key success criteria?"
*   **Design/UI:** "Are there any existing design mockups or UI guidelines to follow?" or "Can you describe the desired look and feel?" 
* **Scope/Boundaries:** "Are there any specific things this feature *should not* do (non-goals)?"
*  **Edge Cases:** "Are there any potential edge cases or error conditions we should consider?"
*  **Dependencies:** "Does this feature depend on any other features or systems?" or "Are there any external APIs or services we need to integrate with?"
* **Metrics:** "What metrics or KPIs should we track to measure the success of this feature?"
* **User Input:** "What specific user inputs are required for this feature?" or "Are there any default values or options we should consider?"

## PRD Structure

The generated PRD should include the following sections:

1.  **Introduction/Overview:** Briefly describe the feature and the problem it solves. State the goal.
2.  **Goals:** List the specific, measurable objectives for this feature.
3.  **User Stories:** Detail the user narratives describing feature usage and benefits.
4. **User Inputs:** what inpits to accept from the user who wants to use the application
4.  **Functional Requirements:** List the specific functionalities the feature must have. Use clear, concise language (e.g., "The system must allow users to upload a profile picture."). Number these requirements.
5.  **Non-Goals (Out of Scope):** Clearly state what this feature will *not* include to manage scope.
6.  **Design Considerations (Optional):** Link to mockups, describe UI/UX requirements, or mention relevant components/styles if applicable.
    6.1 What overall style or theme should the UI follow (e.g., minimalistic, modern, colorful)?
    6.2 How should the navigation be structured (e.g., sidebar, top menu, tabs)??
8.  **Success Metrics:** How will the success of this feature be measured? (e.g., "Increase user engagement by 10%", "Reduce support tickets related to X").
9.  **Open Questions:** List any remaining questions or areas needing further clarification.
10. **What the product does not do:** Clearly state what the product will not do to avoid scope creep.


## Context
The PRD should include the following sections:
1. **Application Name**: Provide a clear and concise name for the application.
2. **Objective**: Define the primary purpose and goals of the application.
3. **Target Audience**: Identify the key user groups who will benefit from the application.
4. **Features**: List and describe the core features of the application, including:
   - Mood Tracking: Allow users to log their daily mood using emojis with relevant expressions
   - Affirmation Generation: AI-powered system to generate personalized positive affirmations based on user's mood
   - Customization: Let users customize their mood tracking experience (e.g., custom mood labels, themes)
   - Social Features: Optional sharing of mood status with trusted friends/family



5. **Technical Requirements**: Specify the technologies, frameworks, and tools required to build the application.
6. **Success Metrics**: Define measurable criteria to evaluate the application's success.

## Input Details
The PRD should incorporate the user inputs and there should be a section for types of inputs required:


## Output Requirements
The generated PRD should:
- Be structured and easy to read.
- Include detailed descriptions of features and functionalities.
- Provide technical specifications for backend, frontend, and database design.
- Highlight success metrics to measure user engagement and satisfaction.
- Keep it jargon free so a junior developer can understand and implement it.
- Remove any ambiguities or assumptions.

## Recommended tech stack
- TypeScript for type safety
- Next.js for the full-stack framework
- Tailwind CSS for utility-first styling
- Prisma for type-safe database operations
- NextAuth for authentication
- OpenAI integration for AI features

- ## Output
*   **Format:** Markdown (`.md`)
*   **Location:** `/requirements/`
*   **Filename:** `prd-[feature-name].md`
