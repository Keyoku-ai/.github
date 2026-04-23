# Keyoku — Product Hunt Launch Kit

## Tagline (60 char max)
Make any AI agent autonomous

## Description (500 char max)
Most AI memory tools just store and retrieve. Keyoku goes further: auto-recall, auto-capture, knowledge graph, and a heartbeat system that acts on what matters without being asked.

Three autonomy levels: observe, suggest, or act. Powered by a local Go engine with semantic search, memory decay, and dedup. TypeScript SDK & OpenClaw plugin.

## Topics
- Developer Tools (primary)
- Open Source
- Artificial Intelligence

## First Comment

Hey Product Hunt! I'm Tye, an AI solutions architect. I love building proof of concepts and executing on innovative ideas.

The launch of OpenClaw changed how I think about autonomous AI agents. Today's agents have incredible reasoning and massive context windows for complex tasks. But they're reactive and one-shot. You close the session, everything is gone. Open a new one, start from scratch.

With models like GPT-5.4 and Claude Opus 4.6, long-running tasks are finally possible. But even the best models are missing something fundamental: the cognitive, proactive parts of what makes us human.

Think about what makes us autonomous. We recall. We think. We act. Current AI agents don't do any of that on their own.

OpenClaw gives you a great foundation for building AI agents, but out of the box memory is basic and the heartbeat is static. Keyoku plugs directly into OpenClaw and changes both.

First, it adds a real memory system: auto-recall, auto-capture, knowledge graph, semantic search, memory decay, and deduplication.

But memory alone isn't enough. The real difference is what Keyoku does with it. The heartbeat system continuously scans your agent's memory, detects what needs attention, and takes action based on what it finds. Deadlines approaching, stale context, recurring patterns, sentiment shifts. Your agent doesn't just remember. It thinks and acts on what it knows.

Three autonomy levels let you control how far it goes: observe, suggest, or act.

Everything runs locally on a Go engine. Your data stays on your machine.

One command to add it to any OpenClaw agent:

npx @keyoku/openclaw init

Where we're headed: Keyoku starts with OpenClaw, but the goal is plug-and-play for any AI agent framework. A cloud platform is coming for teams and hosted deployments, and more language support beyond TypeScript is in progress.

Give it a try. Star the repo if you find it useful. I'm looking for feedback on the approach, especially around the heartbeat system and autonomy levels.

## Thumbnail
- 240x240 square
- Use logo-key.svg converted to PNG

## Gallery Images (1270x760, aim for 5-7)
1. Hero — product name + tagline + key visual
2. How it works — architecture flow diagram
3. Knowledge graph — visualization of relationships
4. Heartbeat — what it detects and how it acts
5. Autonomy levels — observe / suggest / act visual
6. Install — terminal screenshot of one-command setup
7. Tech stack — Go engine + TypeScript SDK + OpenClaw plugin

## Video Script (optional, ~90 sec)

[0:00-0:10] Hook
Voice: "What if your AI agent could think and act on what it knows, without being asked?"

[0:10-0:25] Install
Screen: Terminal, run npx @keyoku/openclaw init
Voice: "Keyoku adds intelligent memory to any OpenClaw agent. One command."

[0:25-0:45] Knowledge graph + memory
Screen: Agent connecting info across sessions, referencing relationships
Voice: "Keyoku builds a knowledge graph from your conversations. It tracks relationships between concepts, files, and decisions across every session."

[0:45-1:10] Heartbeat
Screen: Agent proactively surfacing something useful without being prompted
Voice: "The heartbeat system continuously scans your agent's memory and acts on what it finds. Deadlines, patterns, stale context. Your agent doesn't just remember. It acts."

[1:10-1:20] Autonomy
Screen: Config toggling between levels, agent behavior changing
Voice: "You control how far it goes. Observe. Suggest. Or act."

[1:20-1:30] Close
Screen: GitHub repo, install command
Voice: "Keyoku. Memory that acts. Try it now."

## Pre-Launch Checklist
- [ ] PH account active and engaged for weeks before launch
- [ ] Logo uploaded as thumbnail (240x240 PNG)
- [ ] Gallery images created (1270x760)
- [ ] Video recorded and uploaded to YouTube (optional)
- [ ] Tagline, description, first comment finalized
- [ ] Topics selected
- [ ] Supporter list ready (people with established PH accounts)
- [ ] Social media posts drafted (Twitter/X, LinkedIn, Reddit)
- [ ] npx @keyoku/openclaw init tested and working
- [ ] Someone assigned to respond to every PH comment within 5 min

## Launch Day
- Launch at 12:01 AM Pacific Time (Tuesday or Wednesday)
- Post maker comment immediately
- Notify supporters ("I launched, check it out" — never "upvote me")
- Share on social media
- Cross-post: Hacker News, Reddit r/programming, relevant Discords
- Respond to EVERY comment within 5 minutes all day
