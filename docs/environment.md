# Recorded environment and reproduction notes

The metadata records the following environment for both runs:

| Item | Recorded value |
| --- | --- |
| Runtime | Google Colab on Linux |
| GPU | Tesla T4 |
| Precision | `torch.float16` |
| Python | 3.13.15 |
| PyTorch | 2.11.0+cu130 |
| Transformers | 5.20.1 |
| Accelerate | 1.15.0 |
| Hugging Face Hub | 1.33.0 |
| Model | `Qwen/Qwen2.5-1.5B-Instruct` |
| Model/tokenizer revision | Unknown (`null`) |

The package `requirements.txt` records the non-runtime-specific library versions. The PyTorch CUDA build must match the chosen GPU/runtime; use the appropriate installation instructions for the environment rather than assuming a generic wheel will provide `+cu130`.

For a new run, open `notebooks/01_model_setup.ipynb` in a Colab GPU runtime, verify CUDA, load the model, and run only the relevant case workflow. The notebook saves exact prompts and metadata into a new run directory and refuses ordinary reruns in the same kernel.

Do not rerun the notebook to verify the existing study. This package already includes the completed raw records. A new run may differ because the exact model revision was not recorded and greedy generation can still depend on software and runtime details.
