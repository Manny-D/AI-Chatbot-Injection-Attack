# Artificial Intelligence (AI) Chatbots and Injection Attacks

![AI CB](https://github.com/Manny-D/Injection-Attack-AI-Chatbot/assets/99146530/ccc19ce9-229b-4020-9d48-7479b79abb3f)

## Overview

This is from TryHackMe's Advent of Cyber '23 where the following were the learning objectives:
- Natural language processing (NLP), which powers AI chatbots.
- Prompt injection attacks and how they manipulate chatbot responses.
- How to defend against prompt injection attacks.

AI chatbots like ChatGPT are widely used, but they're vulnerable to prompt injection attacks. Prompt injection is akin to social engineering, targeting chatbots to elicit unintended responses. Companies are rapidly adopting AI chatbots, making security critical.

<br>

### Our First Attack:

Prompt injection can extract sensitive info from chatbots. Simply asking the chatbot for sensitive info can sometimes reveal it.

![Van Chatty](https://github.com/Manny-D/Injection-Attack-AI-Chatbot/assets/99146530/492330c9-2b29-47a9-a052-8e10b581071b)

<br>

### Behind the Intelligence:

Chatbots learn from vast datasets, influencing their responses and potentially exposing confidential information. Natural Language Processing (NLP) enables chatbots to understand and respond to human language by predicting the next word based on context. While removing sensitive data from training may seem like a solution, the dynamic nature of information and the complexity of retraining models post-deployment present significant challenges. It is important to understand that chatbot training is very intricate and implementing robust security measures is necessary to protect against vulnerabilities.

<br>

### Prompt-Assisted Security Measures:

Developers can add a system prompt to guide chatbot responses. 

![Van Chatty 2](https://github.com/Manny-D/Injection-Attack-AI-Chatbot/assets/99146530/c0e71887-121c-42f9-a88d-dbedcce4d1ee)

However, system prompts can be bypassed by cleverly phrased questions.

![Van Chatty 3](https://github.com/Manny-D/Injection-Attack-AI-Chatbot/assets/99146530/86f70991-f211-44c2-86b6-cb3ae877c286)

![Van Chatty 4](https://github.com/Manny-D/Injection-Attack-AI-Chatbot/assets/99146530/46835b34-5274-42b4-9f85-66baf401690b)

While we could add more rules to the system prompt, it's impossible to cover every possible way users might query the chatbot. System prompts are guidelines for the chatbot, but these queries may still go beyond these guidelines.

<br>

### AI-Assisted Security Measures:

How can Devs defend against the countless possible attacks? Using another AI to intercept and detect malicious inputs before reaching the chatbot can be a viable way.

![Van Chatty 5](https://github.com/Manny-D/Injection-Attack-AI-Chatbot/assets/99146530/fc534c27-2579-4226-9456-5bb47b21fe0c)

While the Interceptor will need continual training to detect new attack patterns, attackers may find ways around the interceptor by employing creative and out of the box thinking.

![image](https://github.com/Manny-D/Injection-Attack-AI-Chatbot/assets/99146530/1e7bb993-0159-462a-8c2b-ef7c2f9b2ceb)

<br>

## Conclusion

The rapid advancement of AI chatbots, powered by Natural Language Processing (NLP), has revolutionized digital interactions but also introduced vulnerabilities like prompt injection attacks. These attacks can manipulate chatbot responses to extract sensitive information. While security measures like system prompts and AI Interceptors can mitigate these risks, the evolving nature of attacks and chatbot technologies demands ongoing vigilance and adaptation.

<br>

### Related Story

[Tricking a GM chatbot into selling a Chevy Tahoe for $1](https://www.upworthy.com/prankster-tricks-a-gm-dealership-chatbot-to-sell-him-a-76000-chevy-tahoe-for-1-rp)

![$1 Tahoe](https://github.com/Manny-D/AI-Chatbot-Injection-Attack/assets/99146530/4e026a55-99c6-4600-af6f-14371eb3632c)
