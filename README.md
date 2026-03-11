# How we use AI

_A forkable set of norms for software development teams using AI tools. Fork it, adapt it, make it yours._

---

## Raise the bar, don't lower it

It's now trivially easy to prompt a feature into existence. That ease is a trap. The bar for what ships should remain high — or get higher. Before building anything, ask: does this need to exist? Talk to your team. Talk to your users. Don't make that decision alone.

## Product thinking before prototyping

A working prototype is not worth more than time spent understanding why you'd build something in the first place. The center of gravity has shifted from writing code to crafting goals, understanding users, and being crystal clear about the experience and value you want to create. Start there.

## Leave the code better than you found it

When iterating on a feature, it's tempting to let the AI absorb the hackiness in the original design rather than fix it. Resist this. Refactor. The willingness to clean up the underlying design — not just paper over it — is what separates a codebase that compounds in value from one that becomes a liability.

## Fix before you add

AI tools keep pulling teams toward the next feature. There is often far more value in fixing what you have and improving how you build things. Slow down. Repair. Improve the process. New features built on a shaky foundation just create more work downstream.

## All code has a human owner

Generated code is not ownerless. Every line merged into your codebase must be owned by an engineer who is responsible for its correctness, security, and maintainability. Using AI is just a different tool. The accountability doesn't change — it's their code, as if they'd written it themselves.

## Engineers at the center, from the start

AI is a tool under human control, not a replacement for engineering judgment. For non-engineers, AI can be a useful prototyping tool — but those prototypes are not enduring software, and they can't be handed off to engineers to support. To properly architect a system, an engineer must be involved from the beginning. Performance, scalability, security, and the ongoing overhead of maintenance require expertise that cannot be prompted into existence.

## Review and test relentlessly

Peer review is not optional. Automated testing must gate all production deployments. These practices don't become less important because AI is writing code — they become more important. When comprehensive tests are in place, AI tools can even use test output to self-correct. That feedback loop is a feature, not a workaround.

## Protect the team

The increased velocity AI creates can quietly inflate workloads and lead to burnout. A study in Harvard Business Review found that adding AI actually intensified work, putting engineers at risk. The employers most enthusiastic about AI are sometimes the least enthusiastic about employee wellbeing. Set limits. Enforce breaks. Don't let the productivity illusion erode your team.

## Cultivate delayed gratification

Everything great comes from being able to delay gratification for as long as possible. AI erodes this — it makes it easy to ship now, to get the dopamine hit of a working demo, to move on before the work is truly done. Cultivate the discipline to slow down, think deeply, and build things worth building. We may be collectively losing this ability. Fight for it.

## Code volume is not the measure

LLMs create the illusion of productivity because a lot of code gets written. But code is not the product — reliability, maintainability, and genuine user value are. The engineers who care deeply about quality, who ask the harder questions, who give a damn about what they ship: those are the ones who matter most.

---

## Credits and inspiration

- **Dax Raad** ([@thdxr](https://twitter.com/thdxr)), creator of OpenCode, whose post on the three challenges LLMs introduce to software teams — shipping unworthy features, tolerating hackiness, and neglecting cleanup — inspired the foundation of this document.
- **Ben Werdmuller** for his article [Good Vibes, Bad Vendors](https://werd.io/good-vibes-bad-vendors/), which articulated the skills shift, the importance of engineers being central to the process, and the risks of burnout, security, and quality degradation.
- **Gergely Orosz** ([@GergelyOrosz](https://twitter.com/GergelyOrosz)) for distilling Dax's ideas into the memorable framing: "don't ship features just because you can."
- **Manthan Gupta** for the observation that LLMs create the illusion of productivity, and that the engineers who give a damn about quality are the ones who won't be replaced.
