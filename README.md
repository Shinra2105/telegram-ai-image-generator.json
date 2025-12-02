**Telegram AI Style Transfer Bot**

**Description: A full-stack interactive bot built on n8n. It demonstrates complex media handling and multi-model AI chaining.**

Workflow Logic:

Ingestion: Receives an image via Telegram Trigger.

Vision Analysis: Uses Google Gemini Vision to generate a detailed biometric description of the user (preserving identity features).

User Interaction: Sends a Telegram Menu (Inline Keyboard) for style selection (Simpson, Lego, Spartan, Stranger Things).

Generation: Chains the Gemini prompt + User Style into Replicate (Stable Diffusion/Flux) to generate the new image.

Delivery: Uploads the result to Dropbox and sends it back to the user on Telegram.
