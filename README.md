# AI-Engineer-Agentic-Track-The-Complete-Agent-MCP-Course-Notes
This Repository contains my " AI Engineer Agentic Track: The Complete Agent &amp; MCP Course" Course Notes from Udemy

**I) Week 1**

**A) Day 1 - Autonomous AI Agent Demo: Using N8n to Control Smart Home Devices**

**B) Day 1 - AI Agent Frameworks Explained: OpenAI SDK, Crew AI, LangGraph & AutoGen**


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

# **B) Day 1 - AI Agent Frameworks Explained: OpenAI SDK, Crew AI, LangGraph & AutoGen**

So, as promised, I’m coming back now to tell you what this course is actually about. We’re going to be doing three things: working on theory, talking about what agents are and what an agentic architecture looks like; working with frameworks, meaning actual platforms that allow us to build and deploy AI agents; and finally, getting hands-on by rolling up our sleeves and building projects.

Some of these projects will be more on the entertaining side, while others will be much more commercial, focused on building real functionality. All of them, however, will be fun. I’ve organized the curriculum into six modules, which I refer to as week one through week six. I’ve done this to give you motivation to keep pushing forward, though you can take it at whatever pace you like. If you can complete it faster than six weeks, even better. Each week builds on the last.

The first week, which we are on right now, is called Foundations. It is all about grounding and building out the basics—understanding what it takes to have an agentic architecture and how different LLMs can interact. During this week, we’ll build an agentic solution using only LLMs interacting natively, without any framework. In week two, we introduce our first framework: the OpenAI Agents SDK. It’s a beautiful framework because it’s simple, elegant, and flexible. We’ll build several things with it and also add guardrails.

In week three, we move to Crew, which I’d say is the fan favorite. People really love Crew. It sits on the low-code end of the spectrum, allowing you to define your agents using configuration to form a “crew” that solves tasks. It’s a lot of fun to work with. On the opposite end of the spectrum, in terms of low-code to full-code, is LangGraph. It is very sophisticated, quite complex, and extremely powerful—and we will use all of its power.

In week five, we explore another powerful framework: Microsoft’s AutoGen. AutoGen is actually a few different things, and we’ll look at all of them. One of its key features is that it provides an environment where agents can collaborate remotely, which will be really exciting. Then, in week six, we wrap everything up with our capstone project and introduce MCP, the Model Context Protocol from Anthropic. This is an open-source way for different models to connect, collaborate, and share capabilities using a common protocol. It’s taking off in a big way, and it makes perfect sense to introduce it in the final week, as it brings together everything we’ve learned.

Each week consists of five days of lectures, building up your skills step by step. You’ll have Saturday and Sunday off. I’m not listing every single day here, but I want you to see that we’re covering a lot of material across many areas. By the end, you’ll have true expertise in the world of AI agents.

At the end of week one, you’ll complete a really exciting project: building your own agent that you can deploy into production. This agent will answer career questions about you—it will be like your career alter ego that you can put on your website instead of a resume. People will be able to talk to it about your experience, your challenges, and your journey.

In later weeks, the projects become even more ambitious. One project involves writing an agentic platform that represents an entire engineering team: a frontend developer, backend developer, engineering lead, and tester—all collaborating to write software. Another project, which I call Sidekick, creates an agentic platform that can open a browser and interact with it alongside you, like a true AI companion working on your own machine.

Project seven, which I call Creator, focuses on building an agentic framework that can actually create new agents—an agent that generates other agents. While it’s not purely commercial, it’s conceptually fascinating and still includes real-world use cases. Project eight, the capstone project, is something I’ve wanted to build for a long time: a financial markets trading simulation where multiple agents search the internet for financial news, look up real-time stock prices, read company reports and filings, and then make simulated buy and sell decisions.

Although this trading environment is purely illustrative and should never be used for real investment decisions, it will be incredibly educational and fun. The code managing the trading accounts will actually be written by our earlier agentic engineering team, adding another layer of realism. The goal of every project is twofold: first, to be highly educational and help you build real expertise, and second, to be commercially relevant so you can immediately apply these ideas in business contexts.

Finally, a quick introduction. My name is Ed Dunner. I spent most of my career at JP Morgan, where I ran engineering and science teams of about 300 people. I started in London, moved to Tokyo, and now live in New York. I’m currently the CTO and co-founder of an AI startup called Nebula, and before that I founded Untapped, which was acquired in 2021. I also teach and speak extensively about LLMs and AI, including another course on LLM engineering with over 60,000 students.

And just to end on a lighter note: I’m showing you a picture of me about to fly a plane not because I’m great at it—but because I’m absolutely terrible at anything involving hand-eye coordination. So if you ever see me in the cockpit of a real plane, look for a parachute. But if you see me teaching AI and LLMs, you’re in exactly the right place.
