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

## 📰 RM-Bench Leaderboard Update

Hi everyone! We have a few exciting updates and improvements to share with the community. Thank you once again for your enthusiastic support and contributions to RM-Bench!

### ✨ What’s New:

1. **License Type Column Added**  
   We've introduced a new column to the leaderboard to indicate each model's **license type**. This addition aims to make it easier for researchers and practitioners to identify models that are open for further development, research, or deployment.

2. **New Average Metrics: Domain Avg & Difficulty Avg**  
   Two new columns have been added:
   - **Domain Avg**: The average score across different domains (Chat, Code, Math, Safety).
   - **Difficulty Avg**: The average score across different difficulty levels (Easy, Normal, Hard).

3. **Clarification on Average Calculation**  
   We've noticed that in some cases, the reported `Overall` score may differ from the computed `Domain Avg` or `Difficulty Avg`. This is absolutely understandable — we realized we hadn’t clearly communicated our averaging method before. To clarify:

   We define the `Overall` score as:

Overall = Domain Avg = Difficulty Avg = (Chat + Code + Math + Safety) / 4

And each difficulty level is computed as:

Easy   = (Safety_Easy + Math_Easy + Chat_Easy + Code_Easy) / 4

Normal = (Safety_Normal + Math_Normal + Chat_Normal + Code_Normal) / 4

Hard   = (Safety_Hard + Math_Hard + Chat_Hard + Code_Hard) / 4

Following this definition ensures that **Domain Avg = Difficulty Avg = Overall**.

4. **New Column: Potentially Score Mismatch**  
To gently assist with clarity, we’ve added a `Potentially Score Mismatch` column. This column simply highlights cases where the reported averages might differ slightly from what’s expected under our standard formula.

If your model is flagged here, **please don’t worry at all** — this is very likely due to us not having communicated the averaging method clearly enough earlier on. It’s not an error on your part, and we truly appreciate the effort that goes into every submission.

