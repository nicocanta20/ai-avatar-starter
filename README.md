# AI Avatar Generator

Generates images of me in any style from a text prompt, like "nicolas as an
astronaut, oil painting". It uses a Stable Diffusion model fine-tuned on my own photos.

Built in January 2023.

## How it works
- Custom Stable Diffusion model (`nicoc/sd-nicolas`) hosted on Hugging Face.
- A Next.js API route calls the Hugging Face Inference API and returns the
  image as base64.
- Handles model cold starts: when Hugging Face responds that the model is still
  loading, the app waits the estimated time and retries (up to 20 times).

## Stack
Next.js 13 · React 18 · Stable Diffusion · Hugging Face Inference API

## Status
Not maintained since 2023.
