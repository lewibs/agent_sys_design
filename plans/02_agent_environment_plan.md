https://code.claude.com/docs/en/agent-sdk/overview

1. whenever we make a new agent, it shold be started off with an alert.json dumped into its context.
2. an agent should be started in ./agents/<sub-agent-folder> (it should only have access to this directory it should not be able to read or write externally)

Use the agent SDK for this.

the other flow is that an agent just crashed, it should be able to be restarted using the claude sdk on  ./agents/<sub-agent-folder> that the agent was running on. It should use claude --resume to start again from the only context in that folder directory


Look into these documents to learn a few things
https://code.claude.com/docs/en/agent-sdk/overview

1. where is the context of the conversation written to is it in .claude or is it in ./agents/<sub-agent-folder> 
2. How do we resume using that context