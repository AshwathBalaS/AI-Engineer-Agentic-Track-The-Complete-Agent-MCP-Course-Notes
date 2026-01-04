# AI-Engineer-Agentic-Track-The-Complete-Agent-MCP-Course-Notes
This Repository contains my " AI Engineer Agentic Track: The Complete Agent &amp; MCP Course" Course Notes from Udemy

**I) Week 1**

**A) Day 1 - Autonomous AI Agent Demo: Using N8n to Control Smart Home Devices**




# **I) Week 1**

# **A) Day 1 - Autonomous AI Agent Demo: Using N8n to Control Smart Home Devices**

Well, hello. My name’s Ed Donner. I’m a two-time AI startup co-founder and a former Managing Director at J.P. Morgan. I’m about to take you on a wild ride.

We’re going to be spending the next six weeks together on an adventure. I’ve actually just finished doing the full six weeks’ worth of projects myself. There are eight projects along the way, and I can tell you that I have some astonishing things in store for you. I genuinely can’t wait to get started. Let’s do this.

Now, it’s customary with these things to kick off with an introduction to myself and to talk about the goals of the course. But people who’ve taken my courses before will know that I don’t like doing that. So let’s not do that. Let’s get straight to action.

Let’s go and see some autonomous AI agents in practice, and we’ll come back and do the other stuff later.

I’ve taken us now to the app n8n, which is an exciting application that’s definitely generating a lot of interest. This is an example of a low-code or no-code workflow app that allows you to construct workflows by orchestrating between different applications, all without necessarily needing to write code yourself.

What makes n8n different from some other workflow tools is that it has generative AI built into it, which is why people are so excited about it. If you come to n8n, you can use the cloud version, which is what we’re doing here, or you can download it and run it locally.

You can press “Get Started” and set up an account if you want to follow along yourself, or you can just watch me. But it might be fun to try this out if you haven’t used it before. I’ve already set up an account, and once I’ve signed in, I get this initial screen prompting me to add my first step.

You can also use one of their templates right away, but we’re going to build something ourselves. So we add a first step. What we’re going to do is start with a chat message.

If I go back to the canvas by pressing “Back to Canvas” in the top left, you can see the canvas layout. We now have a chat box represented visually here, where a user can send a message and something happens as a result of that message.

Next, we press the plus button and move over to the right-hand side, where we select Advanced AI. From there, we create an AI agent. When I go back to the canvas, you can see that we now have a chat message flowing into an AI agent, represented by a box, and something can come out the back of that agent.

You don’t need to know all the details at this stage—this is just to give you an idea. By all means, you can play with this yourself. Most of this course will be about building things like this, but for now, let’s give it a shot.

The next step is to add a chat model. This is the large language model that sits behind the AI agent. I’m going to pick an OpenAI chat model because I already have an OpenAI API key, which we’ll help you set up later if you don’t have one.

Alternatively, you could use Ollama and run everything locally for free, but that would require installing it on your machine. For now, I’ve set up my OpenAI account. To do this yourself, you simply create a new credential and paste in your API key. I’ve already done that, so my OpenAI account is connected.

You can see here that the OpenAI chat model is now connected to my AI agent. So far, so good.

Next, we’re going to add a tool. Tools are one of the most fundamental building blocks of agentic AI, and this week will focus heavily on building and using tools.

I press the plus button again to open up the list of tools that can be connected to the agent. You can see a wide range of tools—things like calculators, Google Calendar integration for booking meetings, email access, Facebook timeline access, even reading Hacker News.

But I’m going to scroll down and pick something I want to show off: the Philips Hue tool. Philips Hue controls smart light bulbs, and I happen to have several of them in my apartment.

I select one of my light strips called the bed strip. I add a field for brightness and let the AI decide what value to use. I also add a field for hue, which represents the color, and again let the AI handle it. That’s all there is to it.

When I go back to the canvas, you can now see visually that the AI agent has access to a tool that can control my Philips Hue light bulb. We now have a full setup: a chat input, an AI agent, a language model, and a tool.

Let’s bring up the chat interface and test it. I type, “Hi there.” You can see the agent thinking, and it replies, “Hello, how may I assist you today?”

Next, I say, “Please turn the lights on. Bright white.” And—bam! The lights turn on. I’m actually wearing the light strip, so you can see it working in real time.

Now, you might say, “Okay, that’s cool. I see tools in action. I see an LLM controlling your lights. But I’m not seeing autonomy yet. I don’t see it making its own decisions.”

So let me show you that.

To make the agent autonomous, we give it agency. I say, “Please pick a color—either deep red or deep blue—and change the lights to that color.” Let’s see what it does.

And there we go. It picks red and changes the lights accordingly. Fantastic.

So there you have it. We’ve built an autonomous agent. It’s a simple task, but you just saw it make its own decision—choosing red over blue—and execute that decision by controlling a physical device, all through n8n’s web app.

That was a small and somewhat superficial example, but it was our first real foray into the world of agentic AI. I strongly encourage you to explore n8n yourself. It’s easy to set up an account, connect web forms, hook into Google Calendar, and try many other integrations. It gives you a great hands-on sense of what it’s like to work with agents.

However, I should point out that this is the last time we’ll be using a low-code or no-code tool like this. For the next six weeks, we’re going to roll up our sleeves and write code. We’ll be building agents ourselves, working with frameworks that allow multiple agents to interact, be orchestrated, and solve real problems.
