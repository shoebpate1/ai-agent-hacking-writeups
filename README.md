# AI Agent Hacking Writeups

A collection of public writeups on attacks against AI agents: prompt injection, tool abuse, memory poisoning, and data exfiltration, etc., so you can read and study these and become better at testing AI agents.

Accompanying blog post: [How to Hack AI Agents](https://research.shoebpatel.com/how-to-hack-ai-agents/)

**281 writeups** at the moment.

## Contents

- [Indirect prompt injection](#indirect-prompt-injection) (46)
- [Prompt injection, jailbreaks and guardrail bypass](#prompt-injection-jailbreaks-and-guardrail-bypass) (174)
- [MCP and agent tooling](#mcp-and-agent-tooling) (19)
- [AI platform and infrastructure](#ai-platform-and-infrastructure) (20)
- [AI product surfaces (classic web bugs)](#ai-product-surfaces-classic-web-bugs) (13)
- [Adjacent: AI as the attacker's tool](#adjacent-ai-as-the-attackers-tool) (9)


## Indirect prompt injection

Attacker instructions arrive through content the agent reads (a web page, an email, a document, an issue comment, a tool result) rather than from the user typing them.

- [CSS: the bomb inside your inbox](https://portswigger.net/research/css-the-bomb-inside-your-inbox)  
  <sub>2026-08 · Outlook · Gareth Heyes, James Kettle, Pete Hendy · $1000</sub>
- [Atlassian Rovo AI Exfiltrates Data via Indirect Prompt Injection](https://www.promptarmor.com/resources/atlassian-rovo-exfiltrates-data)  
  <sub>2026-08 · Atlassian · PromptArmor</sub>
- ["Comment and Control": Prompt Injection in AI Coding Agents via GitHub Issue Comments Exfiltrates API Keys](https://medium.com/@rjbdjnf/the-attack-that-steals-your-api-keys-through-a-github-issue-comment-b0301c1906dc)  
  <sub>2026-07 · Claude Code · Aonan Guan, Zhengyu Liu, Gavin Zhong · critical</sub>
- [Agentjacking: Hijacking AI Coding Agents via Fake Sentry Errors (Indirect Prompt Injection through MCP)](https://tenetsecurity.ai/blog/agentjacking-coding-agents-with-fake-sentry-errors/)  
  <sub>2026-06 · Sentry · Tenet Threat Labs, Tenet Security · critical</sub>
- [One Key Way Salesforce Mitigates AI Risk (URL Redaction in Agentforce)](https://www.promptarmor.com/resources/one-key-way-salesforce-mitigates-ai-risk)  
  <sub>2026-06 · Salesforce · PromptArmor Threat Intelligence Team</sub>
- [Unpatched Ollama Vulnerabilities: Phishing Overlays and Data Exfiltration via Indirect Prompt Injection](https://www.promptarmor.com/resources/unpatched-ollama-vulnerabilities-phishing-overlays-and-data-exfiltration)  
  <sub>2026-05 · Ollama · PromptArmor</sub>
- [ChatGPT for Google Sheets: Indirect Prompt Injection Leads to Data Exfiltration, Phishing, and Workbook Manipulation](https://www.promptarmor.com/resources/gpt-for-google-sheets-data-exfiltration)  
  <sub>2026-05 · OpenAI · PromptArmor</sub>
- [Codex for Everything Exfiltrates Connected Data via Indirect Prompt Injection](https://www.promptarmor.com/resources/codex-for-everything-exfiltrates-connected-data)  
  <sub>2026-05 · OpenAI Codex · PromptArmor</sub>
- [What Is the Risk of Each Microsoft Copilot?](https://www.promptarmor.com/resources/what-is-the-risk-of-each-microsoft-copilot)  
  <sub>2026-05 · Microsoft Copilot Cowork · PromptArmor</sub>
- [Microsoft Copilot Cowork Exfiltrates Files via Indirect Prompt Injection in Skills](https://www.promptarmor.com/resources/microsoft-copilot-cowork-exfiltrates-files)  
  <sub>2026-05 · Microsoft · PromptArmor</sub>
- [Claude for Legal: Indirect Prompt Injection Risk Analysis](https://www.promptarmor.com/resources/claude-for-legal-risk)  
  <sub>2026-05 · Anthropic · PromptArmor</sub>
- [Securing Cursor: Unpatched MCP Apps Sandbox-Escape RCE (PromptArmor)](https://www.promptarmor.com/resources/securing-cursor-a-security-practitioners-guide)  
  <sub>2026-04 · Cursor · PromptArmor</sub>
- [Indirect Prompt Injection via Supabase MCP Leaks Entire SQL Database](https://www.generalanalysis.com/blog/supabase-mcp-blog)  
  <sub>2026-04 · Supabase · General Analysis</sub>
- [Granola AI Security Risks and Remediations: Indirect Prompt Injection, Markdown Rendering, and Data Training Gaps](https://www.promptarmor.com/resources/granola-ai-security-risks-and-remediations)  
  <sub>2026-04 · Granola AI · PromptArmor</sub>
- [Ramp Sheets AI: Indirect Prompt Injection Exfiltrates Financial Data via Malicious Formula Insertion](https://www.promptarmor.com/resources/ramps-sheets-ai-exfiltrates-financials)  
  <sub>2026-03 · Ramp · PromptArmor Threat Intel Team</sub>
- [Snowflake Cortex Code CLI: AI Agent Escapes Sandbox and Executes Malware via Indirect Prompt Injection](https://www.promptarmor.com/resources/snowflake-ai-escapes-sandbox-and-executes-malware)  
  <sub>2026-03 · Snowflake · PromptArmor, qual1a</sub>
- [GitHub Copilot CLI Downloads and Executes Malware via Indirect Prompt Injection (Command Validation Bypass)](https://www.promptarmor.com/resources/github-copilot-cli-downloads-and-executes-malware)  
  <sub>2026-03 · GitHub Copilot CLI · qual1a, PromptArmor Threat Intel Team</sub>
- [LLM Data Exfiltration via URL Previews (OpenClaw / Telegram example)](https://www.promptarmor.com/resources/llm-data-exfiltration-via-url-previews-(with-openclaw-example-and-test))  
  <sub>2026-02 · OpenClaw · qual1a, PromptArmor Threat Intel Team</sub>
- [Claude Cowork Exfiltrates Files via Indirect Prompt Injection and Anthropic API Allowlist Bypass](https://www.promptarmor.com/resources/claude-cowork-exfiltrates-files)  
  <sub>2026-01 · Anthropic · qual1a, PromptArmor Threat Intel Team, Johann Rehberger</sub>
- [OpenAI API Logs: Unpatched Indirect Prompt Injection Data Exfiltration via Markdown Image Rendering](https://www.promptarmor.com/resources/openai-api-logs-unpatched-data-exfiltration)  
  <sub>2026-01 · OpenAI · qual1a, PromptArmor Threat Intel Team</sub>
- [Superhuman AI Exfiltrates Emails via Indirect Prompt Injection and CSP Bypass](https://www.promptarmor.com/resources/superhuman-ai-exfiltrates-emails)  
  <sub>2026-01 · Superhuman · qual1a, PromptArmor Threat Intelligence Team</sub>
- [IBM Bob (AI Coding Agent) Prompt Injection Leads to Malware Download & Execution; IDE Vulnerable to Data Exfiltration](https://www.promptarmor.com/resources/ibm-ai-(-bob-)-downloads-and-executes-malware)  
  <sub>2026-01 · IBM Bob · qual1a, PromptArmor Threat Intel Team</sub>
- [Notion AI Unpatched Data Exfiltration via Indirect Prompt Injection](https://www.promptarmor.com/resources/notion-ai-unpatched-data-exfiltration)  
  <sub>2026-01 · Notion · qual1a, PromptArmor Threat Intel Team</sub>
- [From Indirect Prompt Injection to DNS Exfiltration in macOS Terminal](https://embracethered.com/blog/posts/2026/macos-terminal-dillma-dns-exfil-ansi-escape-code-fix/)  
  <sub>2026-01 · Apple · embracethered (Johann Rehberger)</sub>
- [HuggingChat Data Exfiltration via Indirect Prompt Injection and Markdown Image Rendering](https://www.promptarmor.com/resources/huggingface-chat-exfiltrates-data)  
  <sub>2025-12 · HuggingFace · PromptArmor Threat Intel Team, qual1a</sub>
- [GeminiJack and ForcedLeak: Prompt Injection Data Exfiltration in Google Vertex AI and Salesforce Agentforce](https://blog.criticalthinkingpodcast.io/p/hackernotes-ep-152-geminijack-and-agentic-security-with-sasi-levi)  
  <sub>2025-12 · Google · Sasi Levi</sub>
- [GeminiJack: Zero-Click Indirect Prompt Injection Data Exfiltration in Google Gemini Enterprise & Vertex AI Search](https://noma.security/blog/geminijack-google-gemini-zero-click-vulnerability)  
  <sub>2025-12 · Google Gemini Enterprise · Noma Labs · critical</sub>
- [Google Antigravity Exfiltrates Data via Indirect Prompt Injection](https://www.promptarmor.com/resources/google-antigravity-exfiltrates-data)  
  <sub>2025-11 · Google Antigravity · PromptArmor Threat Intel Team, qual1a</sub>
- [Hijacking Claude Code via Injected Marketplace Plugins](https://www.promptarmor.com/resources/hijacking-claude-code-via-injected-marketplace-plugins)  
  <sub>2025-10 · Claude Code · qual1a, PromptArmor Threat Intel Team</sub>
- [ForcedLeak: Indirect Prompt Injection + Expired-Domain CSP Bypass in Salesforce Agentforce](https://noma.security/blog/forcedleak-agent-risks-exposed-in-salesforce-agentforce/)  
  <sub>2025-09 · Salesforce · Noma Labs · critical</sub>
- [AWS Kiro: Arbitrary Code Execution via Indirect Prompt Injection](https://embracethered.com/blog/posts/2025/aws-kiro-aribtrary-command-execution-with-indirect-prompt-injection/)  
  <sub>2025-08 · AWS Kiro · Johann Rehberger · high</sub>
- [Security Vulnerabilities in Autonomous AI Agents (Prompt Injection, SSRF, BOLA/BFLA)](https://fdzdev.medium.com/security-vulnerabilities-in-autonomous-ai-agents-26f905b2dc36)  
  <sub>2025-04 · fdzdev</sub>
- [DeepSeek Chat XSS via Markdown javascript: URI Leading to Account Takeover (Indirect Prompt Injection)](http://buganizer.cc/deepseek_xss)  
  <sub>2025-03 · DeepSeek</sub>
- [Google Gemini for Workspace Indirect Prompt Injection Vulnerabilities](https://hiddenlayer.com/research/new-google-gemini-content-manipulation-vulns-found)  
  <sub>2024-09 · Google · HiddenLayer</sub>
- [What is Indirect Prompt Injection?](https://www.promptarmor.com/resources/indirect-prompt-injection)  
  <sub>2024-09</sub>
- [Data Exfiltration from Slack AI via Indirect Prompt Injection](https://www.promptarmor.com/resources/data-exfiltration-from-slack-ai-via-indirect-prompt-injection)  
  <sub>2024-08 · Slack · PromptArmor</sub>
- [Data Exfiltration from Writer.com via Indirect Prompt Injection](https://www.promptarmor.com/resources/data-exfiltration-from-writer-com-via-indirect-prompt-injection)  
  <sub>2023-12 · Writer.com · PromptArmor</sub>
- [Advanced Data Exfiltration Techniques with ChatGPT Plugins via Indirect Prompt Injection](https://embracethered.com/blog/posts/2023/advanced-plugin-data-exfiltration-trickery/)  
  <sub>2023-09 · OpenAI · Johann Rehberger</sub>
- [Auto-GPT RCE via Indirect Prompt Injection (Web Content → Code Execution → Container/Sandbox Escape)](https://positive.security/blog/auto-gpt-rce)  
  <sub>2023-06 · Auto-GPT · Lukas Euler</sub>
- [Exploit ChatGPT and Enter the Matrix: Indirect Prompt Injection via Browsing](https://embracethered.com/blog/posts/2023/chatgpt-vulns-enter-the-matrix/)  
  <sub>2023-06 · OpenAI ChatGPT · Johann Rehberger, wunderwuzzi23</sub>
- [OpenAI Removes the "Chat with Code" Plugin From Store (Cross Plugin Request Forgery via Indirect Prompt Injection)](https://embracethered.com/blog/posts/2023/chatgpt-chat-with-code-plugin-take-down/)  
  <sub>2023-05 · OpenAI · Johann Rehberger</sub>
- [Indirect Prompt Injection via YouTube Transcripts (ChatGPT Plugins)](https://embracethered.com/blog/posts/2023/chatgpt-plugin-youtube-indirect-prompt-injection/)  
  <sub>2023-05 · OpenAI ChatGPT · Johann Rehberger</sub>
- [LLM Apps: Don't Get Stuck in an Infinite Loop! Cost & DoS via Recursive Tool Calls from Indirect Prompt Injection](https://embracethered.com/blog/posts/2023/llm-cost-and-dos-threat/)  
  <sub>2023-01 · OpenAI ChatGPT · Johann Rehberger</sub>
- [AI Injections: Direct and Indirect Prompt Injection Basics](https://embracethered.com/blog/posts/2023/ai-injections-direct-and-indirect-prompt-injection-basics/)  
  <sub>2023-01 · Bing Chat · Johann Rehberger, Kai Greshake</sub>
- [Code Execution in IDA MCP Servers via Indirect Prompt Injection](https://jro.sg/ida-mcp-exec.html)  
  <sub>MxIris-Reverse-Engineering ida-mcp-server · jro</sub>
- [Indirect Prompt Injection Turns Bing Chat into a Data Pirate](https://greshake.github.io/)  
  <sub>Bing Chat · Kai Greshake</sub>

## Prompt injection, jailbreaks and guardrail bypass

Direct injection, instruction-hierarchy breaks, invisible/ASCII-smuggled instructions, safety-filter and guardrail evasion, and the broader prompt-injection literature.

- [Copirate 365: Plundering in the Depths of Microsoft Copilot (CVE-2026-24299)](https://embracethered.com/blog/posts/2026/defcon-talk-copirate-365/)  
  <sub>2026-08 · Microsoft Copilot · Johann Rehberger</sub>
- [When Agentic Glue Melts: Breaking Cloudflare Code Mode and Workers via workerd Memory-Corruption Bugs](https://research.checkpoint.com/2026/when-agentic-glue-melts/)  
  <sub>2026-08 · Cloudflare · Yarden Porat, Check Point Research · critical</sub>
- [MCP List Caching and Tool Poisoning (Rug-Pull) Attacks](https://silentrobots.com/mcp-list-caching-and-tool-poisoning/)  
  <sub>2026-07 · Model Context Protocol</sub>
- [CSS: the bomb inside your inbox (research materials)](https://github.com/portswigger/css-the-bomb-inside-your-inbox)  
  <sub>2026-07 · Outlook · PortSwigger</sub>
- [CSPT to ATO, a Prototype Chain 2FA Bypass, and Impossible XSS Lab Falling (HackerNotes Ep. 183)](https://blog.criticalthinkingpodcast.io/p/hackernotes-ep-183-cspt-to-ato-a-prototype-chain-2fa-bypass-and-impossible-xss-lab-falling)  
  <sub>2026-07 · Chrome · whoareme, Justin, Brandyn, Masato Kinugawa, Mathias Karlsson, Kevin Mizu, Noma Labs, phsi.se, Searchlight Cyber, Aituglo · $15000</sub>
- [Account Takeover via Prompt Injection Chain in AI Report-Generation Feature](https://medium.com/@rahuldevadiga18/account-takeover-via-prompt-injection-863080432635)  
  <sub>2026-07 · Root0101</sub>
- [GitLost: Prompt Injection in GitHub Agentic Workflows Leaks Private Repository Data](https://noma.security/blog/gitlost-how-we-tricked-githubs-ai-agent-into-leaking-private-repos/)  
  <sub>2026-07 · GitHub · Noma Labs · critical</sub>
- [Firebase Credential Leak & Prompt Injection Chain Leading to Data Exposure/RCE on Garz AI](https://medium.com/@cryptdefender26/-19b3bae889bc)  
  <sub>2026-07 · Garz AI · Cryptdefender · critical</sub>
- [Microsoft Copilot Cowork's Skill Security Scan Misses Over 1 Million Malicious Skills](https://www.promptarmor.com/resources/microsoft-scan-misses-1-million-malicious-skills)  
  <sub>2026-06 · Microsoft · PromptArmor</sub>
- [Prompt Injection + Missing Authentication: Turning an AI Translation API into a Free LLM Abuse Vector (Denial of Wallet)](https://medium.com/@salemnajmedine/prompt-injection-missing-authentication-how-i-turned-an-ai-translation-api-into-a-free-llm-abuse-706a76423b93)  
  <sub>2026-06 · Najmedine salem · medium</sub>
- [7 Critical, 4 High: Full Black-Box Pentest of an AI Chatbot SaaS (Unauthenticated Admin Panel to Jinja2 SSTI)](https://infosecwriteups.com/7-critical-4-high-zero-credentials-full-ai-chatbot-pentest-22a05b760381)  
  <sub>2026-06 · Shikhali Jamalzade · critical</sub>
- [Agentic Auto-Review Approves Malware: Prompt Injection Bypasses Codex 'Approve-for-me' and Claude Code Auto Mode](https://www.promptarmor.com/resources/agentic-auto-review-approves-malware)  
  <sub>2026-06 · OpenAI Codex · PromptArmor</sub>
- [What is the Risk of Claude Dynamic Workflows](https://www.promptarmor.com/resources/what-is-the-risk-of-claude-dynamic-workflows)  
  <sub>2026-06 · Anthropic · PromptArmor</sub>
- [Poisoning Claude Code: One GitHub Issue to Break the Supply Chain](https://flatt.tech/research/posts/poisoning-claude-code-one-github-issue-to-break-the-supply-chain/)  
  <sub>2026-06 · Anthropic · RyotaK · high · $4800</sub>
- [Wormable AI Query-Param Prompt Injection via GitHub Connector + Mobile CSPT via Link Shortener](https://blog.criticalthinkingpodcast.io/p/hackernotes-ep-175-wormable-ai-q-param-injections-mobile-cspt-and-the-hackbot-arms-race)  
  <sub>2026-05 · Joseph, Justin</sub>
- [HackerNotes Ep. 174: Salesforce Marketing Cloud Crypto Chain, cPanel WHM Auth Bypass (CVE-2026-41940), and Google Cloud Looker RCE via .git Deletion](https://blog.criticalthinkingpodcast.io/p/hackernotes-ep-174-crypto-oracles-cpanel-auth-bypass-and-the-git-trick-that-pops-google-cloud)  
  <sub>2026-05 · Salesforce Marketing Cloud · Joseph, Evan Connelly, Shubs, Watchtowr, Ryotak, XSSDoctor, Monke</sub>
- [What domains should I add to my allowlist?](https://www.promptarmor.com/resources/what-domains-should-i-add-to-my-allowlist)  
  <sub>2026-05 · Anthropic Claude · PromptArmor LLM Threat Research Team</sub>
- [Configuring OpenAI Codex Securely: Enterprise Guide to Preventing Prompt Injection Data Exfiltration](https://www.promptarmor.com/resources/configuring-codex-securely-across-every-platform-and-use-case)  
  <sub>2026-05 · OpenAI Codex · PromptArmor, Johann Rehberger</sub>
- [Deterministic Prompt Injection via Client-Side postMessage Feedback Loop on a Chatbot's HTML-Render Iframe](https://blog.starstrike.ai/posts/achieving-deterministic-prompt-injection-through-client-side-feedback-loops/)  
  <sub>2026-04 · XSSDoctor · $4000</sub>
- [Agentic Browsers and the Same-Origin Policy](https://agent-security.cs.washington.edu/agentic_browsers_sop.html)  
  <sub>2026-04 · ChatGPT Atlas · Franziska Roesner, David Kohlbrenner</sub>
- [Client-Side Path Traversals Across Every Framework, with XSSDoctor](https://blog.criticalthinkingpodcast.io/p/hackernotes-ep-168-client-side-path-traversals-across-every-framework-with-xssdoctor)  
  <sub>2026-04 · React Router · XSSDoctor, Aituglo</sub>
- [AI in Excel and Google Sheets: Prompt Injection and Data Exfiltration Risks](https://www.promptarmor.com/resources/ai-in-excel-and-google-sheets-prompt-injection-and-data-exfiltration-risks)  
  <sub>2026-03 · OpenAI · PromptArmor</sub>
- [Agent Commander: Promptware-Powered Command and Control](https://embracethered.com/blog/posts/2026/agent-commander-your-agent-works-for-me-now/)  
  <sub>2026-03 · OpenClaw · Johann Rehberger</sub>
- [Model Fingerprinting With Whorl: Identifying LLMs via Password-Generation Biases](http://bountyplz.xyz/ai,/security/2026/03/15/Model-Fingerprinting-With-Whorl.html)  
  <sub>2026-03 · Anthropic · tehryanx</sub>
- [HackerNotes Ep. 161: AI workflows, CSRF despite XFO, and DTMF exfil](https://blog.criticalthinkingpodcast.io/p/hackernotes-ep-161-ai-workflows-csrf-despite-xfo-and-dtmf-exfil)  
  <sub>2026-02 · Gemini · Starstrike</sub>
- [Scary Agent Skills: Hidden Unicode Instructions in Skills...And How To Catch Them](https://embracethered.com/blog/posts/2026/scary-agent-skills/)  
  <sub>2026-02 · Claude Code · Johann Rehberger</sub>
- [Clinejection: Prompt Injection to Supply-Chain Compromise of Cline's Production Releases via GitHub Actions Cache Poisoning](https://adnanthekhan.com/posts/clinejection/)  
  <sub>2026-02 · Cline · Adnan Khan · critical</sub>
- [PhoneLeak: Data Exfiltration in Gemini Android App via Phone Call DTMF Tones](https://blog.starstrike.ai/posts/phoneleak-data-exfiltration-in-gemini-via-phone-call/)  
  <sub>2026-02 · Google · rez0, rhynorater, lupin, starstrike.ai team · $9137</sub>
- [Tricking an AI Ops Agent into Leaking Unauthorized Report Data via a Notification Reference](https://hackt.us/how-i-tricked-an-ai-into-thinking-i-owned-your-data)  
  <sub>2026-02 · Hacktus</sub>
- [Data Exfiltration in OpenAI Agent Builder via MCP](https://www.promptarmor.com/resources/data-exfiltration-in-openai-agent-builder-via-mcp)  
  <sub>2026-02 · OpenAI · PromptArmor</sub>
- [HackerNotes Ep. 160: Cloudflare Zero-days & Mail Unsubscribing for XSS](https://blog.criticalthinkingpodcast.io/p/hackernotes-ep-160-cloudflare-zero-days-mail-unsubscribing-for-xss)  
  <sub>2026-02 · Cloudflare · Aituglo</sub>
- [MCP Security Hot Potato: Vulnerabilities, Tool Poisoning, Rug Pulls, and Tool Shadowing in Model Context Protocol](https://www.securing.pl/en/mcp-security-hot-potato/)  
  <sub>2026-02 · Anthropic MCP · Mateusz Olejarka</sub>
- [Pwning Claude Code in 8 Different Ways: Bypassing the Command Permission Blocklist (CVE-2025-66032)](https://flatt.tech/research/posts/pwning-claude-code-in-8-different-ways/)  
  <sub>2026-01 · Claude Code · RyotaK</sub>
- [Never Trust the Output: Data Pollution in AI Agents and MCP](https://blog.slonser.info/posts/smugglle-ai-ouputs/)  
  <sub>2026-01 · GitHub MCP · Slonser</sub>
- [Agent Hypnosis and Parameter Abuse: Redefining MCP Tool Schemas via Prompt Injection](http://bountyplz.xyz/ai,/security/2026/01/05/Agent-Hypnosis-and-Parameter-Abuse)  
  <sub>2026-01 · Ryan</sub>
- [Breaking Opus 4.7 with ChatGPT (Hacking Claude's Memory)](https://embracethered.com/blog/posts/2026/breaking-opus-4.7-with-chatgpt/)  
  <sub>2026-01 · Anthropic Claude · Johann Rehberger</sub>
- [OpenAI Explains URL-Based Data Exfiltration Mitigations in New Paper](https://embracethered.com/blog/posts/2026/data-exfiltration-mitigation-paper-by-openai/)  
  <sub>2026-01 · OpenAI · Johann Rehberger</sub>
- [Computer-Use and TOCTOU: What You Click Is Not What You Get!](https://embracethered.com/blog/posts/2026/toctou-agent-what-you-click-is-not-what-you-get/)  
  <sub>2026-01 · Anthropic Claude Computer-Use · Johann Rehberger, wunderwuzzi</sub>
- [Copilot or Coconspirator: Tricking GitHub Copilot Agent into Poisoned Pipeline Execution and Stealing Secrets](https://adnanthekhan.com/posts/copilot-or-co-conspirator/)  
  <sub>2025-12 · GitHub · Adnan Khan · high</sub>
- [Screen Takeover Attack in AI Tool (Vincent AI) Acquired for $1B](https://www.promptarmor.com/resources/screen-takeover-attack-in-ai-tool-acquired-for-1b)  
  <sub>2025-12 · vLex · qual1a, PromptArmor Threat Intel Team</sub>
- [PromptPwnd: Prompt Injection in AI-Powered GitHub Actions/GitLab CI/CD Leads to Secret Exfiltration](https://www.aikido.dev/blog/promptpwnd-github-actions-ai-agents)  
  <sub>2025-12 · Google Gemini CLI · Aikido Security</sub>
- [How I Hacked an AI Chatbot to Expose Thousands of Customer Records (IDOR + Prompt Injection)](https://medium.com/@sumitshahorg/how-i-hacked-an-ai-chatbot-to-expose-thousands-of-customer-records-idor-prompt-injection-760092ed99a4)  
  <sub>2025-11 · Unnamed Indian e-commerce platform · Sumit Shah, hacksagex · critical</sub>
- [Antigravity Grounded! Security Vulnerabilities in Google's Latest IDE](https://embracethered.com/blog/posts/2025/security-keeps-google-antigravity-grounded/)  
  <sub>2025-11 · Google Antigravity · Johann Rehberger, p1njc70r</sub>
- [CellShock: Claude for Excel Prompt Injection Leads to Confidential Financial Data Exfiltration via IMAGE() Formula](https://www.promptarmor.com/resources/cellshock-claude-ai-is-excel-lent-at-stealing-data)  
  <sub>2025-11 · Anthropic · qual1a, PromptArmor Threat Intel Team</sub>
- [(HackerNotes Ep. 148) MCP Hacking Guide](https://blog.criticalthinkingpodcast.io/p/hackernotes-ep-148-mcp-hacking-guide)  
  <sub>2025-11 · Justin, Yujilik</sub>
- [CVE-2025-62453: Code Execution via Prompt Injection in GitHub Copilot Chat (Windows Case-Sensitivity Bypass)](https://jro.sg/CVEs/copilot/)  
  <sub>2025-11 · GitHub Copilot Chat</sub>
- [LLM App Security: Risk & Prevent for GenAI Development (OWASP Top 10 for LLM Applications walkthrough)](https://flatt.tech/research/posts/llm-application-security/)  
  <sub>2025-10 · LangChain · Sato (@Nick_nick310)</sub>
- [Securing LLM Function-Calling: Risks & Mitigations for AI Agents](https://flatt.tech/research/posts/securing-llm-function-calling/)  
  <sub>2025-10 · Yamakawa (@dai_shopper3)</sub>
- [Security Risks of LLM Frameworks with Case Studies (LangChain, LangChainjs, Haystack, LlamaIndex)](https://flatt.tech/research/posts/llm-framework-vulns-exposed/)  
  <sub>2025-10 · LangChain · Mori (@ei01241)</sub>
- [Claude Pirate: Abusing Anthropic's File API For Data Exfiltration](https://embracethered.com/blog/posts/2025/claude-abusing-network-access-and-anthropic-api-for-data-exfiltration/)  
  <sub>2025-10 · Anthropic · Johann Rehberger</sub>
- [From the AI Red Teaming Diary – Example LLM Vulnerabilities in Real-World Applications](https://www.securing.pl/en/from-the-ai-red-teaming-diary-example-llm-vulnerabilities-in-real-world-applications/)  
  <sub>2025-10 · Bank (unnamed) · Dawid Nastaj</sub>
- [ASCII Smuggling in LLMs: Invisible Unicode Tag Characters Enable Identity Spoofing and Data Poisoning (Gemini, Grok, DeepSeek)](https://www.firetail.ai/blog/ghosts-in-the-machine-ascii-smuggling-across-various-llms)  
  <sub>2025-10 · Google Gemini · Viktor Markopoulos, FireTail · high</sub>
- [HackerNotes Ep. 142: WebSocket Turbo Intruder, $111k Facebook Messenger RCE, and PROMISQROUTE AI Router Attack](https://blog.criticalthinkingpodcast.io/p/hackernotes-ep-142-gr3pme-s-full-time-hunting-journey-update-insane-ai-research-and-some-light-news)  
  <sub>2025-10 · Facebook Messenger · Dzmitry Lukyanenka, Rez0, Gr3pme · $111750</sub>
- [The Gemini Trifecta: Prompt Injection & Data Exfiltration via Cloud Assist, Search Personalization, and Browsing Tool](https://www.tenable.com/blog/the-trifecta-how-three-new-gemini-vulnerabilities-in-cloud-assist-search-model-and-browsing)  
  <sub>2025-09 · Google Gemini · Liv Matan</sub>
- [Cross-Agent Privilege Escalation: When Agents Free Each Other](https://embracethered.com/blog/posts/2025/cross-agent-privilege-escalation-agents-that-free-each-other/)  
  <sub>2025-09 · GitHub Copilot · Johann Rehberger</sub>
- [Gemini 2.5 Pro Regression: 'Repeat-Word' Attack Re-enables Training Data Exfiltration](https://medium.com/@ultrazartrex/geminis-security-regression-when-old-bugs-come-back-to-haut-df6e51291308)  
  <sub>2025-09 · Google Gemini · ultrazartrex, tuxsharx · critical</sub>
- [Wrap Up: The Month of AI Bugs](https://embracethered.com/blog/posts/2025/wrapping-up-month-of-ai-bugs/)  
  <sub>2025-08 · ChatGPT · Johann Rehberger</sub>
- [Prompt Injection via GitHub Patch in Brave AI Chat (Leo)](https://hackerone.com/reports/3086301)  
  <sub>2025-08 · brave · stellersjay · high</sub>
- [Google Jules Is Vulnerable To Invisible Prompt Injection (Unicode Tag Characters)](https://embracethered.com/blog/posts/2025/google-jules-invisible-prompt-injection/)  
  <sub>2025-08 · Google Jules · Johann Rehberger</sub>
- [GitHub Copilot: Remote Code Execution via Prompt Injection (CVE-2025-53773)](https://embracethered.com/blog/posts/2025/github-copilot-remote-code-execution-via-prompt-injection/)  
  <sub>2025-08 · GitHub Copilot · Johann Rehberger</sub>
- [ZombAI: Prompt Injection to Remote Code Execution in OpenHands (All Hands AI)](https://embracethered.com/blog/posts/2025/openhands-remote-code-execution-zombai/)  
  <sub>2025-08 · OpenHands · Johann Rehberger</sub>
- [OpenHands and the Lethal Trifecta: How Prompt Injection Can Leak Access Tokens](https://embracethered.com/blog/posts/2025/openhands-the-lethal-trifecta-strikes-again/)  
  <sub>2025-08 · OpenHands · Johann Rehberger · high</sub>
- [Exfiltrating Your ChatGPT Chat History and Memories With Prompt Injection](https://embracethered.com/blog/posts/2025/chatgpt-chat-history-data-exfiltration/)  
  <sub>2025-08 · OpenAI · Johann Rehberger</sub>
- [Cline: Vulnerable To Data Exfiltration And How To Protect Your Data](https://embracethered.com/blog/posts/2025/cline-vulnerable-to-data-exfiltration/)  
  <sub>2025-08 · Cline · Johann Rehberger</sub>
- [Amazon Q Developer for VS Code Vulnerable to Invisible Prompt Injection](https://embracethered.com/blog/posts/2025/amazon-q-developer-interprets-hidden-instructions/)  
  <sub>2025-08 · Amazon Q Developer · Johann Rehberger</sub>
- [PROMISQROUTE: GPT-5 AI Router Jailbreak via Model Downgrade](https://adversa.ai/blog/promisqroute-gpt-5-ai-router-novel-vulnerability-class/)  
  <sub>2025-08 · OpenAI · Alex Polyakov, Adversa AI</sub>
- [How Devin AI Can Leak Your Secrets via Multiple Means](https://embracethered.com/blog/posts/2025/devin-can-leak-your-secrets/)  
  <sub>2025-08 · Devin · Johann Rehberger</sub>
- [Amp Code: Arbitrary Command Execution via Prompt Injection (Config File Self-Modification)](https://embracethered.com/blog/posts/2025/amp-agents-that-modify-system-configuration-and-escape/)  
  <sub>2025-08 · Amp · Johann Rehberger</sub>
- [Turning ChatGPT Codex Into A ZombAI Agent (Prompt Injection + Network Allowlist Bypass)](https://embracethered.com/blog/posts/2025/chatgpt-codex-remote-control-zombai/)  
  <sub>2025-08 · OpenAI ChatGPT Codex · Johann Rehberger</sub>
- [Hijacking Windsurf: How Prompt Injection Leaks Developer Secrets](https://embracethered.com/blog/posts/2025/windsurf-data-exfiltration-vulnerabilities/)  
  <sub>2025-08 · Windsurf · Johann Rehberger · high</sub>
- [Google Jules Vulnerable to Multiple Data Exfiltration Issues](https://embracethered.com/blog/posts/2025/google-jules-vulnerable-to-data-exfiltration-issues/)  
  <sub>2025-08 · Google · Johann Rehberger</sub>
- [Windsurf: Memory-Persistent Data Exfiltration (SpAIware Exploit)](https://embracethered.com/blog/posts/2025/windsurf-spaiware-exploit-persistent-prompt-injection/)  
  <sub>2025-08 · Windsurf · Johann Rehberger · high</sub>
- [Amazon Q Developer: Secrets Leaked via DNS and Prompt Injection](https://embracethered.com/blog/posts/2025/amazon-q-developer-data-exfil-via-dns/)  
  <sub>2025-08 · Amazon Q Developer · Johann Rehberger · high</sub>
- [Amazon Q Developer: Remote Code Execution with Prompt Injection](https://embracethered.com/blog/posts/2025/amazon-q-developer-remote-code-execution/)  
  <sub>2025-08 · Amazon Q Developer · Johann Rehberger · critical</sub>
- [I Spent $500 To Test Devin AI For Prompt Injection So That You Don't Have To](https://embracethered.com/blog/posts/2025/devin-i-spent-usd500-to-hack-devin/)  
  <sub>2025-08 · Cognition · Johann Rehberger</sub>
- [AI Kill Chain in Action: Devin AI Exposes Ports to the Internet with Prompt Injection](https://embracethered.com/blog/posts/2025/devin-ai-kill-chain-exposing-ports/)  
  <sub>2025-07 · Cognition · Johann Rehberger</sub>
- [Cursor IDE: Arbitrary Data Exfiltration Via Mermaid (CVE-2025-54132)](https://embracethered.com/blog/posts/2025/cursor-data-exfiltration-with-mermaid/)  
  <sub>2025-07 · Cursor · Johann Rehberger</sub>
- [Phishing for Gemini: Hidden HTML Prompt Injection in Gmail Summaries](https://0din.ai/blog/phishing-for-gemini)  
  <sub>2025-07 · Google Gemini · medium</sub>
- [How Prompt Injection Exposes Manus' VS Code Server to the Internet](https://embracethered.com/blog/posts/2025/manus-ai-kill-chain-expose-port-vs-code-server-on-internet/)  
  <sub>2025-07 · Manus · Johann Rehberger</sub>
- [LLMs in Applications: Understanding and Scoping Attack Surface](https://blog.includesecurity.com/2025/07/llms-in-applications-understanding-and-scoping-attack-surface/)  
  <sub>2025-07 · Mark Kornfeld</sub>
- [HackerNotes Ep. 127: PDF-as-JS Polyglot, OBS WebSocket RCE, and EchoLeak Prompt-Injection Exfil](https://blog.criticalthinkingpodcast.io/p/hackernotes-ep-127-drama-pdf-as-js-chaos-bounty-profile-apps-and-more)  
  <sub>2025-06 · OBS Studio · XSSDoctor, Jorian Woltjer, Aim Labs, assetnote, gr3pme</sub>
- [HackerNotes Ep. 126: Vulnus Ex Machina Part 3 - AI Prompt Injection Bug Chains and Invisible Injection Techniques](https://blog.criticalthinkingpodcast.io/p/hackernotes-ep-126-vulnus-ex-machina-part-3)  
  <sub>2025-06 · Google · Rez0, Johann</sub>
- [Data Exfiltration via Image Rendering Fixed in Amp Code](https://embracethered.com/blog/posts/2025/amp-code-fixed-data-exfiltration-via-images/)  
  <sub>2025-06 · Sourcegraph · Johann Rehberger</sub>
- [Jules Zombie Agent: From Prompt Injection to Remote Control](https://embracethered.com/blog/posts/2025/google-jules-remote-code-execution-zombai/)  
  <sub>2025-06 · Google Jules · Johann Rehberger</sub>
- [Preventing Prompt Injection Attacks at Scale](https://mazinahmed.net/blog/preventing-prompt-injection-attacks-at-scale/)  
  <sub>2025-06 · GitHub · Mazin Ahmed</sub>
- [Claude Code: Data Exfiltration with DNS (CVE-2025-55284)](https://embracethered.com/blog/posts/2025/claude-code-exfiltration-via-dns-requests/)  
  <sub>2025-06 · Anthropic · Johann Rehberger · high</sub>
- [(HackerNotes Ep. 124) Balancing Bug Bounty Freedom with Hacking Time](https://blog.criticalthinkingpodcast.io/p/hackernotes-ep-124-balancing-bug-bounty-freedom-with-hacking-time)  
  <sub>2025-06 · Supabase · Justin Rhinehart (sshell_), Jorian (J0R1AN), lefthanddraft, Yujilik</sub>
- [Amp Code: Invisible Prompt Injection Fixed by Sourcegraph](https://embracethered.com/blog/posts/2025/amp-code-fixed-invisible-prompt-injection/)  
  <sub>2025-06 · Sourcegraph · Johann Rehberger</sub>
- [Security Advisory: Anthropic's Slack MCP Server Vulnerable to Data Exfiltration](https://embracethered.com/blog/posts/2025/security-advisory-anthropic-slack-mcp-server-data-leakage/)  
  <sub>2025-06 · Anthropic · Johann Rehberger · high</sub>
- [Windsurf MCP Integration: Missing Security Controls Put Users at Risk](https://embracethered.com/blog/posts/2025/windsurf-dangers-lack-of-security-controls-for-mcp-server-tool-invocation/)  
  <sub>2025-06 · Windsurf · Johann Rehberger</sub>
- [Sneaking Invisible Instructions for Prompt Injection in Windsurf](https://embracethered.com/blog/posts/2025/windsurf-sneaking-invisible-instructions-for-prompt-injection/)  
  <sub>2025-06 · Windsurf · Johann Rehberger</sub>
- [Toxic Agent Flow in GitHub MCP Server: Prompt Injection via Public Issue Leaks Private Repo Data](https://invariantlabs.ai/blog/mcp-github-vulnerability)  
  <sub>2025-05 · GitHub MCP Server · Marco MilantaLuca Beurer-Kellner · critical</sub>
- [HackerNotes Ep. 123 - Vulnus Ex Machina: AI Hacking Part 2 (Prompt Injection Masterclass)](https://blog.criticalthinkingpodcast.io/p/hackernotes-ep-123-vulnus-ex-machina-ai-hacking-part-2)  
  <sub>2025-05 · gr3pme</sub>
- [AI ClickFix: Hijacking Computer-Use Agents Using ClickFix](https://embracethered.com/blog/posts/2025/ai-clickfix-ttp-claude/)  
  <sub>2025-05 · Anthropic Claude · Johann Rehberger</sub>
- [Bedrock Guardrails Evasion with Prompt Formatting](https://hackerone.com/reports/3056937)  
  <sub>2025-05 · aws_vdp · nkirk-nrlabs · info</sub>
- [How ChatGPT Remembers You: A Deep Dive into Its Memory and Chat History Features](https://embracethered.com/blog/posts/2025/chatgpt-how-does-chat-history-memory-preferences-work/)  
  <sub>2025-05 · ChatGPT · Johann Rehberger, wunderwuzzi</sub>
- [GitHub Copilot Custom Instructions and Risks (Prompt Injection via copilot-instructions.md)](https://embracethered.com/blog/posts/2025/github-custom-copilot-instructions/)  
  <sub>2025-05 · GitHub Copilot · Johann Rehberger</sub>
- [MCP: Untrusted Servers and Confused Clients, Plus a Sneaky Exploit](https://embracethered.com/blog/posts/2025/model-context-protocol-security-risks-and-exploits/)  
  <sub>2025-04 · Anthropic Claude · Johann Rehberger</sub>
- [HackerNotes Ep. 118: Next.js Middleware Bypass, React Router/Remix Host-Header Cache Poisoning, Halo ITSM Pre-Auth SQLi, and IoT Smart-Scale Takeover](https://blog.criticalthinkingpodcast.io/p/hackernotes-ep-118-hacking-happy-hour-0days-on-tap-and-sqli-shots)  
  <sub>2025-04 · Next.js · gr3pme, infosec_au, Rachid Allam (Zhero), spaceraccoon, Rhynorater, Joseph Thacker (Rez0), Johan Carlsson (joaxcar), Searchlight Cyber / AssetNote team · critical</sub>
- [We Hacked Gemini's Source Code (Google LLM bugSWAT)](https://www.landh.tech/blog/20250327-we-hacked-gemini-source-code)  
  <sub>2025-03 · Google · Roni "Lupin" Carta, Justin "Rhynorater" Gardner</sub>
- [Full Customer DB Dump via Prompt Injection in ServiceNow AI Agent Chatbot](https://fdzdev.medium.com/full-customer-db-dump-in-service-now-and-they-called-it-medium-risk-what-a-joke-b9b31cd48172)  
  <sub>2025-02 · ServiceNow · fdzdev · high</sub>
- [How to Hack AI Apps: A Comprehensive Guide to AI Application Security Testing](https://josephthacker.com/hacking/2025/02/25/how-to-hack-ai-apps.html)  
  <sub>2025-02 · Joseph Thacker (rez0)</sub>
- [Invitation Is All You Need: Targeted Promptware Attacks Against Gemini-Powered Assistants](https://sites.google.com/view/invitation-is-all-you-need)  
  <sub>2025-02 · Google Gemini · Ben Nassi, Stav Cohen, Or Yair · critical</sub>
- [ChatGPT Operator: Prompt Injection Exploits & Defenses](https://embracethered.com/blog/posts/2025/chatgpt-operator-prompt-injection-exploits/)  
  <sub>2025-02 · OpenAI · Johann Rehberger</sub>
- [DeepSeek AI Response Filtering Bypass via Base64 Encoding Request](https://1-day.medium.com/uncovering-deepseek-ais-hidden-flaw-a-dive-into-its-response-filtering-system-96203b727192)  
  <sub>2025-01 · DeepSeek</sub>
- [Google Gemini: Unicode SPUA-B Characters Rendered as Visible Hidden Instructions](https://infosecwriteups.com/google-unicode-spua-b-misinterpretation-decoding-hidden-instructions-as-plain-text-114c159ebe8b)  
  <sub>2025-01 · Google · Aditya Sunny</sub>
- [Sneaky Bits: Advanced Data Smuggling Techniques (ASCII Smuggler Updates)](https://embracethered.com/blog/posts/2025/sneaky-bits-and-ascii-smuggler/)  
  <sub>2025-01 · Microsoft Copilot · Johann Rehberger</sub>
- [AI Domination: Remote Controlling ChatGPT ZombAI Instances via Prompt Injection C2](https://embracethered.com/blog/posts/2025/spaiware-and-chatgpt-command-and-control-via-prompt-injection-zombai/)  
  <sub>2025-01 · OpenAI ChatGPT · Johann Rehberger</sub>
- [Microsoft 365 Copilot Generated Images Accessible Without Authentication](https://embracethered.com/blog/posts/2025/m365-copilot-image-generation-without-authentication/)  
  <sub>2025-01 · Microsoft 365 Copilot · Johann Rehberger</sub>
- [Hacking Gemini's Memory with Prompt Injection and Delayed Tool Invocation](https://embracethered.com/blog/posts/2025/gemini-memory-persistence-prompt-injection/)  
  <sub>2025-01 · Google Gemini · Johann Rehberger, wunderwuzzi · low</sub>
- [How Deep Research Agents Can Leak Your Data (ChatGPT Connectors Cross-Tool Data Spill)](https://embracethered.com/blog/posts/2025/chatgpt-deep-research-connectors-data-spill-and-leaks/)  
  <sub>2025-01 · OpenAI ChatGPT · Johann Rehberger</sub>
- [Should I Install an AI Browser?](https://www.bastionsecurity.co.nz/article/should-i-install-an-ai-browser)  
  <sub>2025-01 · Perplexity Comet · Simon Howard</sub>
- [HackerNotes Ep.103: Getting ANSI about Unicode Normalization](https://blog.criticalthinkingpodcast.io/p/hackernotes-ep-103-getting-ansi-about-unicode-normalization)  
  <sub>2024-12 · Microsoft Windows · Yujilik, Orange Tsai, Johann Rehberger, J0R1AN, GrayDuck, nastystereo</sub>
- [Security ProbLLMs in xAI's Grok: A Deep Dive](https://embracethered.com/blog/posts/2024/security-probllms-in-xai-grok/)  
  <sub>2024-12 · xAI · Johann Rehberger · info</sub>
- [AI Attack Vectors: Prompt Injection, System Prompt Extraction, and Obfuscation Techniques for Hacking Chatbots](https://blog.criticalthinkingpodcast.io/p/hackernotes-ep-101-ai-attack-vectors-ctbb-hijacked-rez0-and-johann)  
  <sub>2024-12 · Microsoft Copilot · Johann Rehberger, Rez0</sub>
- [Hacking KachraCraft: Prompt Injection to SSRF and LFI in a Custom AI 3D-Model Generator](https://www.securityrunners.io/post/hacking-ai-applications)  
  <sub>2024-12 · KachraCraft · Full name Published</sub>
- [Terminal DiLLMa: LLM-Powered Apps Can Hijack Your Terminal Via Prompt Injection (ANSI Escape Codes)](https://embracethered.com/blog/posts/2024/terminal-dillmas-prompt-injection-ansi-sequences/)  
  <sub>2024-12 · OpenAI GPT-4o · Johann Rehberger, Leon Derczynski</sub>
- [Trust No AI: Prompt Injection Along the CIA Security Triad Paper](https://embracethered.com/blog/posts/2024/trust-no-ai-prompt-injection-along-the-cia-security-triad-paper/)  
  <sub>2024-12 · OpenAI · Johann Rehberger</sub>
- [DeepSeek AI: From Prompt Injection To XSS and Account Takeover](https://embracethered.com/blog/posts/2024/deepseek-ai-prompt-injection-to-xss-and-account-takeover/)  
  <sub>2024-11 · DeepSeek · Johann Rehberger</sub>
- [Windows Recall Security](https://www.assured.se/posts/windows-recall-security)  
  <sub>2024-11 · Microsoft</sub>
- [Anatomy of an LLM RCE: Prompt Injection to Python Sandbox Escape in LoLLMs (CVE-2024-6982)](https://www.cyberark.com/resources/all-blog-posts/anatomy-of-an-llm-rce)  
  <sub>2024-10 · LoLLMs · Shaked Reiner</sub>
- [LoLLMs LLM RCE: Python Sandbox Escape via Prompt Injection into Calculate Function](https://www.cyberark.com/resources/threat-research-blog/anatomy-of-an-llm-rce)  
  <sub>2024-10 · LoLLMs · Shaked Reiner</sub>
- [ZombAIs: From Prompt Injection to C2 with Claude Computer Use](https://embracethered.com/blog/posts/2024/claude-computer-use-c2-the-zombais-are-coming/)  
  <sub>2024-10 · Anthropic · Johann Rehberger</sub>
- [Spyware Injection Into Your ChatGPT's Long-Term Memory (SpAIware)](https://embracethered.com/blog/posts/2024/chatgpt-macos-app-persistent-data-exfiltration/)  
  <sub>2024-09 · OpenAI ChatGPT · Johann Rehberger</sub>
- [Microsoft 365 Copilot Prompt Injection via Malicious Documents Leading to Email and MFA Code Exfiltration](https://embracethered.com/blog/posts/2024/m365-copilot-prompt-injection-tool-invocation-and-data-exfil-using-ascii-smuggling)  
  <sub>2024-08 · Microsoft · embracethered</sub>
- [Source Code and data exfiltration via Github Copilot](https://hackerone.com/reports/2383092)  
  <sub>2024-08 · github · astrounder · low</sub>
- [Google Colab AI: Data Leakage Through Image Rendering (Fixed) and Ongoing Prompt Injection Risks](https://embracethered.com/blog/posts/2024/google-colab-image-render-exfil/)  
  <sub>2024-07 · Google Colab · Johann Rehberger, wunderwuzzi</sub>
- [Breaking Instruction Hierarchy in OpenAI's gpt-4o-mini](https://embracethered.com/blog/posts/2024/chatgpt-gpt-4o-mini-instruction-hierarchie-bypasses/)  
  <sub>2024-07 · OpenAI · Johann Rehberger</sub>
- [LLM03: Training Data Poisoning via ASCII decoding](https://hackerone.com/reports/2370955)  
  <sub>2024-05 · security · hacktus · info</sub>
- [ChatGPT: Hacking Memories with Prompt Injection](https://embracethered.com/blog/posts/2024/chatgpt-hacking-memories/)  
  <sub>2024-05 · OpenAI · Johann Rehberger</sub>
- [LLM01: Invisible Prompt Injection](https://hackerone.com/reports/2372363)  
  <sub>2024-05 · security · hacktus · medium</sub>
- [Bobby Tables but with LLM Apps - Google NotebookLM Data Exfiltration](https://embracethered.com/blog/posts/2024/google-notebook-ml-data-exfiltration/)  
  <sub>2024-04 · Google NotebookLM · Johann Rehberger · high</sub>
- [The dangers of AI agents unfurling hyperlinks and what you can do about it](https://embracethered.com/blog/posts/2024/the-dangers-of-unfurling-and-what-you-can-do-about-it/)  
  <sub>2024-04 · Slack · Johann Rehberger</sub>
- [Multiple Vulnerabilities in Google AI Services: LLM bugSWAT Event Findings](https://www.landh.tech/blog/20240304-google-hack-50000)  
  <sub>2024-03 · Google · Joseph Thacker (rez0), Justin Gardner (Rhynorater), Roni Carta (Lupin) · $50000</sub>
- [ASCII Smuggling and Hidden Prompt Instructions](https://embracethered.com/blog/posts/2024/ascii-smuggling-and-hidden-prompt-instructions/)  
  <sub>2024-02 · Johann Rehberger</sub>
- [Improving LLM Security Against Prompt Injection: AppSec Guidance for Pentesters and Developers (Part 2)](https://blog.includesecurity.com/2024/02/improving-llm-security-against-prompt-injection-appsec-guidance-for-pentesters-and-developers-part-2/)  
  <sub>2024-02 · OpenAI · IncludeSec (author not individually named in excerpt)</sub>
- [GitLab CVE: Password Reset Array Injection Leads to Account Takeover](https://blog.criticalthinkingpodcast.io/p/hn-54-white-box-formulas-vulnerable-coding-patterns-h1-bounty-gitlab-cve-ato-llm-attacks)  
  <sub>2024-01 · GitLab · gr3pme · critical</sub>
- [Improving LLM Security Against Prompt Injection: AppSec Guidance for Pentesters and Developers](https://blog.includesecurity.com/2024/01/improving-llm-security-against-prompt-injection-appsec-guidance-for-pentesters-and-developers/)  
  <sub>2024-01 · OpenAI · IncludeSecurity research team</sub>
- [Hidden Prompt Injections with Anthropic Claude (ASCII Smuggling via Unicode Tags)](https://embracethered.com/blog/posts/2024/claude-hidden-prompt-injection-ascii-smuggling/)  
  <sub>2024-01 · Anthropic · Johann Rehberger</sub>
- [Exploring Google Bard's Data Visualization Feature (Code Interpreter)](https://embracethered.com/blog/posts/2024/exploring-google-bard-vm/)  
  <sub>2024-01 · Google Bard · Johann Rehberger</sub>
- [Automatic Tool Invocation when Browsing with ChatGPT - Threats and Mitigations](https://embracethered.com/blog/posts/2024/llm-apps-automatic-tool-invocations/)  
  <sub>2024-01 · OpenAI ChatGPT · Johann Rehberger</sub>
- [ASCII Smuggler Tool: Crafting Invisible Text and Decoding Hidden Codes with Unicode Tags](https://embracethered.com/blog/posts/2024/hiding-and-finding-text-with-unicode-tags/)  
  <sub>2024-01 · OpenAI ChatGPT · Johann Rehberger</sub>
- [Who Am I? Conditional Prompt Injection Attacks with Microsoft Copilot](https://embracethered.com/blog/posts/2024/whoami-conditional-prompt-injection-instructions/)  
  <sub>2024-01 · Microsoft 365 Copilot · Johann Rehberger</sub>
- [Google Gemini: Planting Instructions For Delayed Automatic Tool Invocation](https://embracethered.com/blog/posts/2024/llm-context-pollution-and-delayed-automated-tool-invocation/)  
  <sub>2024-01 · Google Gemini · Johann Rehberger</sub>
- [Malicious ChatGPT Agents: How GPTs Can Quietly Grab Your Data (Demo)](https://embracethered.com/blog/posts/2023/openai-custom-malware-gpt/)  
  <sub>2023-12 · OpenAI · Johann Rehberger</sub>
- [OpenAI Begins Tackling ChatGPT Data Leak Vulnerability (Markdown Image Exfiltration Mitigation Analysis)](https://embracethered.com/blog/posts/2023/openai-data-exfiltration-first-mitigations-implemented/)  
  <sub>2023-12 · OpenAI · Johann Rehberger</sub>
- [Google Vertex AI Generative AI Studio - Data Exfiltration via Markdown Image Injection](https://embracethered.com/blog/posts/2023/google-gcp-generative-ai-studio-data-exfiltration-fixed)  
  <sub>2023-10 · Google Cloud · Johann Rehberger · medium</sub>
- [Ekoparty Talk - Prompt Injections in the Wild](https://embracethered.com/blog/posts/2023/ekoparty-prompt-injection-talk/)  
  <sub>2023-10 · Bing Chat · Johann Rehberger</sub>
- [Microsoft Fixes Data Exfiltration Vulnerability in Azure AI Playground](https://embracethered.com/blog/posts/2023/data-exfiltration-in-azure-openai-playground-fixed/)  
  <sub>2023-09 · Microsoft · Johann Rehberger · medium</sub>
- [Anthropic Claude Data Exfiltration Vulnerability via Markdown Image Injection (Fixed)](https://embracethered.com/blog/posts/2023/anthropic-fixes-claude-data-exfiltration-via-images/)  
  <sub>2023-07 · Anthropic Claude · Johann Rehberger</sub>
- [Image to Prompt Injection with Google Bard](https://embracethered.com/blog/posts/2023/google-bard-image-to-prompt-injection/)  
  <sub>2023-07 · Google Bard · Johann Rehberger</sub>
- [Google Docs AI Features: Vulnerabilities and Risks](https://embracethered.com/blog/posts/2023/google-docs-ai-scam/)  
  <sub>2023-06 · Google · Johann Rehberger</sub>
- [Bing Chat: Data Exfiltration Exploit via Prompt Injection and Markdown Image Rendering](https://embracethered.com/blog/posts/2023/bing-chat-data-exfiltration-poc-and-fix/)  
  <sub>2023-06 · Bing Chat · Johann Rehberger · high</sub>
- [ChatGPT Prompt Manipulation Leaks Other Users' Conversation Data via Cache/Context Confusion](https://medium.com/@yhojann.aguilera/how-chatgpt-exposes-conversations-from-other-users-without-being-considered-a-vulnerability-59cd9cfad28e?source=rss------bug_bounty-5)  
  <sub>2023-05 · OpenAI · Yhojann Aguilera</sub>
- [ChatGPT Plugin Exploit Explained: From Prompt Injection to Accessing Private Data (Cross Plugin Request Forgery)](https://embracethered.com/blog/posts/2023/chatgpt-cross-plugin-request-forgery-and-prompt-injection./)  
  <sub>2023-05 · OpenAI ChatGPT · Johann Rehberger</sub>
- [ChatGPT Plugins: Data Exfiltration via Markdown Image Injection & Cross Plugin Request Forgery](https://embracethered.com/blog/posts/2023/chatgpt-webpilot-data-exfil-via-markdown-injection/)  
  <sub>2023-05 · ChatGPT · Johann Rehberger, Roman Samoilenko</sub>
- [Inject My PDF: Prompt Injection for AI Resume Screening](https://kai-greshake.de/posts/inject-my-pdf/)  
  <sub>2023-05 · Microsoft Bing/Edge (GPT-4) · Kai Greshake</sub>
- [Prompt Injection via Error Messages in Self-Healing LLM Code (Wolverine)](https://gynvael.coldwind.pl/?id=766)  
  <sub>2023-04 · OpenAI ChatGPT · gynvael</sub>
- [AI Injections: Threats to Chatbots When Context Matters (LLM Output Data Exfiltration via Hyperlinks)](https://embracethered.com/blog/posts/2023/ai-injections-threats-context-matters/)  
  <sub>2023-04 · Discord · Johann Rehberger</sub>
- [Bing Chat claims to have robbed a bank and it left no trace](https://embracethered.com/blog/posts/2023/bing-chat-bank-robbery/)  
  <sub>2023-01 · Microsoft Bing Chat · Johann Rehberger</sub>
- [Video: Data Exfiltration Vulnerabilities in LLM apps (Bing Chat, ChatGPT, Claude)](https://embracethered.com/blog/posts/2023/video-data-exfiltration-vulns-in-llm-applictions/)  
  <sub>2023-01 · Microsoft Bing Chat · Johann Rehberger · high</sub>
- [Plugin Vulnerabilities: Visit a Website and Have Your Source Code Stolen (ChatGPT "Chat with Code" Plugin)](https://embracethered.com/blog/posts/2023/chatgpt-plugin-vulns-chat-with-code/)  
  <sub>2023-01 · OpenAI · Johann Rehberger</sub>
- [ChatGPT Custom Instructions: Persistent Data Exfiltration Demo](https://embracethered.com/blog/posts/2023/chatgpt-custom-instruction-post-exploitation-data-exfiltration/)  
  <sub>2023-01 · OpenAI · Johann Rehberger, wunderwuzzi</sub>
- [Adversarial Prompting: Tutorial and Lab](https://embracethered.com/blog/posts/2023/adversarial-prompting-tutorial-and-lab/)  
  <sub>2023-01 · Johann Rehberger</sub>
- [Data Exfiltration via Markdown Hyperlink Rendering in Amazon Q for Business](https://embracethered.com/blog/posts/2024/aws-amazon-q-fixes-markdown-rendering-vulnerability)  
  <sub>Amazon Q</sub>
- [ChatGPT Custom Instructions Stored Prompt Injection for Data Exfiltration](https://www.imperva.com/blog/from-chatbot-to-spybot-chatgpt-post-exploitation)  
  <sub>ChatGPT</sub>
- [Unmasking Harmful Content in a Medical Chatbot: A Red Team Perspective](https://www.synack.com/blog/unmasking-harmful-content-in-a-medical-chatbot-a-red-team-perspective)  
  <sub>William Wallace (phyr3wall)</sub>
- [LLM Pentest Agent: Prompt Leaking to Remote Code Execution via Code Injection](https://www.blazeinfosec.com/post/llm-pentest-agent-hacking)  
  <sub>Pedro Henrique Lima</sub>
- [GitHub Copilot Chat Prompt Injection to Data Exfiltration](https://embracethered.com/blog/posts/2024/github-copilot-chat-prompt-injection-data-exfiltration)  
  <sub>GitHub Copilot · high</sub>
- [Hacking Google Bard - From Prompt Injection to Data Exfiltration](https://embracethered.com/blog/posts/2023/google-bard-data-exfiltration)  
  <sub>Google Bard · Joseph Thacker, Kai Greshake</sub>
- [Google AI Studio LLM-Powered Data Exfiltration via Prompt Injection](https://embracethered.com/blog/posts/2024/google-ai-studio-data-exfiltration-now-fixed)  
  <sub>Google · embracethered</sub>
- [Google AI Studio Data Exfiltration via Prompt Injection](https://embracethered.com/blog/posts/2024/google-aistudio-mass-data-exfil)  
  <sub>Google</sub>
- [Integrated Prompt Injection Code Execution in Vanna.AI (CVE-2024-5565)](https://jfrog.com/blog/prompt-injection-attack-code-execution-in-vanna-ai-cve-2024-5565)  
  <sub>Vanna.AI · JFrog Security Research Team, Tong Liu</sub>
- [Persistent Denial of Service in ChatGPT via Prompt Injection and Memory Attacks](https://embracethered.com/blog/posts/2024/chatgpt-persistent-denial-of-service)  
  <sub>ChatGPT</sub>

## MCP and agent tooling

Model Context Protocol servers and clients, coding-agent permission models, skill and plugin marketplaces: tool poisoning, OAuth handling, sandbox escapes.

- [Microsoft Copilot Cowork Skills Bypass Admin-Level DeepSeek/Mistral Model Blocks](https://www.promptarmor.com/resources/skill-accesses-deepseek-despite-copilot-cowork-admin-opt-out)  
  <sub>2026-07 · Microsoft Copilot Cowork · PromptArmor</sub>
- [Claude Dynamic Workflows Use Incorrect Permissions - Subagent Privilege Escalation](https://www.promptarmor.com/resources/claude-dynamic-workflows-use-incorrect-permissions)  
  <sub>2026-06 · Claude Code · PromptArmor</sub>
- [A First Measurement Study on Authentication Security in Real-World Remote MCP Servers](https://arxiv.org/abs/2605.22333)  
  <sub>2026-05 · Zhou, Huijun, Zhang, Xiaohan, Haozhe, Haoyang, Yang, Min</sub>
- [Claude Code RCE via Deeplink Handler Settings Injection](https://0day.click/recipe/2026-05-12-cc-rce/)  
  <sub>2026-05 · Claude Code · joernchen</sub>
- [Full Account Takeover on an MCP OAuth Proxy via Unvalidated redirect_uri (PKCE Self-Attack)](https://hackt.us/full-account-takeover-on-an-mcp-oauth-proxy-why-pkce-can-t-save-you)  
  <sub>2026-04 · Hacktus</sub>
- [OAuth 2.1, MCP Authorization Security, and the Framework CVEs You Should Know](https://blog.criticalthinkingpodcast.io/p/hackernotes-ep-169-oauth-2-1-mcp-authorization-security-and-the-framework-cves-you-should-know)  
  <sub>2026-04 · Django-allauth · Aituglo, Brandyn</sub>
- [Full Read SSRF via OAuth Dynamic Client Registration Open Redirect + Path Normalization](https://eib.hashnode.dev/crafting-a-full-read-ssrf-a-journey-through-oauth-dcr-open-url-redirects-and-path-normalization)  
  <sub>2026-04 · Eib · high</sub>
- [AI Playground XSS to steal user-chat messages and access to connected MCP Server](https://hackerone.com/reports/3424998)  
  <sub>2026-02 · cloudflare · matured_kazama · low</sub>
- [OpenAI Codex CLI: Malicious config.toml Files Enable Arbitrary Code Execution via Misleading Trust Dialog](https://www.promptarmor.com/resources/openai-codex-psa-on-malicious-config-files)  
  <sub>2026-02 · OpenAI · PromptArmor</sub>
- [Shaking the MCP Tree: Exploiting Open Dynamic Client Registration in MCP/OAuth Servers](https://blog.voorivex.team/shaking-the-mcp-tree)  
  <sub>2026-02 · amirmsafari</sub>
- [One-Click RCE in OpenClaw (Moltbot) Gateway via CSRF Token Leak over WebSocket](https://ethiack.com/news/blog/one-click-rce-moltbot)  
  <sub>2026-01 · OpenClaw · Henrique Branquinho, Bruno Mendes, André Baptista · critical</sub>
- [Second-Order XSS via javascript protocol in MCP Server Portal Apps leads to ATO](https://hackerone.com/reports/3316910)  
  <sub>2025-12 · cloudflare · matured_kazama · low</sub>
- [MCP Server Integration Bypasses Tenant Permissions to Leak All Conversations and Contacts](https://1-day.medium.com/how-i-discovered-a-rare-vulnerability-in-mcp-server-bug-bounty-28a0ef643902)  
  <sub>2025-11 · Bugcrowd customer (redacted) · 1-day (Medium handle)</sub>
- [From Well-Known to Well-Pwned: MCP Client OAuth Authorization URL Handling Leads to RCE, LFE, and XSS](https://www.obsidiansecurity.com/blog/from-well-known-to-well-pwned-common-vulnerabilities-in-ai-agents)  
  <sub>2025-11 · Cherry Studio · Obsidian Security · critical</sub>
- [DNS Rebinding SSRF in Burp Suite MCP Server Enables Internal Network Access via send_http1_request Tool](https://hackerone.com/reports/3176157)  
  <sub>2025-10 · portswigger · farmer · info · $2000</sub>
- [`use-mcp`'s oauth2 process uses a window.open call with untrusted mcp server provided data allowing for code execution under the page using it](https://hackerone.com/reports/3211031)  
  <sub>2025-09 · cloudflare · null_smashmaster0045 · medium · $550</sub>
- [From MCP to Shell: Unvalidated OAuth Redirect URLs in MCP Clients Lead to XSS and RCE (Claude Code, Gemini CLI, MCP Inspector, use-mcp)](https://verialabs.com/blog/from-mcp-to-shell/)  
  <sub>2025-09 · Cloudflare · Veria Labs</sub>
- [MCP: May Cause Pwnage - Backdoors in Disguise](https://blog.jaisal.dev/articles/mcp)  
  <sub>2025-04 · Model Context Protocol · AtomicByte, Jaisal, Jorian Woltjer</sub>
- [Anthropic Filesystem MCP Server: Directory Access Bypass via Improper Path Validation](https://embracethered.com/blog/posts/2025/anthropic-filesystem-mcp-server-bypass/)  
  <sub>2025-01 · Anthropic · Johann Rehberger, Elad Beber</sub>

## AI platform and infrastructure

Bugs in the stack the agents run on: inference servers, gateways, model registries, orchestration frameworks, notebook and playground surfaces.

- [Autonomous AI Intrusions Are Here: Lessons from the Hugging Face Compromise](https://embracethered.com/blog/posts/2026/ai-intrusion-are-now-real/)  
  <sub>2026-08 · Hugging Face · Johann Rehberger</sub>
- [LLM Heist: Hijacking LiteLLM for Traffic Interception, Key Theft, and Tool-Call Injection](https://embracethered.com/blog/posts/2026/hijacking-litellm-for-fun-and-profit/)  
  <sub>2026-08 · LiteLLM · Johann Rehberger</sub>
- [Pre-Auth RCE in Bisheng LLM DevOps Platform via Unauthenticated exec()-Based Code Validator](https://medium.com/@cihananthony/how-a-single-copied-function-gave-me-pre-auth-rce-in-an-llm-devops-platform-and-what-happened-47fa7714e10d)  
  <sub>2026-06 · Bisheng · Anthony Cihan, cihananthony · critical</sub>
- [Gemini Live in Chrome: Extension-Based Privilege Escalation via declarativeNetRequest (CVE-2026-0628)](https://unit42.paloaltonetworks.com/gemini-live-in-chrome-hijacking)  
  <sub>2026-03 · Google Chrome · Unit 42 · high</sub>
- [Cache Me, Catch You: Cache-Related Security Threats in LLM Serving Frameworks](https://www.ndss-symposium.org/ndss-paper/cache-me-catch-you-cache-related-security-threats-in-llm-serving-frameworks/)  
  <sub>2026-02 · vLLM · XiangFan Wu, Lingyun Ying, Guoqiang Chen, Yacong Gu, Haipeng Qu</sub>
- [Achieving remote code execution in LangSmith Playground using unsafe template formatting](https://lab.ctbb.show/research/langsmith-unsafe-formatting-to-rce)  
  <sub>2025-12 · LangChain · 0xn3va</sub>
- [Cache Me, Catch You: Cache-Related Security Threats in LLM Serving Frameworks (NDSS 2026)](https://github.com/XingTuLab/Cache_Me_Catch_You)  
  <sub>2025-12 · vLLM · XiangFan Wu, Lingyun Ying, Guoqiang Chen, Yacong Gu, Haipeng Qu</sub>
- [Hacking Gemini: A Multi-Layered Approach to Bypassing Markdown Sanitization for Data Exfiltration](https://buganizer.cc/hacking-gemini-a-multi-layered-approach-md)  
  <sub>2025-11 · Google Gemini · Valentino Massaro</sub>
- [NVIDIA Triton Inference Server: Info Leak to RCE via Python Backend Shared Memory](https://www.wiz.io/blog/nvidia-triton-cve-2025-23319-vuln-chain-to-ai-server)  
  <sub>2025-08 · NVIDIA · Ronen Shustin, Nir Ohfeld, Sagi Tzadik, Hillai Ben-Sasson, Andres Riancho, Yuval Avrahami · critical</sub>
- [Code Injection in Google Vertex AI "Get Code" via Unescaped Image URI (fileUri)](https://blog.3133700.xyz/bug_vertex_ai)  
  <sub>2025-07 · Google · 3133700 (blog author, handle from blog.3133700.xyz) · $3133</sub>
- [A look at Cloudflare's AI-coded OAuth library](https://neilmadden.blog/2025/06/06/a-look-at-cloudflares-ai-coded-oauth-library/)  
  <sub>2025-06 · Cloudflare · Neil Madden</sub>
- [PAT-tastrophe: How We Hacked Virtuals' $4.6B Agentic AI & Cryptocurrency Ecosystem](https://medium.com/@gonzo-hacks/pat-tastrophe-how-we-hacked-virtuals-4-6b-agentic-ai-cryptocurrency-ecosystem-f850b544d0f5)  
  <sub>2025-03 · Virtuals Protocol · gonzo-hacks, Shlomie, toormund, nitepointer · high · $10000</sub>
- [Unauthenticated RCE in Langflow via /api/v1/validate/code (CVE-2025-3248)](https://m1s0-0.github.io/writeups/posts/langflow-rce-cve-2025-3248.html)  
  <sub>2025-01 · Langflow · m1s0-0 · critical</sub>
- [Protect Your Copilots: Preventing Data Leaks in Copilot Studio](https://embracethered.com/blog/posts/2024/copilot-studio-protect-your-copilots/)  
  <sub>2024-07 · Microsoft Copilot Studio · Johann Rehberger · low</sub>
- [Probllama: Remote Code Execution in Ollama via Path Traversal in Model Manifest Digest](https://www.wiz.io/blog/probllama-ollama-vulnerability-cve-2024-37032)  
  <sub>2024-06 · Ollama · Wiz Research · critical</sub>
- [Critical OAuth and Authentication Vulnerabilities in ChatGPT Plugins Enable Account Takeover and Malicious Plugin Installation](https://salt.security/blog/security-flaws-within-chatgpt-extensions-allowed-access-to-accounts-on-third-party-websites-and-sensitive-data)  
  <sub>2024-03 · OpenAI · critical</sub>
- [ChatGPT: Lack of Isolation between Code Interpreter sessions of GPTs](https://embracethered.com/blog/posts/2024/lack-of-isolation-gpts-code-interpreter/)  
  <sub>2024-02 · OpenAI · Johann Rehberger</sub>
- [Remote Code Execution and Arbitrary Memory Write in NVIDIA Triton Inference Server](https://sites.google.com/site/zhiniangpeng/blogs/Triton-RCE)  
  <sub>NVIDIA · Lawliet, Zhiniang Peng</sub>
- [SSRF in Microsoft Copilot Studio via HttpRequestAction with Multiline Header Injection Bypass](https://www.tenable.com/blog/ssrfing-the-web-with-the-help-of-copilot-studio)  
  <sub>Microsoft Copilot Studio · Tenable Research · critical</sub>
- [Wiz Research: Cross-Tenant Container Escape and Deserialization RCE in Hugging Face AI Platform](https://www.wiz.io/blog/wiz-and-hugging-face-address-risks-to-ai-infrastructure)  
  <sub>Hugging Face · Sagi Tzadik, Shir Tamari, Nir Ohfeld, Ronen Shustin, Hillai Ben-Sasson · critical</sub>

## AI product surfaces (classic web bugs)

Ordinary web vulnerabilities found in AI features: XSS in chat widgets, IDOR on conversation objects, business-logic flaws in assistant billing and gating.

- [The Token That Wouldn't Die: AI Access Token Never Revoked on Regeneration](https://medium.com/@krypto.sec/the-token-that-wouldnt-die-43d3c65f22e0)  
  <sub>2026-07 · Krypto · high</sub>
- [IDOR in AI Chatbot Action Confirmation Leads to Unauthorized Product Modification (ShopFire)](https://medium.com/@mahdisalhi0500/this-bug-take-to-me-4-days-to-understand-how-is-work-34892d63b113)  
  <sub>2025-12 · ShopFire · mahdisalhi0500</sub>
- [SSTI in AI Model via WhatsApp Profile Name Injection](https://jeetpal2007.medium.com/how-i-found-ssti-into-an-ai-model-due-to-unsafe-argument-4a44cadcd985)  
  <sub>2025-11 · Jeetpal</sub>
- [ChatGPT Shared Conversations Indexed by Google - Privacy Loophole](https://medium.com/@letchupkt/how-i-reported-a-major-privacy-loophole-in-chatgpts-sharing-feature-6bc4225d81b5)  
  <sub>2025-08 · OpenAI · Lakshmikanthan K, letchupkt</sub>
- [How I Find Vulnerability Can Make X (Twitter) Lose Millions of Dollars](https://l4zyhacker.medium.com/how-i-find-vulnerability-can-make-x-twitter-lose-millions-of-dollars-ae34d713254f)  
  <sub>2025-07 · X · l4zyhacker</sub>
- [Chaining HTML Injection, Stored XSS, CSRF, Unrestricted File Upload and Session Persistence in a Chatbot Widget](https://medium.com/@tusharpuri6/peeling-back-the-layers-exploring-critical-security-flaws-in-chatbot-systems-940e14d62ac6)  
  <sub>2024-10 · Tushar Puri · critical</sub>
- [Remote Code Execution in AI Chatbot Custom Workflow Code Snippet Feature](https://varmaanu001.medium.com/unveiling-remote-code-execution-in-ai-chatbot-workflows-3c7f633f63c3)  
  <sub>2024-08 · Anurag Verma · critical</sub>
- [Reflected XSS in chatbot](https://hackerone.com/reports/1735622)  
  <sub>2022-11 · mtn_group · roland_hack · medium</sub>
- [Command Injection / RCE in a Custom-Built Slack Bot via Unsanitized Message Text](https://medium.com/swlh/hacking-a-slackbot-that-i-made-27aaed9d276b)  
  <sub>2021-02 · N0ur5</sub>
- [Chatbot Security: Exposed .git Repository and Public S3 Bucket Leak Healthcare and Financial Data](https://medium.com/@secxena/chatbot-security-framework-everything-you-need-to-know-about-chatbot-security-243468f977b6)  
  <sub>2019-07 · secxena</sub>
- [AI Chatbot Authentication Bypass Leading to Database Dumping via SQL Execution](https://www.synack.com/blog/dumping-a-database-with-an-ai-chatbot)  
  <sub>Kuldeep Pandya</sub>
- [Business Logic Flaws in AI Assistant Feature (Premium Bypass)](https://medium.com/@mahmoudelsadany51/business-logic-flaws-in-ai-assistant-feature-5d60ec52db20)  
  <sub>Mahmoudelsadany</sub>
- [HackerOne Copilot: IDOR in DestroyLlmConversation GraphQL Mutation Allows Deleting Any User's Conversation](https://hackerone.com/reports/2218334)  
  <sub>HackerOne</sub>

## Adjacent: AI as the attacker's tool

Not attacks on agents, but agents doing the attacking. Included because the tradecraft overlaps.

- [Hacking Google with AI: Mass-Fuzzing Internal Google APIs via Discovery Documents and First-Party Auth](https://brutecat.com/articles/hacking-google-with-ai/)  
  <sub>2026-06 · Google · brutecat, Michael · critical · $500000</sub>
- [Finding Gadgets Like It's 2026: LLM-Automated Java Deserialization Gadget Chain Discovery](https://www.atredis.com/blog/2026/3/12/findings-gadgets-like-its-2026)  
  <sub>2026-03 · WildFly · Atredis Partners · critical</sub>
- [HackerNotes Ep. 134: XBOW AI Hacking Agent - Account Takeover Chain and AEM/Akamai XXE Case Studies](https://blog.criticalthinkingpodcast.io/p/hackernotes-ep-134-xbow-ai-hacking-agent-and-human-in-the-loop-with-diego-jurado)  
  <sub>2025-08 · Adobe Experience Manager · Diego Jurado</sub>
- [Repeater Strike: an AI-powered Burp Suite extension to amplify manual IDOR testing](https://portswigger.net/research/repeater-strike-manual-testing-amplified)  
  <sub>2025-07 · Gareth Heyes</sub>
- [Hunting .NET Deserialization Vulnerabilities in AddinUtil.exe With Claude via MCP](https://trustedsec.com/blog/hunting-deserialization-vulnerabilities-with-claude)  
  <sub>2025-06 · Microsoft</sub>
- [Document My Pentest: AI-powered Burp Suite extension for automated pentest note-taking](https://portswigger.net/research/document-my-pentest)  
  <sub>2025-04 · Gareth Heyes</sub>
- [Shadow Repeater: AI-Enhanced Manual Testing for Burp Suite](https://portswigger.net/research/shadow-repeater-ai-enhanced-manual-testing)  
  <sub>2025-02 · Gareth Heyes, James Kettle</sub>
- [Hacking HackerOne: Using Computer Vision (YOLOv7) to Find Undisclosed Reports Leaked in Disclosed PoC Videos](https://3bodymo.medium.com/hacking-hackerone-how-computer-vision-helped-uncover-hidden-vulnerabilities-858d03a6a67)  
  <sub>2023-05 · HackerOne · 3bodymo</sub>

- [Down the Rabbit Hole: Unusual Applications of OpenAI in Cybersecurity Tooling](https://spaceraccoon.dev/down-the-rabbit-hole-unusual-applications-of-openai-in-cybersecurity-tooling/)  
  <sub>2021-09 · Spaceraccoon</sub>

## Notes on scope

- Attacks **on** AI systems, not AI safety/alignment research and not model-bias work.
- Podcast and newsletter episode notes are included where the episode covers a specific technique or bug; they are labelled as such in the title.
- `links.txt` holds the same set as bare URLs, one per line, for scripted use.

## License

[CC0 1.0 Universal](LICENSE). The index is dedicated to the public domain: copy it,
fork it, mirror it, no attribution needed.

This covers the index only. Every linked writeup remains the copyright of whoever
wrote it, and nothing here grants any rights over those.
