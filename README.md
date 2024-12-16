# **2024年第二届科学智能大赛地球科学赛道：AI极端降水预报**  
[大赛链接](http://competition.sais.com.cn/competitionDetail/532234/format)
<img width="1505" alt="image" src="https://github.com/user-attachments/assets/06f76c9c-2aa7-4f05-894d-525225218c57">

## Data Demo
```bash
https://github.com/zhengkai15/extreme-precipitation-demo.git
```
## **Top 10 尝试方案开源代码**
本项目为 **“2024年第二届科学智能大赛地球科学赛道：AI极端降水预报”** 的尝试方案，经过线下测试可进入 **Top 10**。  
开源目标是分享一个工程化的实现，方便其他研究者和开发者快速复现结果，并探索 **鲁棒性结论**。此外，项目中会逐步分享一些个人的实验分析和心得。

## **代码结构**

```plaintext
.
├── exp/                # 实验结果文件夹（输出路径）
├── code/               # 核心代码实现（数据处理、模型定义等）
├── conf/               # 配置文件（实验参数配置）
├── run_script/         # 运行脚本（批量测试或训练）
├── train_main.py       # 主程序入口（训练、推理等）
└── requirements.txt    # 环境依赖文件
```

## 运行方式

1. Debug 模式

用于快速调试和小规模测试：
```shell
python -u train_main.py \
    --noise.use_noise true \
    --training.batch_size 1 \
    --debug.verbose true \
    --model.name unet
```
2. 批量试验对比

运行批量实验脚本：
```shell
bash run_script/?.sh
```

## 试验结论分析
实验结果分析和结论将逐步补充，敬请期待。

## 环境依赖
安装所需依赖：
```shell
pip install -r requirements.txt
```

## 开源说明
欢迎研究者和开发者在此基础上改进，任何贡献和反馈都非常感谢！
