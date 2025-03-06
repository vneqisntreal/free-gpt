
# FreeGPT - Simplified Access to Free AI Models (Demo/Educational Purposes Only)

## What is FreeGPT?

FreeGPT is a Python module that provides a simplified interface for interacting with various free AI models available online. It essentially acts as a wrapper, turning publicly accessible AI demos and APIs into an easy-to-use Python library that mimics the OpenAI API structure. This allows you to experiment with AI text generation without needing paid API keys or complex setups. **Please note that this project is for educational and demonstrative purposes only.**

## How does FreeGPT work?

FreeGPT connects to websites and services that offer free access to AI models. It then standardizes the input and output format, allowing you to interact with these models using a consistent Python interface. It essentially bridges the gap between different free AI services and a unified programming experience.

## How do you make money?

We don't. This project is currently a hobby/proof-of-concept, created for educational and experimental purposes.

## Current Supported Models:

*   GPT-4o
*   GPT-4o-Mini
*   GPT-3.5 Turbo

**Note:** Model availability depends on the underlying free services. Check the FreeGPT documentation for the most up-to-date list and any specific usage instructions.

## How do I use the module?

```python
# pip3 install freegpt-client

from freegpt_client import Client # Corrected import

openai = Client()

response = openai.chat.completions.create(
    model="gpt-4o",  # or another supported model - check documentation
    messages=[{"role": "user", "content": "Heyo!"}]
)

print(response.choices[0].message.content)
```

**Important Notes:**

*   **Installation:** Make sure to install the correct package name `freegpt-client`.
*   **Model Availability:** The availability and performance of specific models depend entirely on the availability and terms of the underlying free AI services. Check the FreeGPT documentation for the most up-to-date list, their sources, and any specific usage instructions.
*   **Rate Limits & Reliability:** Free AI services often have rate limits and may be unreliable. Expect slower response times and potential service interruptions. FreeGPT cannot guarantee uptime or performance.
*   **Quality & Accuracy:** The quality and accuracy of the generated text depend entirely on the underlying AI models being used. Free models may not be as powerful or reliable as paid options.
*   **Takedown Requests:** If you are a service provider and believe your site should not be included in FreeGPT, please create an issue on the GitHub repository with a detailed explanation. We will review the request and take appropriate action.

## Disclaimer

**Disclaimer:** This project is for educational purposes only. Use at your own risk. The author is not liable for any damages, losses, or legal issues arising from the use of FreeGPT. You are responsible for adhering to the terms of service of all underlying services. Accessing or using certain models may violate their terms or be illegal in your jurisdiction. No warranty is provided. Use for learning, and be aware of potential risks and limitations. Check the terms of underlying services frequently.
