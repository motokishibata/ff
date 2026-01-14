1. apt update
2. apt install -y git-all ffmpeg
3. bash Miniconda3-latest-Linux-x86_64-autoinput.sh
4. conda install nvidia/label/cuda-12.1.0::cuda-runtime nvidia/label/cudnn-9.10.0::cudnn
   ※cudaのバージョンは12.1～12.4が互換
5. python install.py --onnxruntime cuda --skip-conda
6. python facefusion.py run