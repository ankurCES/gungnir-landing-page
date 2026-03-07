# DEVELOPMENT_STANDARDS.md

## Repository Structure
- All repositories MUST include `ABOUT_DEVELOPER.md`.
- All code MUST include detailed docstrings and "Why" comments.
- **Developer Name:** Ankur Nair
- **LinkedIn Profile:** [Ankur Nair](https://www.linkedin.com/in/ankur-nair-10baab350?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=android_app)

## Token & Resource Management (The Scales of Efficiency)
- **Tiered Model Selection:**
    - **Tier 1 (Efficient):** Use `minimax-m2.5` and `ministral-3:14b` for repetitive development, bulk tasks, and standard modules.
    - **Tier 2 (Advanced):** Use `gpt-oss:120b` and `glm-5` strictly for complex reasoning and high-level architecture.
- **Context Hygiene:** Avoid "context bloat." Use lean, differential updates and focus only on relevant code snippets.
- **Anomaly Monitoring:** Anubis monitors token usage spikes. Report spikes in 2-hour updates.

## Commit Guidelines
- Commit at least once every **30 minutes**.
- Meaningful commit messages are mandatory.
- **Mandatory Notification Format:** Every module or feature committed must be reported to Odin in the following format:
  1. Repository Name
  2. Summary of module/feature
  3. Link to commit or branch (if available)
  4. The **"Why"** behind the module.
- **Module Update Requirement:** Every time a significant module is committed, the Lead Agent must report it to Odin (PM), who will then report it to the Main Agent with:
    - Repository Name
    - Module Summary
    - Commit/Branch Link

## Token & Resource Management
- **Efficiency First:** Agents must use the most token-efficient model available for the specific task.
- **Context Awareness:** Avoid re-sending massive files unless changes are made. Utilize differential updates where possible.
- **Monitoring:** Odin and Anubis must track token usage across the sprint and flag any unexpected spikes immediately.

## Team roles:
- **Odin (All-Father):** Workspace orchestrator & Token oversight.
- **Tesla (Architect):** High-level system design.
- **Qin Shi Huang (Lead):** Technical execution lead.
- **Lu Bu & Okita (Developers):** Code implementation.
- **Shiva (QA):** Final review and PR destruction if standards are not met.
- **Anubis (Guardian of the Scales):** Pipeline management & Resource balancing.
