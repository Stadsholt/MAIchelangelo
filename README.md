# MAIchelangelo - Physical AI Art Generator

### 7th-Semester Mini-Project · Aalborg University

**MAIchelangelo** is an interactive art installation that lets visitors co-create artworks with AI in a physical, room-scale setup. The experience blends tactile interaction, live camera input, and real-time AI-generated image editing to produce personalised art pieces inspired by styles like Michelangelo, Picasso, or Van Gogh.

## Live Transformation

![Gif](https://github.com/user-attachments/assets/3ce3381f-0bc4-4fce-9721-369892279e91)

## Prototype Setup

![Prototype](https://github.com/user-attachments/assets/11a1f089-cd09-44f1-b9de-2cb05c2e2901)

Visitors interact with physical 3D-printed puzzle pieces arranged on a surface. A live camera feed captures the layout, which is then interpreted by an AI model based on a user-provided style instruction. The result is a reimagined artwork generated in real time.

## Art Style Examples

The installation can interpret a variety of art styles based on user instruction:
![Others](https://github.com/user-attachments/assets/bd204646-3d1a-4c27-8273-6a1f58900ec3)

## How does it work?

- **Live camera input** via Gradio
- **Editable instructions** to guide the AI ("make it look like Picasso", "paint it like it’s from the 1500s", etc.)
- **CFG & seed control** for experimentation
- **Automatic resizing & safety disabled** for full creative output

## Tech Stack

- Python
- [Gradio](https://gradio.app) – for interface and webcam input
- [Stable Diffusion InstructPix2Pix](https://huggingface.co/timbrooks/instruct-pix2pix) – AI image-to-image generation
- [Torch](https://pytorch.org/) – GPU acceleration
- [PIL / ImageOps](https://pillow.readthedocs.io/) – image processing
- Webcam + physical 3D-printed interface
- Google Colab (for deployment)
