Welcome to Megatron-LLM's documentation!
========================================

.. image:: imgs/llama-falcon.png

This library enables pre-training and fine-tuning of large language models (LLMs) at scale.
Our repository is a modification of the `original Megatron-LM codebase <https://github.com/NVIDIA/Megatron-LM>`_ by Nvidia.

Added key features include:

- `Llama <https://arxiv.org/abs/2302.13971>`_, `Llama 2 <https://arxiv.org/abs/2307.09288>`_ and `Falcon <https://huggingface.co/tiiuae>`_ support.
- Training of large models (70B Llama2, 65B Llama1 and 40B Falcon) on commodity hardware on multiple nodes.
- 3-way parallelism: tensor parallel, pipeline parallel and data parallel training (inherited from Megatron)
- Grouped-query attention (GQA) and multi-query attention (MQA)
- Rotary Position Embeddings (RoPE) [was added independently by the Megatron project subsequent to us]
- RMS layer norm
- FlashAttention 2
- BF16 / FP16 training
- Support for special tokens tokenizers
- WandB integration


User guide
----------

For information on installation and usage, take a look at our user guide.

.. toctree::
   :maxdepth: 2

   guide/index


API
---

Detailed information about Megatron-LLM components:

.. toctree::
   :maxdepth: 2

   api/index




Citation
--------

If you use this software please cite it:

.. code-block:: bib

   @software{epfmgtrn,
     author       = {Alejandro Hernández Cano  and
                     Matteo Pagliardini  and
                     Kyle Matoba  and
                     Amirkeivan Mohtashami  and
                     Olivia Simin Fan  and
                     Axel Marmet  and
                     Deniz Bayazit  and
                     Igor Krawczuk  and
                     Zeming Chen  and
                     Francesco Salvi  and
                     Antoine Bosselut  and
                     Martin Jaggi},
     title        = {epfLLM Megatron-LM},
     year         = 2023,
     url          = {https://github.com/epfLLM/Megatron-LLM}
   }
