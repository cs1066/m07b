Several uses of LLMs show up repeatedly in practice. What follows are the common categorizations and what is known (or can be reasonably inferred) about how common they are.

**NOTE:** AI produced (August 2026), human (Mike) edited and verified (to the best of my ability).

---

## 1. Generation / Authoring Mode

**What it is:** Produce new text/artifacts from a prompt: drafts, emails, stories, marketing copy, code stubs, UI copy, etc.

**Why it’s important:**

- This is one of the most common LLM use cases: writing assistance, marketing content, coding helpers, etc.

**Evidence of prevalence:**

- Public product messaging from OpenAI, Google, Microsoft, etc. heavily centers on “writing assistance,” “email drafting,” “content generation,” and “coding assistance” use cases.
- Numerous surveys and product case studies report content creation and code generation as top LLM uses (e.g., for GitHub Copilot-like tools and business writing assistants).  
  Even without exact percentages here, it is safe to say this is a *primary* real-world usage pattern.


## 2. Explanation / Tutoring Mode

**What it is:** Explain concepts, walk through reasoning, teach step-by-step, answer “why” and “how” questions in an educational way. It’s transforming *complex or opaque information* into an *understandable form*.

- Example: “Explain this error message as if I’m new to Python”, “Walk me through how backpropagation works.”

**Why it’s important:**

- Many users treat LLMs as on-demand tutors, documentation explainers, or “StackOverflow with explanations.”
- It’s valuable to treat “Explain clearly, not just solve” as a distinct behavioral mode because:
  - The answer format is different (step-by-step, analogies).
  - The success criteria are different (user understanding, not just correctness).

**Evidence of prevalence:**

- Widespread anecdotal reports of students and professionals using LLMs as study aids, concept explainers, and code tutors.
- Learning-focused tools (e.g., chat-based docs, AI “tutors” integrated into courseware) are a major product category; their core capability is explanation rather than decision-making or data synthesis.


## 3. Critique / Review Mode

**What it is:** Evaluate and provide feedback on existing content, decisions, or plans: code reviews, writing critique, UX review, argument analysis.

Examples:
- “Review this PR and list potential bugs and design issues.”
- “Critique this essay for clarity and structure.”
- “Find logical flaws in this argument.”

**Why it’s important:**

- It’s operationally different from generation as you’re not asking for new content but for evaluation against quality criteria.
- It’s hugely useful in workflows: LLMs as reviewers of code, documents, policies, UX copy, etc.

**Evidence of prevalence:**

- Developer-oriented LLM tools include “code review” as a core selling point.
- Editing-focused AI writing tools emphasize “improve,” “revise,” “polish,” and “critique” as key actions distinct from pure drafting.


## 4. Retrieval / Q&A Mode (Knowledge Lookup)

**What it is:** Answer questions by retrieving and summarizing information from a knowledge base (internal docs, web, PDFs, etc.). Key in this usage is the finding and summarizing of relevant information in a larger corpus.”

**Why it’s important:**

- Many “RAG” (retrieval-augmented generation) systems are built around this: agent queries vector DB or search index, then summarizes.
- It has different implementation and prompting patterns (e.g., “If unsure, say so; don’t hallucinate; cite sources”).

**Evidence of prevalence:**

- Major enterprise AI products focus on “answer questions from your documents” as a flagship capability.
- In knowledge-work settings, this is often the first LLM deployment scenario.


## 5. Extraction / Interpretation / Structuring Mode

**What it is:** Turn unstructured or semi-structured inputs (one or many) into structured data: JSON, tables, key-value pairs, entities.

Examples:
  - “From this contract, extract party names, effective date, and termination clause into JSON.”
  - “From these customer emails, extract product, sentiment, and urgency.”

**Why it’s important:**

- It’s a core building block in many enterprise workflows (compliance, operations, CRM, analytics).
- Very different success criterion: strict schema adherence, minimal hallucination, high recall/precision.

**Evidence of prevalence:**

- Numerous LLM-based products for contract analysis, invoice processing, KYC/onboarding, etc. focus on entity extraction and structuring.
- “Structured output” and “JSON-mode” capabilities are heavily marketed features of modern LLM APIs, underscoring common demand.


## 6. Simulation / Role-Play Mode

**What it is:** The model simulates an agent, persona, environment, or multi-agent interaction: customer, interviewer, adversary, user, etc.

Examples:
- “Act as an angry customer; I’ll practice handling complaints.”
- “Simulate an interview panel asking me questions for this role.”
- “Role-play as a skeptical stakeholder challenging this plan.”

**Why it’s important:**

- Unique use cases: training, scenario planning, UX testing, conversation rehearsal.
- Allows exploring social dynamics and edge cases that may not be captured in static data.

**Evidence of prevalence:**

- Common in coaching, sales training, and customer support training products using LLMs.
- Frequently-seen individual prompts where users ask models to “act as X” or “play the role of Y.”


## 7. Decision-making / Planning Support

**What it is:** Provide the LLM with goals, constraints, and context, and it recommends actions, creates plans, suggests priorities, or lists tradeoffs. The LLM's work can be tilted toward "conservative, risk-averse" outcomes or "creative, exploratory" ones.

**Why it's important:**

- Acts as a cognitive sounding board, helping humans systematically weigh trade-offs and evaluate complex, multi-variable scenarios.
- The success criteria are strategic viability, rigor, and goal alignment rather than just linguistic fluency or raw correctness.
- Helps counter human cognitive biases (e.g., anchoring, tunnel vision) by surfacing non-obvious alternatives, edge cases, and hidden assumptions.

**Evidence of prevalence:**

- Widely used across knowledge work (managers, developers, consultants) for roadmapping, project prioritization, risk analysis, and strategic brainstorming.
- Enterprise AI assistants (e.g., Microsoft 365 Copilot, Notion AI) prominently feature decision-support capabilities such as project planning, agenda synthesis, and scenario analysis in their core toolsets.


## 8. Tool-Orchestration / Agentic Mode

**What it is:** Use the LLM as a controller that plans and executes sequences of tool calls: APIs, databases, search, code execution, etc.

Contrasts with (7):
- AIs in decision support: “Given context, recommend what a human should do.”
- Agentic mode: “Given a high-level user goal, autonomously pick tools and call them to *do the work*,” while the human just sees the result.

Examples:
- “Given a GitHub repo and this bug description, run tests, inspect logs, propose a fix, and open a PR.”
- “Given my todo list in Notion, prioritize tasks and reschedule events on my calendar.”

**Why it’s important:**

This is where LLMs shift from “advisor” to “operator.” The success criteria become:
  - Correct tool usage
  - Error handling
  - Multi-step planning

**Evidence of prevalence:**

- A growing category of “AI agents” products and frameworks (e.g., task-oriented agents, workflow automation tools) use LLMs primarily in this orchestration role.
- Many API features now focus on tools/function-calling capabilities specifically for this mode.
