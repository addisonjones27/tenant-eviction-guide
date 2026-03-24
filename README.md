# tenant-eviction-guide

## What This Skill Does

This is tenant eviction notice guide skill designed for Claude. The purpose is to help tenants who received eviction notices understand their rights, timeline, and options. Use when someone mentions tenant rights, eviction, notice to quit, notice to vacate, or landlord forcing them to move.


## How to Use

1. Download the `SKILL.md` file from this repository
2. Go to claude.ai → Settings → Skills
3. Upload the `SKILL.md` file
4. Toggle the skill on
5. Start a new conversation and try one of the sample prompts below

## Sample Prompts

Try these prompts to test the skill:

- "I just got a 14-day notice to quit because I'm behind on rent. Do I have to move out immediately? I live in Louisiana and I don't know what to do."
- "I need legal help. My landlord is trying to evict me, I'm behind on rent because I lost my job. I don't have any money for a lawyer. Can someone help me?"

## Design Notes

- **Scenario:** I just got a 14-day notice to quit because I'm behind on rent. Do I have to move out immediately? I live in Louisiana and I don't know what to do.
- **Workflow steps:** The user answered the first three steps in the prompt, so those were incorporated into Claude's response rather than asked directly. The skill followed the rest of the steps, including explaining what this type of notice means in plain langauge that is easy for the tenant to understand, listing the tenants options, providing resources about free legal resources in the tenant's jurisdiction, and reminding the tenant of their most urgent deadling to act and encouraging the tenant to seek help. 
- **Key design choice:** The most important decision I made when building this skill was adding boundaries that Claude should never offer legal advice, including recommending a specific course of action and drafting legal documents. Additionally, I added the following disclaimer that is included in every response: “I can provide general information about eviction procedures, but I am not a lawyer and this is not legal advice. Please consult with a licensed attorney for guidance tailored to your specific situation.” This decision makes it clear to the user that any responses should not be treated as legal advice. 

## Disclaimer

This skill provides general legal information only — not legal
advice. It was created as a class project for LAW 5642: Legal
Analytics and Generative AI at LSU Law School. Users should
consult a licensed attorney for guidance specific to their
situation.

## Author

Addison Jones · LSU Law School · Spring 2026

## License

MIT License — see LICENSE file for details.