If you'd like to recheck your scores or ensure alignment with our formula, we offer a small helper function that can recompute the averages for you. You can find it here:
👉 [`utils.py` from Line 48 to 75](https://github.com/THU-KEG/RM-Bench/blob/main/scripts/utils.py#L48-L75)

We hope this helps make the leaderboard more transparent and consistent for everyone. Thank you again for your understanding and collaboration! 💛

## Detailed Leaderboard
| Model Name                                                                                                                                   | Model Type      | Chat   | Math   | Code   | Safety   | Easy   | Normal   | Hard   | Domain Avg   | Difficulty Avg   |   Overall | Potentially Score Mismatch   | License Type   |
|:---------------------------------------------------------------------------------------------------------------------------------------------|:----------------|:-------|:-------|:-------|:---------|:-------|:---------|:-------|:-------------|:-----------------|----------:|:-----------------------------|:---------------|
| [Skywork-Reward-V2-Llama-3.1-8B-40M](https://arxiv.org/pdf/2507.01352)                                                                       | Scalar RM       | -      | -      | -      | -        | 97.6   | 96.9     | 93.5   | -            | 96.0             |      96   | Not Available                | Open Weight    |
| [Skywork-Reward-V2-Llama-3.1-8B](https://arxiv.org/pdf/2507.01352)                                                                           | Scalar RM       | -      | -      | -      | -        | 97.0   | 95.0     | 86.5   | -            | 92.8             |      92.8 | Not Available                | Open Weight    |
| [REWARDANYTHING-8B](https://huggingface.co/WisdomShell/RewardAnything-8B-v1)                                                                 | Reasoning GenRM | 76.7   | 90.3   | 75.2   | 90.2     | 89.4   | 85.3     | 84.4   | 83.1         | 86.4             |      86.4 | True                         | Open Weight    |
| [Llama-3.3-Nemotron-Super-49B-GenRM-Multilingual + voting@32](https://huggingface.co/nvidia/Llama-3_3-Nemotron-Super-49B-GenRM-Multilingual) | GenRM           | 76.3   | 93.2   | 79.0   | 93.5     | 92.1   | 88.5     | 75.9   | 85.5         | 85.5             |      85.5 | False                        | Open Source    |
| [DeepSeek R1](https://huggingface.co/deepseek-ai/DeepSeek-R1)                                                                                | Reasoning LLM   | 84.2   | 72.7   | 93.6   | 90.7     | -      | -        | 80.2   | 85.3         | 80.2             |      85.3 | Not Available                | Open Weight    |
| [Llama-3.3-Nemotron-Super-49B-GenRM-Multilingual](https://huggingface.co/nvidia/Llama-3_3-Nemotron-Super-49B-GenRM-Multilingual)             | GenRM           | 77.2   | 91.9   | 74.7   | 92.9     | 90.7   | 86.7     | 75.1   | 84.2         | 84.2             |      84.2 | False                        | Open Source    |
| [Llama-3.3-Nemotron-Super-49B-GenRM + voting@32](https://huggingface.co/nvidia/Llama-3_3-Nemotron-Super-49B-GenRM)                           | GenRM           | 74.0   | 92.7   | 77.4   | 92.1     | 92.6   | 87.3     | 72.3   | 84.0         | 84.1             |      84   | False                        | Open Source    |
| [RM-R1-DeepSeek-Distilled-Qwen-32B](https://huggingface.co/gaotang/RM-R1-DeepSeek-Distilled-Qwen-32B)                                        | Reasoning GenRM | 74.2   | 91.8   | 74.1   | 95.4     | 89.5   | 85.4     | 76.7   | 83.9         | 83.9             |      83.9 | False                        | Open Source    |
| [Llama-3.3-Nemotron-Super-49B-GenRM](https://huggingface.co/nvidia/Llama-3.3-Nemotron-Super-49B-GenRM)                                       | GenRM           | 73.7   | 91.4   | 75.0   | 90.6     | 91.2   | 85.7     | 71.2   | 82.7         | 82.7             |      82.7 | False                        | Open Source    |
| [J1-Llama-70B](https://arxiv.org/html/2505.10320v1)                                                                                          | Reasoning GenRM | -      | -      | -      | -        | -      | -        | -      | -            | -                |      82.7 | Not Available                | Open Weight    |
| [Skywork-Reward-V2-Qwen3-8B](https://arxiv.org/pdf/2507.01352)                                                                               | Scalar RM       | -      | -      | -      | -        | 91.9   | 85.7     | 70.1   | -            | 82.6             |      82.6 | Not Available                | Open Weight    |
| [Llama-3.3-Nemotron-70B-Reward-Multilingual](https://huggingface.co/nvidia/Llama-3.3-Nemotron-70B-Reward-Multilingual)                       | Scalar RM       | 86.2   | 82.4   | 66.8   | 94.1     | 84.3   | 84.5     | 78.3   | 82.4         | 82.4             |      82.4 | False                        | Open Source    |
| [Qwen-3-Nemotron-32B-Reward](https://huggingface.co/nvidia/Qwen-3-Nemotron-32B-Reward)                                                       | Scalar RM       | 86.1   | 76.1   | 70.2   | 95.2     | 85.1   | 83.4     | 77.3   | 81.9         | 81.9             |      81.9 | False                        | Open Source    |
| [Skywork-Reward-V2-Qwen3-4B](https://arxiv.org/pdf/2507.01352)                                                                               | Scalar RM       | -      | -      | -      | -        | 92.1   | 84.7     | 67.9   | -            | 81.6             |      81.6 | Not Available                | Open Weight    |
| [RM-R1-DeepSeek-Distilled-Qwen-14B](https://huggingface.co/gaotang/RM-R1-DeepSeek-Distilled-Qwen-14B)                                        | Reasoning GenRM | 71.8   | 90.5   | 69.5   | 94.1     | 86.2   | 83.6     | 74.4   | 81.5         | 81.4             |      81.5 | False                        | Open Source    |
| [Skywork-Reward-V2-Llama-3.2-3B](https://arxiv.org/pdf/2507.01352)                                                                           | Scalar RM       | -      | -      | -      | -        | 91.5   | 84.1     | 67.8   | -            | 81.1             |      81.1 | Not Available                | Open Weight    |
| [Llama-3.3-Nemotron-70B-Reward](https://huggingface.co/nvidia/Llama-3.3-Nemotron-70B-Reward)                                                 | Scalar RM       | 75.4   | 84.5   | 69.3   | 90.4     | 92.1   | 84.1     | 63.5   | 79.9         | 79.9             |      79.9 | False                        | Open Source    |
| [RM-R1-Qwen-Instruct-32B](https://huggingface.co/gaotang/RM-R1-Qwen-Instruct-32B)                                                            | Reasoning GenRM | 75.3   | 83.9   | 56.2   | 93.9     | 86.3   | 80.5     | 70.4   | 77.3         | 79.1             |      79.1 | True                         | Open Source    |
| [Skywork-Reward-V2-Qwen3-1.7B](https://arxiv.org/pdf/2507.01352)                                                                             | Scalar RM       | -      | -      | -      | -        | 93.0   | 83.4     | 59.7   | -            | 78.7             |      78.7 | Not Available                | Open Weight    |
| [Qwen-2.5-Nemotron-32B-Reward](https://huggingface.co/nvidia/Qwen-2.5-Nemotron-32B-Reward)                                                   | Scalar RM       | 76.0   | 73.9   | 66.2   | 93.5     | 85.6   | 80.5     | 65.9   | 77.4         | 77.3             |      77.4 | False                        | Open Source    |
| [GPT-4.1](https://openai.com)                                                                                                                | LLM             | 79.5   | 68.1   | 67.3   | 93.1     | 85.7   | 77.0     | 69.5   | 77.0         | 77.4             |      77.4 | False                        | Proprietary    |
| [Skywork-Reward-V2-Llama-3.2-1B](https://arxiv.org/pdf/2507.01352)                                                                           | Scalar RM       | -      | -      | -      | -        | 91.3   | 79.9     | 57.8   | -            | 76.3             |      76.3 | Not Available                | Open Weight    |
| [RM-R1-Qwen-Instruct-14B](https://huggingface.co/gaotang/RM-R1-Qwen-Instruct-14B)                                                            | Reasoning GenRM | 75.6   | 75.4   | 60.6   | 93.6     | 82.6   | 77.5     | 68.8   | 76.3         | 76.3             |      76.1 | False                        | Open Source    |
| [Qwen3-8B](https://huggingface.co/Qwen/Qwen3-8B)                                                                                             | LLM             | 66.5   | 77.1   | 57.0   | 84.4     | 76.4   | 74.3     | 74.4   | 71.2         | 75.0             |      75   | True                         | Open Weight    |
| [Skywork-Reward-V2-Qwen3-0.6B](https://arxiv.org/pdf/2507.01352)                                                                             | Scalar RM       | -      | -      | -      | -        | 90.3   | 78.0     | 54.8   | -            | 74.4             |      74.4 | Not Available                | Open Weight    |
| [DeepSeek V3](https://huggingface.co/deepseek-ai/DeepSeek-V3)                                                                                | LLM             | 76.3   | 65.7   | 62.2   | 88.3     | 80.4   | 73.2     | 67.3   | 73.1         | 73.6             |      73.6 | False                        | Open Weight    |
| [Skywork-Reward-Llama-3.1-8B-v0.2](https://huggingface.co/Skywork/Skywork-Reward-Llama-3.1-8B-v0.2)                                          | Scalar RM       | 69.3   | 62.1   | 53.4   | 96.0     | 89.3   | 75.8     | 52.6   | 70.2         | 72.6             |      72.6 | True                         | Open Source    |
| [RM-R1-DeepSeek-Distilled-Qwen-7B](https://huggingface.co/gaotang/RM-R1-DeepSeek-Distilled-Qwen-7B)                                          | Reasoning GenRM | 64.0   | 83.9   | 56.2   | 85.3     | 75.9   | 73.1     | 68.1   | 72.4         | 72.4             |      72.4 | False                        | Open Source    |
| [GRM-Llama3.2-3B-rewardmodel-ft](https://huggingface.co/Ray2333/GRM-Llama3.2-3B-rewardmodel-ft)                                              | Scalar RM       | 68.6   | 61.9   | 52.8   | 95.2     | 90.8   | 75.9     | 49.4   | 69.6         | 72.0             |      72   | True                         | Open Source    |
| [FsfairX-LLLaMA3-RM-v0.1](https://huggingface.co/sfairXC/FsfairX-LLaMA3-RM-v0.1)                                                             | Scalar RM       | 67.3   | 62.8   | 55.7   | 91.8     | 87.4   | 74.8     | 52.8   | 69.4         | 71.7             |      71.7 | True                         | Open Source    |
| [Self-taught-evaluator-llama3.1-70B](https://huggingface.co/facebook/Self-taught-evaluator-llama3.1-70B)                                     | GenRM           | 73.4   | 65.7   | 56.3   | 90.4     | 80.2   | 74.5     | 59.7   | 71.5         | 71.5             |      71.5 | False                        | Open Source    |
| [INF-ORM-Llama3.1-70B](https://huggingface.co/infly/INF-ORM-Llama3.1-70B)                                                                    | Scalar RM       | 66.3   | 65.6   | 56.8   | 94.8     | 91.8   | 76.1     | 44.8   | 70.9         | 70.9             |      70.9 | False                        | Open Source    |
| [Llama-3.1-Nemotron-70B-Reward](https://huggingface.co/nvidia/Llama-3.1-Nemotron-70B-Reward)                                                 | Scalar RM       | 70.7   | 64.3   | 57.4   | 90.3     | 92.5   | 76.4     | 43.1   | 70.7         | 70.7             |      70.7 | False                        | Open Source    |
| [RM-R1-Qwen-Instruct-7B](https://huggingface.co/gaotang/RM-R1-Qwen-Instruct-7B)                                                              | Reasoning GenRM | 66.6   | 67.0   | 54.6   | 92.6     | 79.2   | 71.7     | 59.7   | 70.2         | 70.2             |      70.2 | False                        | Open Source    |
| [Skywork-Reward-Llama-3.1-8B](https://huggingface.co/Skywork/Skywork-Reward-Llama-3.1-8B)                                                    | Scalar RM       | 69.5   | 60.6   | 54.5   | 95.7     | 89.0   | 74.7     | 46.6   | 70.1         | 70.1             |      70.1 | False                        | Open Source    |
| [URM-LLama-3.1-8B](https://huggingface.co/LxzGordon/URM-LLaMa-3.1-8B)                                                                        | Scalar RM       | 71.2   | 61.8   | 54.1   | 93.1     | 84.0   | 73.2     | 53.0   | 70.0         | 70.1             |      70   | False                        | Open Source    |
| [Nemotron-340B-Reward](https://huggingface.co/nvidia/Nemotron-340B-Reward)                                                                   | Scalar RM       | 71.2   | 59.8   | 59.4   | 87.5     | 81.0   | 71.4     | 56.1   | 69.5         | 69.5             |      69.5 | False                        | Open Source    |
| [Llama-3-OffsetBias-RM-8B](https://huggingface.co/NCSOFT/Llama-3-OffsetBias-RM-8B)                                                           | Scalar RM       | 71.3   | 61.9   | 53.2   | 89.6     | 84.6   | 72.2     | 50.2   | 69.0         | 69.0             |      69   | False                        | Open Source    |
| [internlm2-20b-reward](https://huggingface.co/internlm/internlm2-20b-reward)                                                                 | Scalar RM       | 63.1   | 66.8   | 56.7   | 86.5     | 82.6   | 71.6     | 50.7   | 68.3         | 68.3             |      68.3 | False                        | Open Source    |
| [GRM-llama3-8B-sftreg](https://huggingface.co/Ray2333/GRM-llama3-8B-sftreg)                                                                  | Scalar RM       | 62.7   | 62.5   | 57.8   | 90.0     | 83.5   | 72.7     | 48.6   | 68.2         | 68.3             |      68.2 | False                        | Open Source    |
| [EvalPlanner-Llama-8B](https://openreview.net/forum?id=PNRznmmWP7)                                                                           | GenRM           | -      | -      | -      | -        | -      | -        | -      | -            | -                |      68.1 | Not Available                | Unknown        |
| [ArmoRM-Llama3-8B-v0.1](https://huggingface.co/RLHFlow/ArmoRM-Llama3-8B-v0.1)                                                                | Scalar RM       | 67.8   | 57.5   | 53.1   | 92.4     | 82.2   | 71.0     | 49.8   | 67.7         | 67.7             |      67.7 | False                        | Open Source    |
| [Skywork-Reward-Gemma-2-27B](https://huggingface.co/Skywork/Skywork-Reward-Gemma-2-27B)                                                      | Scalar RM       | 69.5   | 54.7   | 53.2   | 91.9     | 78.0   | 69.2     | 54.9   | 67.3         | 67.4             |      67.3 | False                        | Open Source    |
| [internlm2-7b-reward](https://huggingface.co/internlm/internlm2-7b-reward)                                                                   | Scalar RM       | 61.7   | 71.4   | 49.7   | 85.5     | 85.4   | 70.7     | 45.1   | 67.1         | 67.1             |      67.1 | False                        | Open Source    |
| [Eurus-RM-7b](https://huggingface.co/openbmb/Eurus-RM-7b)                                                                                    | Scalar RM       | 59.9   | 60.2   | 56.9   | 86.5     | 87.2   | 70.2     | 40.2   | 65.9         | 65.9             |      65.9 | False                        | Open Source    |
| [SOLAR-10.7B-Instruct-v1.0](https://huggingface.co/upstage/SOLAR-10.7B-Instruct-v1.0)                                                        | GenRM           | 78.6   | 52.3   | 49.6   | 78.9     | 57.5   | 67.6     | 69.4   | 64.8         | 64.8             |      64.8 | False                        | Open Source    |
| [JudgeLRM](https://arxiv.org/abs/2504.00050)                                                                                                 | Reasoning GenRM | 59.9   | 59.9   | 51.9   | 87.3     | 73.2   | 66.2     | 54.8   | 64.8         | 64.7             |      64.7 | False                        | Open Weight    |
| [RM-Mistral-7B](https://huggingface.co/weqweasdas/RM-Mistral-7B)                                                                             | Scalar RM       | 57.4   | 57.0   | 52.7   | 87.2     | 88.6   | 67.1     | 34.9   | 63.6         | 63.5             |      63.5 | False                        | Open Source    |
| [Mistral-7B-instruct-Unified-Feedback](https://huggingface.co/Ray2333/reward-model-Mistral-7B-instruct-Unified-Feedback)                     | Scalar RM       | 56.5   | 58.0   | 51.7   | 86.8     | 87.1   | 67.3     | 35.3   | 63.2         | 63.2             |      63.2 | False                        | Open Source    |
| [tulu-v2.5-70b-preference-mix-rm](https://huggingface.co/allenai/tulu-v2.5-70b-preference-mix-rm)                                            | Scalar RM       | 58.2   | 51.4   | 55.5   | 87.1     | 72.8   | 65.6     | 50.7   | 63.0         | 63.0             |      63   | False                        | Open Source    |
| [stablelm-2-12b-chat](https://huggingface.co/stabilityai/stablelm-2-12b-chat)                                                                | LLM             | 67.2   | 54.9   | 51.6   | 65.2     | 69.1   | 63.5     | 46.6   | 59.7         | 59.7             |      59.7 | False                        | Open Weight    |