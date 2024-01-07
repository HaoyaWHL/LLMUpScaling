# LLMUpScaling

本项目旨在收集最全的从SLM到LLM的UpScaling方法

## 名词解释

| 缩写| 全程   |
| :--------  | :-----  |
| SLM| small language model|
| LLM| large language model|
| UpScaling | 在Gopher的文章中也称reverse distillatio|

## 函数列表

| method        | 对应文件   |  方案说明  |
| :--------  | :-----  | :----:  |
| concat| concat_diff_layers.py|把两个slm的不同层合并为一个llm|
|linear interpolation | linear_inter_layers.py |通过线性插值的方式把slm扩充为llm|
|random initialize | random_add_layers.py |初始化需要扩充的层数并拼接在现有slm之中|
|add_width | add_width_layers.py |扩充slm的hidden_size从而达到llm的参数量|

## Reference

1. [《SOLAR 10.7B: Scaling Large Language Models with Simple yet Effective Depth Up-Scaling 》](https://arxiv.org/pdf/2312.15166.pdf)
2. [《Scaling Language Models: Methods, Analysis & Insights from Training Gopher》](https://arxiv.org/pdf/2112.11446.pdf)

---

## `Todo` 列表

- [x] 增加以上函数的jupyter文件；
- [x] 增加对应py文件；
- [x] 增加对应原理图；
- [x] 增加训练框架；
- [x] 发布7B-70B模型在huggingface上

---

最新更新于 2024.01.07
