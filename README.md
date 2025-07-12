# 🏆 RM-Bench Leaderboard

Welcome to the RM-Bench Leaderboard!

First off, a big **thank you** to the community! Since the release of [RM-Bench](https://arxiv.org/abs/2410.16184), we’re excited to see **50+ reward models** evaluated using our benchmark. To facilitate further research and model comparison, we are launching this public leaderboard.

🔍 **Notes:**
- The results listed here are mainly taken from the original papers or project reports.  
- If you find any mistakes or inconsistencies, please [open an issue](https://github.com/THU-KEG/RM-Bench-Leaderboard/issues) to let us know.

📢 **Contribute Your Results:**
We welcome everyone to submit their results!  
To add your model:
1. Open a Pull Request (PR).
2. Include a link to your paper/project.
3. (Optional but appreciated) Attach your RM-Bench result file for reproducibility.

⚠️ **Please note:**  
The leaderboard is still **under construction**, and there may be bugs or layout changes as we improve it. Thanks for your understanding!

🎉 Enjoy exploring and contributing to reward model research!


## Detailed Leaderboard
| Model Name                                                                                                                                   | Model Type      | Chat   | Math   | Code   | Safety   | Easy   | Normal   | Hard   |   Overall |
|:---------------------------------------------------------------------------------------------------------------------------------------------|:----------------|:-------|:-------|:-------|:---------|:-------|:---------|:-------|----------:|
| [Skywork-Reward-V2-Llama-3.1-8B-40M](https://arxiv.org/pdf/2507.01352)                                                                       | Scalar RM       | -      | -      | -      | -        | 97.6   | 96.9     | 93.5   |      96   |
| [Skywork-Reward-V2-Llama-3.1-8B](https://arxiv.org/pdf/2507.01352)                                                                           | Scalar RM       | -      | -      | -      | -        | 97.0   | 95.0     | 86.5   |      92.8 |
| [REWARDANYTHING-8B](https://huggingface.co/WisdomShell/RewardAnything-8B-v1)                                                                 | Reasoning GenRM | 76.7   | 90.3   | 75.2   | 90.2     | 89.4   | 85.3     | 84.4   |      86.4 |
| [Llama-3.3-Nemotron-Super-49B-GenRM-Multilingual + voting@32](https://huggingface.co/nvidia/Llama-3_3-Nemotron-Super-49B-GenRM-Multilingual) | GenRM           | 76.3   | 93.2   | 79.0   | 93.5     | 92.1   | 88.5     | 75.9   |      85.**5** |
| [DeepSeek R1](https://huggingface.co/deepseek-ai/DeepSeek-R1)                                                                                | Reasoning LLM   | 84.2   | 72.7   | 93.6   | 90.7     | -      | -        | 80.2   |      85.3 |
| [Llama-3.3-Nemotron-Super-49B-GenRM-Multilingual](https://huggingface.co/nvidia/Llama-3_3-Nemotron-Super-49B-GenRM-Multilingual)             | GenRM           | 77.2   | 91.9   | 74.7   | 92.9     | 90.7   | 86.7     | 75.1   |      84.2 |
| [Llama-3.3-Nemotron-Super-49B-GenRM + voting@32](https://huggingface.co/nvidia/Llama-3_3-Nemotron-Super-49B-GenRM)                           | GenRM           | 74.0   | 92.7   | 77.4   | 92.1     | 92.6   | 87.3     | 72.3   |      84   |
| [RM-R1-DeepSeek-Distilled-Qwen-32B](https://huggingface.co/gaotang/RM-R1-DeepSeek-Distilled-Qwen-32B)                                        | Reasoning GenRM | 74.2   | 91.8   | 74.1   | 95.4     | 89.5   | 85.4     | 76.7   |      83.9 |
| [Llama-3.3-Nemotron-Super-49B-GenRM](https://huggingface.co/nvidia/Llama-3.3-Nemotron-Super-49B-GenRM)                                       | GenRM           | 73.7   | 91.4   | 75.0   | 90.6     | 91.2   | 85.7     | 71.2   |      82.7 |
| [J1-Llama-70B](https://arxiv.org/html/2505.10320v1)                                                                                          | Reasoning GenRM | -      | -      | -      | -        | -      | -        | -      |      82.7 |
| [Skywork-Reward-V2-Qwen3-8B](https://arxiv.org/pdf/2507.01352)                                                                               | Scalar RM       | -      | -      | -      | -        | 91.9   | 85.7     | 70.1   |      82.6 |
| [Llama-3.3-Nemotron-70B-Reward-Multilingual](https://huggingface.co/nvidia/Llama-3.3-Nemotron-70B-Reward-Multilingual)                       | GenRM           | 86.2   | 82.4   | 66.8   | 94.1     | 86.5   | 85.4     | 80.0   |      82.4 |
| [Qwen-3-Nemotron-32B-Reward](https://huggingface.co/nvidia/Qwen-3-Nemotron-32B-Reward)                                                       | GenRM           | 86.1   | 76.1   | 70.2   | 95.2     | 85.1   | 83.4     | 77.3   |      81.9 |
| [Skywork-Reward-V2-Qwen3-4B](https://arxiv.org/pdf/2507.01352)                                                                               | Scalar RM       | -      | -      | -      | -        | 92.1   | 84.7     | 67.9   |      81.6 |
| [RM-R1-DeepSeek-Distilled-Qwen-14B](https://huggingface.co/gaotang/RM-R1-DeepSeek-Distilled-Qwen-14B)                                        | Reasoning GenRM | 71.8   | 90.5   | 69.5   | 94.1     | 86.2   | 83.6     | 74.4   |      81.5 |
| [Skywork-Reward-V2-Llama-3.2-3B](https://arxiv.org/pdf/2507.01352)                                                                           | Scalar RM       | -      | -      | -      | -        | 91.5   | 84.1     | 67.8   |      81.1 |
| [Llama-3.3-Nemotron-70B-Reward](https://huggingface.co/nvidia/Llama-3.3-Nemotron-70B-Reward)                                                 | GenRM           | 75.4   | 84.5   | 69.3   | 90.4     | 92.1   | 85.7     | 71.1   |      79.9 |
| [RM-R1-Qwen-Instruct-32B](https://huggingface.co/gaotang/RM-R1-Qwen-Instruct-32B)                                                            | Reasoning GenRM | 75.3   | 83.9   | 56.2   | 93.9     | 86.3   | 80.5     | 70.4   |      79.1 |
| [Skywork-Reward-V2-Qwen3-1.7B](https://arxiv.org/pdf/2507.01352)                                                                             | Scalar RM       | -      | -      | -      | -        | 93.0   | 83.4     | 59.7   |      78.7 |
| [Qwen-2.5-Nemotron-32B-Reward](https://huggingface.co/nvidia/Qwen-2.5-Nemotron-32B-Reward)                                                   | GenRM           | 76.0   | 73.9   | 66.2   | 93.5     | 85.6   | 80.5     | 65.9   |      77.4 |
| [GPT-4.1](https://openai.com)                                                                                                                | LLM             | 79.5   | 68.1   | 67.3   | 93.1     | 85.7   | 77.0     | 69.5   |      77.4 |
| [Skywork-Reward-V2-Llama-3.2-1B](https://arxiv.org/pdf/2507.01352)                                                                           | Scalar RM       | -      | -      | -      | -        | 91.3   | 79.9     | 57.8   |      76.3 |
| [RM-R1-Qwen-Instruct-14B](https://huggingface.co/gaotang/RM-R1-Qwen-Instruct-14B)                                                            | Reasoning GenRM | 75.6   | 75.4   | 60.6   | 93.6     | 82.6   | 77.5     | 68.8   |      76.1 |
| [Qwen3-8B](https://huggingface.co/Qwen/Qwen3-8B)                                                                                             | LLM             | 66.5   | 77.1   | 57.0   | 84.4     | 76.4   | 74.3     | 74.4   |      75   |
| [Skywork-Reward-V2-Qwen3-0.6B](https://arxiv.org/pdf/2507.01352)                                                                             | Scalar RM       | -      | -      | -      | -        | 90.3   | 78.0     | 54.8   |      74.4 |
| [DeepSeek V3](https://huggingface.co/deepseek-ai/DeepSeek-V3)                                                                                | LLM             | 76.3   | 65.7   | 62.2   | 88.3     | 80.4   | 73.2     | 67.3   |      73.6 |
| [Skywork-Reward-Llama-3.1-8B-v0.2](https://huggingface.co/Skywork/Skywork-Reward-Llama-3.1-8B-v0.2)                                          | Scalar RM       | 69.3   | 62.1   | 53.4   | 96.0     | 89.3   | 75.8     | 52.6   |      72.6 |
| [RM-R1-DeepSeek-Distilled-Qwen-7B](https://huggingface.co/gaotang/RM-R1-DeepSeek-Distilled-Qwen-7B)                                          | Reasoning GenRM | 64.0   | 83.9   | 56.2   | 85.3     | 75.9   | 73.1     | 68.1   |      72.4 |
| [GRM-Llama3.2-3B-rewardmodel-ft](https://huggingface.co/Ray2333/GRM-Llama3.2-3B-rewardmodel-ft)                                              | Scalar RM       | 68.6   | 61.9   | 52.8   | 95.2     | 90.8   | 75.9     | 49.4   |      72   |
| [FsfairX-LLLaMA3-RM-v0.1](https://huggingface.co/sfairXC/FsfairX-LLaMA3-RM-v0.1)                                                             | Scalar RM       | 67.3   | 62.8   | 55.7   | 91.8     | 87.4   | 74.8     | 52.8   |      71.7 |
| [Self-taught-evaluator-llama3.1-70B](https://huggingface.co/facebook/Self-taught-evaluator-llama3.1-70B)                                     | GenRM           | 73.4   | 65.7   | 56.3   | 90.4     | 80.2   | 74.5     | 59.7   |      71.5 |
| [INF-ORM-Llama3.1-70B](https://huggingface.co/infly/INF-ORM-Llama3.1-70B)                                                                    | Scalar RM       | 66.3   | 65.6   | 56.8   | 94.8     | 91.8   | 76.1     | 44.8   |      70.9 |
| [Llama-3.1-Nemotron-70B-Reward](https://huggingface.co/nvidia/Llama-3.1-Nemotron-70B-Reward)                                                 | GenRM           | 70.7   | 64.3   | 57.4   | 90.3     | 92.2   | 76.8     | 48.0   |      70.7 |
| [RM-R1-Qwen-Instruct-7B](https://huggingface.co/gaotang/RM-R1-Qwen-Instruct-7B)                                                              | Reasoning GenRM | 66.6   | 67.0   | 54.6   | 92.6     | 79.2   | 71.7     | 59.7   |      70.2 |
| [Skywork-Reward-Llama-3.1-8B](https://huggingface.co/Skywork/Skywork-Reward-Llama-3.1-8B)                                                    | Scalar RM       | 69.5   | 60.6   | 54.5   | 95.7     | 89.0   | 74.7     | 46.6   |      70.1 |
| [URM-LLama-3.1-8B](https://huggingface.co/LxzGordon/URM-LLaMa-3.1-8B)                                                                        | Scalar RM       | 71.2   | 61.8   | 54.1   | 93.1     | 84.0   | 73.2     | 53.0   |      70   |
| [Nemotron-340B-Reward](https://huggingface.co/nvidia/Nemotron-340B-Reward)                                                                   | Scalar RM       | 71.2   | 59.8   | 59.4   | 87.5     | 81.0   | 71.4     | 56.1   |      69.5 |
| [Llama-3-OffsetBias-RM-8B](https://huggingface.co/NCSOFT/Llama-3-OffsetBias-RM-8B)                                                           | Scalar RM       | 71.3   | 61.9   | 53.2   | 89.6     | 84.6   | 72.2     | 50.2   |      69   |
| [internlm2-20b-reward](https://huggingface.co/internlm/internlm2-20b-reward)                                                                 | Scalar RM       | 63.1   | 66.8   | 56.7   | 86.5     | 82.6   | 71.6     | 50.7   |      68.3 |
| [GRM-llama3-8B-sftreg](https://huggingface.co/Ray2333/GRM-llama3-8B-sftreg)                                                                  | Scalar RM       | 62.7   | 62.5   | 57.8   | 90.0     | 83.5   | 72.7     | 48.6   |      68.2 |
| [EvalPlanner-Llama-8B](https://openreview.net/forum?id=PNRznmmWP7)                                                                           | GenRM           | -      | -      | -      | -        | -      | -        | -      |      68.1 |
| [ArmoRM-Llama3-8B-v0.1](https://huggingface.co/RLHFlow/ArmoRM-Llama3-8B-v0.1)                                                                | Scalar RM       | 67.8   | 57.5   | 53.1   | 92.4     | 82.2   | 71.0     | 49.8   |      67.7 |
| [Skywork-Reward-Gemma-2-27B](https://huggingface.co/Skywork/Skywork-Reward-Gemma-2-27B)                                                      | Scalar RM       | 69.5   | 54.7   | 53.2   | 91.9     | 78.0   | 69.2     | 54.9   |      67.3 |
| [internlm2-7b-reward](https://huggingface.co/internlm/internlm2-7b-reward)                                                                   | Scalar RM       | 61.7   | 71.4   | 49.7   | 85.5     | 85.4   | 70.7     | 45.1   |      67.1 |
| [Eurus-RM-7b](https://huggingface.co/openbmb/Eurus-RM-7b)                                                                                    | Scalar RM       | 59.9   | 60.2   | 56.9   | 86.5     | 87.2   | 70.2     | 40.2   |      65.9 |
| [SOLAR-10.7B-Instruct-v1.0](https://huggingface.co/upstage/SOLAR-10.7B-Instruct-v1.0)                                                        | GenRM           | 78.6   | 52.3   | 49.6   | 78.9     | 57.5   | 67.6     | 69.4   |      64.8 |
| [JudgeLRM](https://arxiv.org/abs/2504.00050)                                                                                                 | Reasoning GenRM | 59.9   | 59.9   | 51.9   | 87.3     | 73.2   | 66.2     | 54.8   |      64.7 |
| [RM-Mistral-7B](https://huggingface.co/weqweasdas/RM-Mistral-7B)                                                                             | Scalar RM       | 57.4   | 57.0   | 52.7   | 87.2     | 88.6   | 67.1     | 34.9   |      63.5 |
| [Mistral-7B-instruct-Unified-Feedback](https://huggingface.co/Ray2333/reward-model-Mistral-7B-instruct-Unified-Feedback)                     | Scalar RM       | 56.5   | 58.0   | 51.7   | 86.8     | 87.1   | 67.3     | 35.3   |      63.2 |
| [tulu-v2.5-70b-preference-mix-rm](https://huggingface.co/allenai/tulu-v2.5-70b-preference-mix-rm)                                            | Scalar RM       | 58.2   | 51.4   | 55.5   | 87.1     | 72.8   | 65.6     | 50.7   |      63   |
| [stablelm-2-12b-chat](https://huggingface.co/stabilityai/stablelm-2-12b-chat)                                                                | LLM             | 67.2   | 54.9   | 51.6   | 65.2     | 69.1   | 63.5     | 46.6   |      59.7 |