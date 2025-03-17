<h1><center>Stable-Video-Diffusion</center></h1>
<h2>Get Start</h2> 
1. 在huggingface官网下载模型,这里给出<a href="https://huggingface.co/stabilityai/stable-video-diffusion-img2vid-xt" target="_blank">svd_xt</a>.<br>
由于直接从huggingface下载较慢，这里推荐使用<a href="https://hf-mirror.com/" target="_blank">HF-Mirror</a>.

中的 `hfd`  ，这里提供Windows使用方法.  
1. 下载<a href="https://hf-mirror.com/hfd/hfd.sh)/" target="_blank">hfd.sh</a>
2. 使用git bash运行`chmod a+x hfd.sh` ,`hfd.sh`详细使用见<a href="https://gist.github.com/padeoe/697678ab8e528b85a2a7bddafea1fa4f" target="_blank">hfd.sh</a>，在git bash中运行`export HF_ENDPOINT=https://alpha.hf-mirror.com`或`export HF_ENDPOINT=https://hf-mirror.com`(两个站点的下载速度不同,自行尝试),最后运行`./hfd.sh stabilityai/stable-video-diffusion-img2vid-xt --include svd_xt.safetensors --hf_username YOUR_HF_USERNAME_NOT_EMAIL --hf_token YOUR_HF_TOKEN `
<h2>ComfyUI</h2>
这里使用ComfyUI作为界面运行模型  

1. 下载`ComfyUI portable:`<a href="https://github.com/comfyanonymous/ComfyUI/releases" target="_blank">ComfyUI_windows_portable_nvidia.7z</a>.
2. 解压并双击`run_nvidia_gpu.bat`.
3. 下载`img2vid.json`，并将该文件拖拽ComfyUI页面中.
4. 将下载好的`svd_xt.safetensors`放到文件夹`ComfyUI_windows_portable/ComfyUI/models/checkpoints`.
5. 在`ComfyUI/custom_nodes`下打开git bash，运行`git clone https://github.com/ltdrdata/ComfyUI-Manager comfyui-manager`下载`ComfyUI-Manager`,将ComfyUI页面中缺失的`custom node`通过Manager安装.
6. 打开电脑设置,<a href="https://blog.csdn.net/Niuagha/article/details/131784306" target="_blank">调整虚拟内存</a>.
7. 上传图片，调整KSampler参数，执行运行就可以生成视频.(8G显存用1024*576的图片跑14帧视频生成足够了).













