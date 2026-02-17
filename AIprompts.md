File that holds all AI prompts. Ask Mode questions not added because the agent is in read-only mode.
-----------------------------------------------------------------------------------------------------

Model: GPT 5.2
Mode: Chat
I am creating a user website to be deployed on Github Pages. Help me write my file skeletons please.

-----------------------------------------------------------------------------------------------------

Model: GPT 5.2
Mode: Chat
I would like it so that the header line wraps up around the "Home" when at the home page, around the "About" when on that page, and so on so that the user has some extra understanding about where they are on my website.

-----------------------------------------------------------------------------------------------------

Model: Auto (agent)
Mode: Agent
Prompt: /create-rule State what AI model is being used before generating response.
/create-rule Append model, mode, and prompt to @AIprompts.md with seperators between prompts.

-----------------------------------------------------------------------------------------------------

Model: Auto (agent)
Mode: Debug
Prompt: Debug  @.cursor/rules/append-prompts-to-aiprompts.mdc so that the mode for all prompts (including this Debug one) is shown instead of using the logging agents (Agent) mode.

-----------------------------------------------------------------------------------------------------

Model: Auto (agent)
Mode: Plan
1. Create testing branch (webtest) so that not every push goes to prod.
1.1 Find out way to open website with localhost to visualize fast UI changes.

-----------------------------------------------------------------------------------------------------

Model: Auto (agent)
Mode: Agent
Prompt: /create-skill reference all .mdc rules for every prompt from all agents

-----------------------------------------------------------------------------------------------------

Model: Auto (agent)
Mode: Agent
Prompt: \section{Experience} ... Update @about.html with the above experiences

-----------------------------------------------------------------------------------------------------

Model: Auto (agent)
Mode: Agent
Prompt: \section{Projects} ... Add above project info to @projects.html

-----------------------------------------------------------------------------------------------------

