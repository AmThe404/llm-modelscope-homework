# llm-modelscope-homework
ModelScope 大语言模型部署与问答测试作业
# ModelScope 大语言模型部署体验

## 一、项目说明

本项目为“大语言模型部署体验”课程作业。实验在 ModelScope DSW-CPU 环境中完成，通过自建 `llm_env` Python 虚拟环境，安装 PyTorch、Transformers、ModelScope 等依赖，并完成两个开源大语言模型的部署与问答测试。

## 二、实验环境

- 平台：ModelScope 魔搭社区
- 环境：DSW-CPU
- Notebook 内核：llm_env
- 主要依赖：torch、transformers、modelscope、accelerate

## 三、测试模型

本实验测试了两个开源大语言模型：

1. Qwen/Qwen2.5-0.5B-Instruct
2. Qwen/Qwen2.5-1.5B-Instruct

## 四、测试内容

主要围绕中文语义理解、歧义句分析和简单逻辑推理进行问答测试。

测试问题示例：

1. 请说出以下两句话区别在哪里？冬天：能穿多少穿多少。夏天：能穿多少穿多少。
2. 单身狗产生的原因有两个，一是谁都看不上，二是谁都看不上。
3. 他知道我知道你知道他不知道吗？这句话里，到底谁不知道？
4. 明明明明明白白白喜欢他，可她就是不说。这句话里，明明和白白谁喜欢谁？

## 五、文件说明

- `llm_test.ipynb`：模型下载、加载和问答测试代码
- `screenshots/`：实验过程与问答结果截图

## 六、实验结论

两个模型均能完成基本中文问答任务。其中，较大参数模型在回答完整性和语义解释方面通常更好，但在 CPU 环境下运行速度较慢；较小模型运行速度较快，但在复杂歧义句和逻辑推理问题上的回答稳定性略弱。
