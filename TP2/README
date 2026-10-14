This repository contains the code, theoretical explanations, and answers for Lab Session 2: Pretraining and Supervised Finetuning, part of the APM 53674: ALTeGraD course.   

Instructor: Prof. Michalis Vazirgiannis   Teaching Assistants: Amr Mohamed and Yang Zhang   Institution: École Polytechnique / Master's Level AI Curriculum🚀 

Overview:
The objective of this lab is to gain hands-on experience in adapting Large Language Models (LLMs) to specific tasks using parameter-efficient fine-tuning (PEFT), quantization, and prompt formatting techniques.   Key Components Covered:Instruction Fine-Tuning: Adapting a pretrained base model into a helpful conversational assistant using instruction-response pairs.   Model Architecture & Quantization: Loading Qwen/Qwen3.5-0.8B-Base using 4-bit NormalFloat (NF4) quantization via bitsandbytes to minimize GPU VRAM consumption on consumer-grade hardware (such as a Google Colab T4 GPU).   Parameter-Efficient Fine-Tuning (LoRA): Injecting low-rank adaptation matrices into the token-mixing layers and MLP blocks to train only a small fraction of the total parameters (~21.6M trainable parameters out of ~0.75B).   French Summarization Task: Fine-tuning the model on giuliadc/orangesum_5k (a French news summarization dataset) with custom chat templates and completion-only loss masking.   Evaluation & Tool Calling: Comparing generations and held-out evaluation loss before and after fine-tuning, followed by functional tool-calling setups.   

🛠️ Requirements & Installation :
This lab is designed to run in environments like Google Colab (T4 GPU) or local machines with CUDA support.   To install the required ecosystem libraries (transformers, datasets, peft, bitsandbytes), 
run:   Bashpip install -q "transformers==5.18.0" "accelerate==1.15.0" "peft==0.21.2" "bitsandbytes==0.50.2"
pip uninstall -y -q torchao

📂 Structure of the Notebook :
Introduction & Setup: Environment checks (nvidia-smi) and package installations.   Quantization & BitsAndBytes Configuration: Analysis of computation dtype (bnb_4bit_compute_dtype) and double quantization benefits.   LoRA Configuration: Setting up rank ($r = 8$), alpha ($32$), and dropout parameters for target linear projection modules.   Baseline Inference: Testing the base model prior to fine-tuning on general queries and French article summarization prompts.   Dataset Preparation & Completion-Only Training: Tokenizing the giuliadc/orangesum_5k dataset, setting prompt labels to -100 to ignore instruction loss, and managing padding with DataCollatorForSeq2Seq.   Training & Evaluation: Configuring the Hugging Face Trainer with gradient checkpointing, mixed-precision (fp16), and logging/evaluation steps.  
