# aiEmailAndMeetingAssistant
This is an open source Copilot Studio Autonomous AI Email Meeting Assistant

In this repo, you will find three different Instruction sets for an autonomous agent that can answer emails and schedule metings on your behalf: Basic, Intermediate, Advanced.

-The Basic instruction set is for an mvp (minimum viable product) agent that can respond to emails on your behalf once you've put them into a vetted folder.

-The Intermediate instruction set can also create calendar meetings upon reuqest.

-The Advanced instruction set also searches for meeting conflicts, proposes other meeting times, and can handle multi-turn conversations. 

This Agent is created in Copilot Studio with GPT 5 (Chat) as the Model.

The agent uses the following Tools:
-Office 365 Outlook > Get emails (V3)
-Office 365 Outlook > Mark as read or unread (V3)
-Office 365 Outlook > Move email (V2)
-Office 365 Outlook > Reply to email (V3)
-Meeting Management MCP Server (Note: this is for Office 365 Outlook)

The autonomous agent is triggered by:
-Office 365 Outlook > When a new email arrives (v3)

Calendar id: Calendar

Known Limitations in Advanced instructions: 
-The agent does not have any instructions on handling Meeting Update or Delete requests. Because of the :Meeting Management MCP Server", it may partially handle this request but may fail on subsequent steps.
-Handling for above limitation can be added by further ehnancing the Advanced instructions. No additional tool should be required.

