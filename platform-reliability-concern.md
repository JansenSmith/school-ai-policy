Bad news (but a plan!). I've done extensive research and testing, and while I was able to get Gemini to write files and retrieve them in isolated sessions, the failure rate is approximately 70%. The literature is clear: Gemini hallucinates file operations habitually and routinely. This is repeatedly documented and clearly architectural — not a configuration issue.

As an AI/ML Engineer and Educator, I need to flag a systemic concern with three interlocking components:

1. Execution hallucination. Gemini's backend silently fails file read/write operations while the model generates language confirming success. Students have no way to distinguish a successful save from a hallucinated one. Research on automation bias (Microsoft Research, 2022) documents the consequence: users stop verifying outcomes and defer to the system's stated confidence — the clinical definition of learned helplessness (Seligman & Maier, 1967), extended to HCI contexts. Research on user reliance (arXiv:2604.04319, 2025) finds that AI errors do not significantly reduce user reliance — users normalize inconsistency rather than correcting for it. The corrective loop that prevents this outcome requires users to be able to save and act on corrections. Gemini's architecture removes that loop entirely.

2. Information siloing. Gemini siloes all student work in discrete, non-persistent chat sessions by default. The one available escape mechanism — Drive file creation — is the capability that hallucinates. Pangrazio (2025, British Journal of Educational Technology) documents exactly this pattern in platform-mediated education: vendor-controlled data infrastructures create institutional dependency on platform providers — and, as I observed in testing, both read and write operations hallucinate, making student-owned continuity structurally impossible. The OECD Digital Education Outlook (2023) identifies data portability as the policy antidote; Gemini's architecture forecloses it.

3. Pedagogical unsoundness. UNESCO's AI Competency Framework for Students (2024) establishes that genuine AI literacy requires students to protect their human agency throughout the design, provision and use of AI — and to integrate new knowledge into their own schemas rather than outsourcing that synthesis to the system. A platform that hallucinates persistence and forecloses portability does neither. Selwyn (2022) argues that AI platforms offering to "free" users from cognitive labour undermine the iterative, self-directed engagement through which genuine competence and autonomy are actually built. A platform that traps student context, hallucinates persistence, and offers no portability cannot serve as the vehicle for teaching AI literacy — it actively models the opposite.

This is a technical finding grounded in current HCI and ML pedagogy literature. The gap between Gemini's stated capabilities and observed reliability crosses the threshold for what I can responsibly require students to depend on.

I see this as two separate issues:
- What do I do Friday, Monday, Tuesday?
- What do we do about this platform issue going forward?

Re F/M/T, options as I see them:
- Teach a basic HueForge filament painting project. I already maintain extensive process documentation in my personal knowledge system; the attached draft curriculum is derived directly from that.
- Teach an existing Inkscape project
- Teach an existing catapult project

Re the platform: I propose we discuss this next week. Would you like me to discuss the matter with [Name A] or [Name B]? Beyond this curriculum, I've been thinking about what it would take to support [program] students with executive functioning — that work requires exactly the kind of persistent, student-owned context that Gemini's architecture forecloses. The platform constraints we've been working within make that difficult to pursue responsibly.

---

Attachments: `lessons-HF.pdf`, `platform-reliability-concern-citations.pdf`
