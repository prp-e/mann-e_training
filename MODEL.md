# Mann-E 4.2 Merged

## Technical Information about the model

* Base Model : [runwayml/stable-diffusion-v1-5](https://huggingface.co/runwayml/stable-diffusion-v1-5)
* Merge : [mann-e/mann-e_4_rev-1-3](https://huggingface.co/mann-e/mann-e_4_rev-1-3)
* Merge amount : %70 fine-tuned SD 1.5 (or _Mann-E version 4.2 base_) and %30 of Mann-E 4.1.3 in order to get the old styles such as _Model Shoot_, _Elden Ring_, _Arcane_, _Analog Style_ and _GTA V Style_. Also this merge can be helpful for _Midjourney version 4_ style artwork as well.

### Training process

The code for pre-processing data and fine-tuning the model is available in [this repository](https://github.com/prp-e/mann-e_training) and you can run it on your own as well.

* Text encoder iterations : 1440 (number of pics times two in order to understand `mstyle` which can give the user a _Midjourney version 5_ vibe).
* Stable Diffusion iterations : 16000 iterations for one epoch
* Time: around 4 hours on a single T4 GPU.