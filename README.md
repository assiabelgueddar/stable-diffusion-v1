# 🎨 Stable Diffusion: Text-to-Image Generation Notebook

This notebook demonstrates how to generate **photorealistic images from text prompts** using the **Stable Diffusion model**. It leverages the `diffusers` library from Hugging Face and is intended for use on machines equipped with **NVIDIA GPUs (≥10GB VRAM)**.

---

## 🚀 Features

- Generate images from text prompts with high realism
- Customize prompts for different artistic or photographic styles
- Uses the `StableDiffusionPipeline` from Hugging Face
- Compatible with Google Colab, Jupyter Notebook, and VS Code

---

## 📦 Dependencies

Install the required libraries using:

```bash
pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu118
pip install diffusers transformers accelerate safetensors
```

Optional (for performance):
```bash
pip install xformers
```

---

## 📷 Example Prompt

Try this for a photorealistic result:

```text
"A high-resolution photograph of a fluffy cat riding a brown horse in a grassy field, natural lighting, shallow depth of field, 50mm lens, realistic fur and textures, National Geographic style"
```

---

## 🖼️ Output

The generated image is displayed inline using `IPython.display`, and can also be saved using `image.save("filename.png")`.

---

## 🧠 Model Info

- **Base Model**: `CompVis/stable-diffusion-v1-4`
- **Text Encoder**: CLIP ViT-L/14 (frozen)
- **UNet Size**: 860M parameters
- **Trained On**: Subset of [LAION-5B](https://laion.ai/blog/laion-5b/)

---

## 📁 File Structure

```
📦stable-diffusion/
 ┣ 📜 stable-diffusion (1).ipynb   ← Jupyter notebook
 ┗ 📄 README.md                     ← You're here
```

---

## 💡 Tips

- Use detailed prompts with styles like `DSLR`, `ultra realistic`, `natural lighting`, etc.
- Run on GPU-enabled environments for best performance.
- Add `pipe.to("cuda")` to move model to GPU.

---

## 📝 Credits

- Developed using tools by [Hugging Face](https://huggingface.co/CompVis/stable-diffusion-v1-4)
- Based on the original Stable Diffusion research by [CompVis](https://github.com/CompVis), [Stability AI](https://stability.ai/), and [LAION](https://laion.ai/)

---

## 📄 License

This project is for **educational and non-commercial** purposes. Refer to the [CreativeML license](https://huggingface.co/CompVis/stable-diffusion-v1-4#license) for model usage.
