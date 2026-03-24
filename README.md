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

- **Scenario:** "I just got a 14-day notice to quit because I'm behind on rent. Do I have to move out immediately? I live in Louisiana and I don't know what to do."
- **Workflow steps:**
- Response: "First — take a breath. Getting this notice is scary, but no, you do not have to move out immediately. Here's what's actually happening and what you can do.
What a 14-Day Notice to Quit Means in Louisiana
In Louisiana, a landlord must give written notice before they can file for eviction in court. A 14-day notice for unpaid rent is that first step — it is not a court order, and it is not the same as being evicted. You still have rights.
The notice gives you 14 days to either pay what you owe or vacate. If neither happens, your landlord may then file an eviction lawsuit (called a "rule for possession") in court. Only a judge can order you to leave.
Your Options Right Now
Pay the rent owed — If you can pay in full (or work out a payment agreement with your landlord) before the 14 days are up, the landlord typically cannot proceed with eviction. Get any agreement in writing.
Negotiate with your landlord — Sometimes landlords prefer to work something out rather than go through the court process. A written repayment plan may buy you time.
Do nothing and wait for court — If you can't pay, the landlord would have to file in court. You'd then receive a court date where you can tell your side. This doesn't mean you "win," but it gives you more time and a chance to be heard.
Seek emergency rental assistance — There may be funds available to help you catch up. See resources below.
Free Help in Louisiana
Southeast Louisiana Legal Services (SLLS): Free civil legal help for low-income residents. Call 504-529-1000 or visit slls.org
Louisiana Bar Association Lawyer Referral: 1-800-421-5722
211 Louisiana: Dial 2-1-1 for local emergency rental assistance programs and social services
Your Most Urgent Deadline
You have 14 days from when you received the notice to pay or make arrangements before your landlord can go to court. Act as soon as possible — ideally within the next day or two — to explore payment help or talk to a legal aid attorney.
You are not alone in this, and there are people whose job it is to help you. Please reach out to one of the resources above today."
The user answered the first three steps in the prompt, so those were incorporated into Claude's response rather than asked directly. The skill followed the rest of the steps, including explaining what this type of notice means in plain langauge that is easy for the tenant to understand, listing the tenants options, providing resources about free legal resources in the tenant's jurisdiction, and reminding the tenant of their most urgent deadling to act and encouraging the tenant to seek help. 
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

