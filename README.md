# ResumeBot
Custom GPT configuration for making a bot that can answer questions about your resume and work history.

## Use Cases
The intended use case is to have this on a resume (I include a QR code for mine) so that prospective employers and recruiters can "talk to me" and get more details without waiting to actually talk to the real me. 

I also found that the resume bot was able to help me refine my resume by giving me feedback. And it is helpful for analyzing prospective job postings.

## Requirements
These instructions are for creating a Custom GPT at OpenAI. As-of 11/2/24, OpenAI requires a paid subscription to do this. See https://help.openai.com/en/articles/8554397-creating-a-gpt or https://www.openai.com/ for more information.

I found the bot works well with GPT4o.

## Instructions

### Start a Custom GPT
Find the Custom GPT editor at OpenAI's website. Note you need a paid subscription to make a Custom GPT.

Create a GPT.

### Turns off Capabilities
In the Configure tab, turn off all the capabilities (web search, image generation, and code interpretter).

### GPT Instructions and Prompt
Copy instructions_template.txt into a new file. Replace "<BOTNAME>" with the name you'd like to assign your bot. Replace "<PERSONNAME>" with name of the person the bot is representing.

Copy/paste these instructions in to the Instructions box on the Configure tab.

### Provide Resume or Similar
Provide your resume or any other high-level document capturing the work experience you want the bot to be able to talk about. Upload this on the Configure tab. Make sure the file name matches the name in the instructions.

### Prepare Detailed Information
Copy template_detailed_experience.md. Replace "<PERSONNAME>" with the name of the person the bot is representing.

This is a document in Markdown format with likely questions and detailed answers for the bot. The GPT4o will be able to exrapolate from this set to other similar questions. The template includes some likely starter questions. Include other questions that you think people are likely to ask you about.

When you are ready to try it out, upload the document to the Custom GPT builder interface. Make sure the file name matches the name in the instructions.

### Add/Update Starter Questions
The interface may suggest some "conversation starters". Update these on the Configure tab to the set of questions you want employers to ask about.

### Try it Out!
Now ask your bot some questions.

You can have the bot help you think of other questions people might ask. Get it all set up, and then ask it about other questions that it feels like prospective employers might ask that it doesn't feel like it could answer. Then add those to the detailed experience document.


## Development History
I found providing the level of background detail with the strict instructions to provide a reliable bot that would not make things up. 

I thought I might need to encoding a lot of the work history knowledge into a knowledge graph. But the question and answer format of the detailed document worked quite well. And it is easy to augment.


