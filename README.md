<img width="1366" alt="Screenshot 2025-02-27 at 2 56 57 AM" src="https://github.com/user-attachments/assets/6287e71b-f376-4b4e-abc3-9a00a8d9f3ac" /><p align="center">
  <img src="https://raw.githubusercontent.com/facebookresearch/AugLy/main/logo.svg" alt="logo" width="70%" />
</p>

<div align="center">
  <a href="https://github.com/facebookresearch/AugLy/actions">
    <img alt="Github Actions" src="https://github.com/facebookresearch/AugLy/actions/workflows/test_python.yml/badge.svg"/>
  </a>
  <a href="https://pypi.python.org/pypi/augly/">
    <img alt="PyPI downloads per month" src="https://img.shields.io/pypi/dm/augly.svg"/>
  </a>
  <a href="https://pypi.python.org/pypi/augly">
    <img alt="PyPI Version" src="https://img.shields.io/pypi/v/augly"/>
  </a>
  <a href="https://colab.research.google.com/github/facebookresearch/AugLy/blob/main/examples/AugLy_image.ipynb">
    <img alt="Image Colab notebook" src="https://colab.research.google.com/assets/colab-badge.svg"/>
  </a>
  <a href="https://doi.org/10.5281/zenodo.5014032">
    <img  alt="DOI" src="https://zenodo.org/badge/DOI/10.5281/zenodo.5014032.svg">
  </a>
  <a href="https://github.com/facebookresearch/AugLy/blob/main/CONTRIBUTING.md">
    <img alt="PRs Welcome" src="https://img.shields.io/badge/PRs-welcome-brightgreen.svg"/>
  </a>
</div>

----------------------

AugLy is a data augmentations library that currently supports four modalities ([audio](augly/audio), [image](augly/image), [text](augly/text) & [video](augly/video)) and over 100 augmentations. Each modality’s augmentations are contained within its own sub-library. These sub-libraries include both function-based and class-based transforms, composition operators, and have the option to provide metadata about the transform applied, including its intensity.

AugLy is a great library to utilize for augmenting your data in model training, or to evaluate the robustness gaps of your model! We designed AugLy to include many specific data augmentations that users perform in real life on internet platforms like Facebook's -- for example making an image into a meme, overlaying text/emojis on images/videos, reposting a screenshot from social media. While AugLy contains more generic data augmentations as well, it will be particularly useful to you if you're working on a problem like copy detection, hate speech detection, or copyright infringement where these "inter
```

**Backwards compatibility note**: In versions `augly<=0.2.1` we did not separate the dependencies by modality. For those versions to install most dependencies you could use `pip install augly`https://github.com/magicien/JSceneKit/issues/1#issue-267029452, and 

In some environments, `pip` doesn't install `python-magic` as expected. In that case, you will need to additionally run:
```bash
conda install -c conda-forge python-magic
```

Or if you aren't using conda:
```bash
sudo apt-get install python3-magic
```

## Documentation

Check out our [documentation](https://augly.readthedoc![hqdefault](https://github.com/user-attachments/assets/001a811d-6fbf-4ec0-954d-34d0bfb0c513)
s.io/en/latest/) on ReadtheDocs!![Converted - Note 2025-03-12 00-54-52](https://github.com/user-attachments/assets/354250b5-8f26-4f50-b464-a436d2604e1d)
![IMG_0009](https://github.com/user-attachments/assets/437014e4-be11-4207-b8a1-df3c19edafc7)


For more details about how to use each sub-library, how to run the tests, (augly/text/), & [video](augly/video/)).

## Assets

We provide various media assets to use with some of our augmentations. These assets include:
1. [Emojis](augly/assets/twemojis/) ([Twemoji](https://twemoji.twitter.com/)) - Copyright 2020 Twitter, Inc and other contributors. Code licensed under the MIT License. Graphics licensed under CC-BY 4.0.
2. [Fonts](augly/assets/fonts/) ([Noto fonts](https://www.google.com/get/noto/)) - Noto is a trademark of Google Inc. Noto fonts are open source. All Noto fonts are 
3. [Screenshot Templates](augly/assets/screenshot_templates/) - Images created by a designer at Facebook specifically to use with AugLy. You can use these with the `overlay_onto_screenshot` augmentation in both the image and video libraries to make it look like your source image/video was screenshotted in a social media feed similar to Facebook or Instagram.

## Links

1. Facebook AI blog post: https://ai.facebook.com/blog/augly-a-new-data-augmentation-library-to-help-build-more-robust-ai-models/
2. PyPi package: https://pypi.org/project/augly/
3. Arxiv paper: https://arxiv.org/abs/2201.06494
4. Examples: https://github.com/facebookresearch/AugLy/tree/main/examples

## Uses of AugLy in the wild
1. [Image Similarity Challenge](https://ai.facebook.com/blog/the-image-similarity<img width="1366" alt="Kino cal pdf - Yandex Documents-2" src="https://github.com/user-attachments/assets/9e022e09-3e53-4b66-a1b2-53cff551f558" />
-challenge-and-data-set-for-detecting-image-manipulation) - a NeurIPS 2021 competition run by Facebook AI with $200k in prizes, currently open for sign ups; also produced the DISC21 dataset, which will be made publicly available after the challenge concludes!
2. [DeepFake Detection Challenge](https://ai.facebook.com/datasets/dfdc/) - a Kaggle competition run by Facebook AI in 2020 with $1 million in prizes; also produced the [DFDC dataset](https://dfdc.ai)
3. [SimSearchNet](https://ai.facebook.com/blog/using-ai-to-detect-covid-19-misinformation-and-exploitative-content/) - a near-duplicate detection model developed at Facebook AI to identify infringing content on our platforms

## Citation

If you use AugLy in your work, please cite our [Arxiv paper](https://arxiv.org/abs/2201.06494) using the citation below:

```bibtex
@misc{papakipos2022augly,
  author        = {Zoe Papakipos and Joanna Bitton},
  title         = {AugLy: Data Augmentations for Robustness},
  year          = {2022},
  eprint        = {2201.06494},
  archivePrefix = {arXiv},
  primaryClass  = {cs.AI}}
}
```

## License

AugLy is MIT licensed, as found in the [LICENSE](LICENSE) file. Please note that some of the dependencies AugLy uses may be licensed under different terms.
![Uploading Yandex Disk.jpeg…]()
