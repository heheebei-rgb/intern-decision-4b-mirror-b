# Intern-Decision-4B 权重镜像 Part B（GitHub 源码包分发）

[internlm/Intern-Decision-4B](https://github.com/internlm/Intern-Decision) 权重分块镜像 **Part B**（需与 Part A 一起下载）。

## 下载与重建
1. **Code → Download ZIP**，与 Part A 的 ZIP 解压到同一目录
2. 本目录执行 `python3 merge_and_verify.py`
3. 产物: `model-language-0002-save_rank0.safetensors` (3.87GB) + `model-vision-0001` (584MB) + `model-projector` (52MB) + tokenizer 全套

## 推理
两 part 合并完成后，目录里有 `model.safetensors.index.json` + `inference.py`，transformers 直接加载（BF16 约需 9-10GB 显存）。
