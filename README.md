# ADL HW3 

## Environment
'''
cd axolotl

pip3 install packaging
pip3 install -e '.[flash-attn,deepspeed]'
'''
Install and set up the environment.

## Train Qlora
'''
// modify the path of base model path, datasets path, and output_dir to desired path and run:
accelerate launch -m axolotl.cli.train examples/llama-2/qlora.yml
'''

## Inference
'''
sh run.sh [path_to_base_model] [path_to_peft_model] [input_data_path] [output_data_path]
'''

