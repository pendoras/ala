# Fooocus - Clothes Inpaint Edition

Modified version of Fooocus with SAM-based clothes detection for easy inpainting.

## Quick Start (Google Colab)

```python
# Clone repo
!git clone https://github.com/pendoras/ala.git
%cd ala

# Run with clothes_inpaint preset
!python entry_with_update.py --share --always-high-vram --preset clothes_inpaint
```

> Model akan di-download otomatis saat pertama kali jalan (~7GB)

## Features

### SAM-based Clothes Detection
Uses SAM (Segment Anything Model) + GroundingDINO for text-based detection.

Default detection prompt: `clothes`

Other prompts you can use:
- `shirt` - Upper body clothing
- `dress` - Dresses
- `pants` - Lower body clothing
- `jacket` - Outerwear

## How to Use

1. Run Fooocus with `--preset clothes_inpaint`
2. Upload a photo to Inpaint or Outpaint tab
3. In Detection prompt, type what you want to detect (e.g. `shirt`, `dress`)
4. Click **"Generate mask from image"**
5. White mask area = what will be changed
6. Write your prompt (e.g., "red silk dress", "blue denim jacket")
7. Click **Generate**

## Credits
Based on [Fooocus](https://github.com/lllyasviel/Fooocus) by lllyasviel
