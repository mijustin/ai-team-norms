# How we use AI

_A forkable set of norms for software development teams using AI tools. Fork it, adapt it, make it yours._

---

## Our philosophy

### We build what the strategy demands

LLMs make it easy for anyone on the team to prompt a feature into existence. Left unchecked, it will result in [feature creep](https://en.wikipedia.org/wiki/Feature_creep), where the product becomes increasingly complex, bloated, and cluttered.

> "[In the age of AI] we have to ruthlessly say no to things that seem legitimately neat but aren't core." – [Michael Feldstein](https://x.com/msfeldstein/status/2031448481311895624)

Here's how we decide "what gets built" on our team. 

Overall direction is set by:
- `Name`: company strategy
- `Name`: product strategy
- `Name`: engineering and architecture

It's their job to maintain a clear product roadmap, focused on our most critical milestones.

Don't make decisions about "what to build" on your own. Reach out to `Name` if you have suggestions or need guidance.

### Not all ideas are worth building 

[is this section needed - something like " Every addition has to
  be maintained, documented, tested, and supported. Before an idea becomes a
  ticket, someone should be able to clearly articulate the user problem it
  solves — not just that it's neat, or that it was easy to prototype."]

### All code has a human owner

> "All code must have a human owner who will take responsibility for it. It’s their code, just as if they’d written it in an integrated development environment; they just happened to use a different tool. If all generated code must ultimately be owned and reviewed by a human, that person is able to tune the results for safety, efficiency, and quality." – [Ben Werdmuller](https://werd.io/good-vibes-bad-vendors/)

Every Pull Request has a human owner and a human reviewer.

### Review and test relentlessly

Peer review is not optional. Automated testing must gate all production deployments.

### Spend more time cleaning things up

> "LLMs keep pulling us to ship the next feature but there's 100x more value in fixing what we have improving our process of how we build things." – [Dax Raad](https://x.com/thdxr/status/2031377117007454421)

### Slow down

The increased velocity AI creates can inflate workloads and lead to burnout. Set limits. Take breaks. Slow down. Think deeply.

---

## Our AI workflow

### Tools

Our team primarily uses `Claude Code`.

For spec-drive development we use [OpenSpec](https://openspec.dev/) / [Get Shit Done](https://github.com/gsd-build/get-shit-done) / 


### Process

1. Plan (spec-driven development)
   → Ask AI for design options
   → Ask AI to propose architecture or tasks

2. Implement the plan
   → Have AI start to implement the plan in iterations (build this, then I'll review)
   → Make commits throughout to save progress
   → Document 

3. Test
   → Generate tests using `this tool`

4. Generate PR
   → Run lint/tests/security checks

5. PR review
   → Human review required even for AI code

---

## Credits and inspiration

- **Dax Raad** ([@thdxr](https://x.com/thdxr)), of OpenCode, [whose post](https://x.com/thdxr/status/2031377117007454421) inspired the creation of this document.
- **Ben Werdmuller** for his article [Good Vibes, Bad Vendors](https://werd.io/good-vibes-bad-vendors/), which articulated the skills shift, the importance of engineers being central to the process, and the risks of burnout, security, and quality degradation.
- **Michael Timbs**'s article [Code Quality in the Age of Coding Agents](https://michaeltimbs.me/blog/code-quality-in-the-age-of-coding-agents/) is a good reference.
- **Addy Osmani** (Google Chrome team engineering lead) wrote up his team's specific workflow: [LLM coding workflow going into 2026](https://addyosmani.com/blog/ai-coding-workflow/)