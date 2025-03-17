<h1><center>Stable-Video-Diffusion</center></h1>
<h2>Get Start</h2> 
1. 在huggingface官网下载模型,这里给出<a href="https://huggingface.co/stabilityai/stable-video-diffusion-img2vid-xt" target="_blank">svd_xt</a>.<br>.
由于使用VPN或梯子从huggingface下载较慢，这里推荐使用<a href="https://hf-mirror.com/" target="_blank">HF-Mirror</a>.

中的 `hfd`  ，这里提供Windows使用方法.  
1. 下载<a href="https://hf-mirror.com/hfd/hfd.sh)/" target="_blank">hfd.sh</a>
2. 使用git bash运行`chmod a+x hfd.sh` ,`hfd.sh`详细使用见<a href="https://gist.github.com/padeoe/697678ab8e528b85a2a7bddafea1fa4f" target="_blank">hfd.sh</a>，在git bash中运行`export HF_ENDPOINT=https://alpha.hf-mirror.com`或`export HF_ENDPOINT=https://hf-mirror.com`(两个站点的下载速度不同,自行尝试),最后运行`./hfd.sh stabilityai/stable-video-diffusion-img2vid-xt --include svd_xt.safetensors --hf_username YOUR_HF_USERNAME_NOT_EMAIL --hf_token YOUR_HF_TOKEN `
<h2>CompfyUI</h2>
这里使用CompfyUI作为界面运行模型  

1. 下载`CompfyUI portable:`<a href="https://github.com/comfyanonymous/ComfyUI/releases" target="_blank">ComfyUI_windows_portable_nvidia.7z</a>
2. 解压并双击`run_nvidia_gpu.bat`
3. 













