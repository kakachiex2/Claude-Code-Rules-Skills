1. Reset your chats every 15–20 messages
   Claude re‑reads the entire conversation on every turn, so older, longer chats become “token black holes.” The more history you carry, the more expensive each new message is, and the faster you slam into limits.
   Treat chats as task‑specific rooms, not a lifetime WhatsApp thread.
   Ask Claude:
   "Summarise everything important we’ve done here into a ‘project card’ under 300–400 tokens: goal, key decisions, current status, and next three actions.”
   Paste that project card into a fresh chat with:
   “New chat, same project. Here’s the context from the last thread: [card]. Continue from here.”
   You’ve just compressed thousands of tokens of history into a few hundred you can cheaply reuse.
2. Ask for plans first, then execution
   Going straight to “Write the full article/app/strategy” invites long answers and multiple rewrites, which compounds token usage. You save a lot by separating thinking from doing.
   Start with a cheap planning pass:
   “Before you write anything, give me a concise plan: a numbered list of steps to complete this task. Keep it under 150 tokens.”
   Once you like the plan, scope the work:
   “Now implement only steps 1 and 2 in detail. Stop after that and wait for my review.”
   If the direction is wrong, you catch it early without paying for the whole journey. If it is right, you move through the plan in controlled, affordable chunks.
3. Summarise and compress your own context
   Every time you paste the same life story, business description, or project background into a new chat, you are burning tokens on duplicate context. Instead, treat that information as a reusable asset.
   Take your long brief and ask Claude:
   “Compress everything I’ve told you about me and this project into a reusable ‘context card’ under 400 tokens. Keep only what you need to do great work; remove fluff and repetition. Use headings.”
   Save that card somewhere you can copy quickly. For new chats, paste the card instead of free‑typing paragraphs. When something important changes, update the card:
   “Update the context card with this new information: [change]. Show me the revised version under 400 tokens.”
   You keep Claude informed while keeping your per‑message cost under control.
4. Turn off tools when you don’t need them
   Web browsing, code execution, search plugins, and other tools are powerful, but each invocation adds extra context and extra responses. Leaving tools on “just in case” makes every message heavier than it has to be.
   For pure writing, idea generation, or simple Q&A, explicitly tell Claude to stay offline:
   “For this session, don’t use any external tools unless I explicitly say ‘use tools’. Answer from your own reasoning and the text I give you.”
   When you do need web or code, temporarily allow them:
   “For this next question you may use tools: [question]. After answering, go back to not using tools by default.”
   You get the benefit of tools only when they are actually worth the extra tokens.
5. Keep files smaller and questions more targeted
   Uploading a 400‑page PDF and asking a broad question forces Claude to consider far more text than necessary. Large files are not the problem; large files plus vague instructions are.
   Split big documents into logical chunks (chapters, sections, appendices) and upload only the relevant piece. If you must use a large file, use a “locator” pass first:
   “You have this entire document. First, tell me which 2–3 sections are most relevant if my only goal is [goal]. Don’t answer the goal yet—just name the sections/pages.”
   Then follow up:
   “Now, using only those sections, answer: [question]. Ignore the rest of the document.”
   You explicitly tell Claude what to ignore, which saves both reading and reasoning tokens.
6. Ask for surgical edits
   The expensive pattern is: generate a long answer, dislike one part, and ask “rewrite the whole thing in a new style.” That doubles or triples tokens for content that was already 90% acceptable.
   Instead, target the work:
   To polish everything but keep meaning:
   “Edit this for clarity and flow. Keep every idea and the overall structure; change wording only.”
   To fix one bad section:
   “Edit just the section under the heading ‘[Heading]’ to be shorter and more direct. Don’t touch anything else.”
   To change tone in two stages:
   “First, clean up grammar and structure without changing tone.”
   “Now adjust tone to be more conversational without losing precision.”
   You pay only for the part that actually changes.
7. Push trivial tasks to cheaper tools and save Claude for the hard stuff
   Claude is often your “expensive brain.” It makes sense to reserve it for tasks where its extra context window and reasoning genuinely matter.
   Offload small, low‑stakes work: simple grammar fixes, tiny paraphrases, basic code snippets, or canned replies can go to lighter models, browser add‑ons, or even built‑in email tools. Keep Claude for:
   Long documents and complex rewrites
   Strategy, architecture, and planning
   Multi‑step reasoning and deep research
   Work that will actually ship to clients or an audience
   You reduce how often you touch Claude without feeling like you are using it less.
8. Split complex workflows into “cheap” and “expensive” phases
   Trying to do research, analysis, and polished writing in a single mega‑prompt forces Claude to browse, synthesise, and generate at maximum cost all at once.
   A better pattern is two phases:
   Phase 1 – Research & notes (tools allowed):
   “Use tools to gather and summarise the 10 most important points about [topic]. Output them as short bullet ‘RESEARCH NOTES’ under 500 tokens, with links.”
   Phase 2 – Writing & reasoning (no tools):
   “Now, without using any tools, and based only on the RESEARCH NOTES above, write [outline/article/email/plan]. Don’t pull in new information.”
   Phase 1 is limited and structured; Phase 2 is offline and cheap. You still get rich answers, but only pay for browsing once.
9. Treat the limit as 80% of what you actually have
   Hitting the hard wall mid‑project is the worst possible timing. It is better to treat Claude’s advertised limit as the “red line” and aim to stay under it.
   As you see warnings or feel you are using Claude heavily:
   Stop starting new big threads.
   Use the remaining messages to capture state and plan the restart.
   Ask Claude:
   “Assume we have 3–5 messages left before my usage cap.
   Summarise what we’ve done so far in this project.
   List the exact next prompts I should run when my usage resets so we can continue smoothly.
   Keep this under 250 tokens.”
   Paste that plan into your notes. When the limit resets, you resume with zero confusion and no need to replay history.
10. Make Claude budget‑aware from the start
    Claude can only optimise for cost if you tell it that cost matters. You can set that expectation explicitly at the beginning of a heavy session.
    Use a “budget contract” like this:
    “For this whole session, assume we have a limited token budget.
    Default to short, high‑information answers unless I say ‘go deep’.
    If you think my request will generate a very long answer or require reading large files, warn me first and suggest a cheaper alternative (for example, outline instead of full draft).
    Ask me to confirm before calling any tools or summarising big documents.
    If there’s a way to solve my problem in fewer turns, tell me.”
    Then, when you are okay with spending more, override it explicitly:
    “This one matters—go deep here even if it’s expensive.”
    You turn Claude into a collaborator that watches your budget instead of a firehose that uses maximum capacity every time.
