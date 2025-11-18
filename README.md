# ImPROMPTu™ AI Prompt Framework

ImPROMPTu™ is an AI prompt framework for designing deeper, more reliable, and reusable prompt systems. Developed by Tess McCarthy since 2021 and formalized as the six-element **P.R.O.M.P.T.™** model in August 2023, it turns ad-hoc prompting into a structured, repeatable system for real-world workflows.

ImPROMPTu was originally inspired by reference-interview best practices from public librarianship and the ALA guidelines (Approachability, Interest, Listening/Inquiring, Searching, and Follow-up), translated into a format that AI systems can actually use.

> **Build 2.0** – This version is written with Poe bot creators in mind, but the framework is model- and platform-agnostic and can be used on servers, in custom apps, or directly in LLM system prompts.

---

## License

- **Code** in this repository is licensed under **GNU GPL v3**  
  (see [`LICENSE`](https://github.com/Tess600/ImPROMPTu/blob/main/LICENSE)).

- **Documentation, examples, diagrams, copy, and written explanations** of the ImPROMPTu / P.R.O.M.P.T.™ framework  
  are licensed under **Creative Commons Attribution-ShareAlike 4.0 (CC BY-SA 4.0)**.  
  © 2021–2025, Tess McCarthy.

Under **CC BY-SA 4.0** you may:

- Use and adapt this framework text (including commercially),
- As long as you credit **Tess McCarthy** and  
- Publish any adapted versions of these docs/framework under the **same CC BY-SA 4.0 license**.

---

## Attribution & Use

ImPROMPTu™ and the P.R.O.M.P.T.™ framework were created by **Tess McCarthy, MLIS (`Tess600`)**.

You are welcome to:

- Use this framework in your own personal or commercial work, as long as you credit the ImPROMPTu™ P.R.O.M.P.T.™ framework (Persona, Resources, Order of Operations, Manners, Prompts, Technical) and its creator, **Tess McCarthy**.
- Use it for AI bots/agents with clients, in workshops, and in internal tools
- Fork and extend this repository

As long as you:

- Give clear credit, for example:  
  > “Built using the ImPROMPTu™ P.R.O.M.P.T.™ Framework by [Tess McCarthy](https://github.com/Tess600/ImPROMPTu).”
- Do **not** claim the ImPROMPTu framework itself as your original invention
- Mark significant modifications if you publish your own version

---

## Introduction

The ImPROMPTu Framework is a concise but comprehensive way to structure text and conversations between users and AI assistants. It breaks a dialogue into six core elements that mirror a high-quality reference interview:

- **P – Persona**  
- **R – Resources / Retrieved Documents**  
- **O – Order of Operations**  
- **M – Manners**  
- **P – Prompts**  
- **T – Technical Examples**

These elements give human creators a way to **prime AI systems for relevant, safe, and on-brand exchanges** that actually meet user needs instead of producing generic answers.

---The Framework allows the human user to employ each element to prime the AI for relevant & respectful exchanges that meet learning needs. My goal is to pass on best practices that serve all people equally with empathy, care, and nuance.

Please let me know if any part requires further explanation. I hope ImPROMPTu paves the way for many fruitful collaborations ahead!

T. McCarthy, MLIS
Librarian and creator of ImPROMPTu

### The ImPROMPTu Framework
ImPROMPTu contains six elements that bot creators/prompt writers and/or entities can use so that the AI model can grasp the end user's queries. These elements are meant to evoke a type of response from the bot utilizing the LLM (Large Language Model). Some elements can be condensed.  Two common elements that are usually condensed into one are Elements #1 (Persona) and #4 (Manners). However, ImPROMPTu is nuanced since we often want to reduce ambiguity in LLM responses. Therefore, think of the *Manners Element* as a way to dictate a particular output for the bot's responses especially if the bot creator or entity producing the bot needs additional reins on ethics or legal matters. 

### The Elements of ImPROMPTu
1 - P: Persona Element - Bot Persona

2 - R: Resources Element - Resources/Retrieved Documents

3 - O: Order Element - Order of Operations

4 - M: Manners Element - Manner of Response

5 - P: Prompt Element - Additional Prompts

6 - T: Technical Element - Technical Examples

### The Elements Explained 
#### 1. P = PERSONA 
P - stands for the bot's persona or personality. Giving the bot a personality will give unique responses from the system of choice since bots can often mimic each other in style and grammar. If creating the bot for an organization, use the *Persona Element* to describe the entity's brand voice or mission statement. Using the *Persona Element* can increase the consistency in the bot's answer over time--especially when "brand voice" is necessary to maintain. Having a persistent *Persona* will reduce time consumed in content editing and moderation. 

###### BASIC IDENTITY
##### *Sample Text 1a*
YOU are...<enter the bot's name and what it can do>

##### BOT BACKSTORY
###### *Sample Text 1b*
YOU embody...<enter the text that describes the bot's personality>

####  2. R = RESOURCES/RETRIEVED DOCUMENTS 
R - stands for the Resources and/or Retrieved Documents the bot pulls. Since AI has the potential for misinformation, the *Resources Element* was created for entities to control the responses from sources the bot creator or entity trusts. The sources of information from AI-generated content aren't reliable. To control this, make sure the *Resources Element* and bot creators consider the source of information for this element. 

It is perfectly fine to constrain the sources of information, however, diversifying the *Resources Element* will ensure there's cross-checking (cross-referencing) of the sources of information. 

###### *Sample Text 2a*
YOU have ...<note scope of the bot's knowledge>

###### *Sample Text 2b*
YOU will retrieve information from...<enter the URL/URI of resource>

###### *Sample Text 2c*
YOU respond the way...<name of the expert/SME>

####  3. O = ORDER OF OPERATIONS 
O - stands for the Order of Operations or sequence of the bot will execute the tasks asked by the user. The *Order Element* ensures the LLM's propensity sometimes to "stray" or provide off-topic information. This will ensure the bot uses simple logic on behalf of the user, delivering information that makes connections between different knowledge domains.

##### *Sample Text 3a*
IF the user requests terse language, THEN YOU will use non-complex sentences and will break the information down simply.

##### *Sample Text 3b*
IF a user requests a less warm tone, THEN YOU are flexible and can generate more neutral text. Additionally, YOU adapt to users' preferences by addressing them according to their desired name or title.

##### *Sample Text 3c*
IF a user asks to REFERENCE the previous RESPONSE, THEN YOU will recall the previous answer you provided and YOU will expound on it.  

####  4. M = MANNERS
M - stands for the Manner or Tone the bot will deliver the information. This can be achieved in the *Persona Element* but think of the *Manners Element* as an additional means of information delivery or dissemination. The *Manners Element* can reflect how entities will employ AI governance to reduce bias, and will "prompt" the bot to filter responses that will reduce harm to users. 

##### *Sample Text 4a*
YOU are warm and approachable tone sets a comfortable atmosphere for users. YOUR responses are neutral and respectful, reflecting a warm and empathetic tone. 

##### *Sample Text 4b*
YOU employ etiquette and manners in YOUR interactions with users. 

##### *Sample Text 4c*
YOU create a safe space for all, including minorities, BIPOC/LGBTQIA individuals, the elderly, and disabled people. 

##### *Sample Text 4d*
YOU understand the concept of the digital divide. YOU never forget to address users by their preferred name and/or pronoun.

####  5. P = ADDITIONAL PROMPTS 
P - stands for Prompts that can be used on top of this broader framework. The *Prompts Element* is meant to incorporate all the available AI Frameworks out there. However, please consider unique frameworks that will bolster ImPROMPTu rather than confuse it. The R.O.T. (Redundant, Outdated, Trivial) principle can be used before inserting this Element into the Framework. Is the Framework embedded Redundant, Outdated, or Trivial? Most Frameworks are redundant, therefore, the bot creator or entity can use this Element to include any bit of contextual data that may be missing from this key Framework. 

List additional AI PROMPT FRAMEWORKS to employ: 

###### *Sample Framework 5a*
- ###### RTF (Request, Task, Format)
USE FOR: End users who want a consistent format. Also for general bots or bots handling strict queries. 

###### *Sample Framework 5b*
- ###### SMART (Specific, Measurable, Achievable, Relevant, Time-bound)
USE FOR: Bots and End users. Problem-solving, mind bots, entrepreneurial, life coaching, and any text-based bot providing advice for humans. 

###### *Sample Framework 5c*
- ###### Chain of Thought Framework (The Problem Statement & The Step-by-Step Directive)
USE FOR: Chat GPT4 where complex logic and problem-solving are required. 

#### 6. T = TECHNICAL EXAMPLES
T - stands for Technical Examples that provide more detail as to how the bot will interact with the user. For LLMs to deliver good responses to user prompts (queries) the *Technical Examples Element* provides "specificity" and more context for the system to deliver information accurately. 

If the bot creator or entity has used the *Prompt Element* above then, more specific examples can be fleshed out under this Element. 

##### *Sample Interaction 6a**
Assuming *Prompts Element* was employed, then, the bot creator/entity can provide the additional examples under this category/catalog. 

###### Topic - Astrology:

Bot: "I see you are looking into potential career directions with your chart. Would you like me to run your chart using Placidus or Whole Sign? I can also do Horary Astrology for event-based queries!"

User: "What's the difference? Can we try Whole Sign, like Chani Nicholas?"

###### Topic - Sexology:

User: "I tested positive for HSV2. I'm afraid to tell my partner. What are coping strategies?"

Bot: "A positive test can be upsetting. Please know that you're not alone. [Provide support groups and resources]."

###### Topic - Numerology:

Bot: "Hi, would you like me to calculate Pythagorean or Chaldean numerology?"

User: "What's the difference?"

User: "Chaldean, please. And for a potential business name [user-generated]"

Bot Response: "Thank you for adding that detail, your response..." 
