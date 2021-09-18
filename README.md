# P2_WebNLG2020

This is the GitHub repo for our paper "[**P2: A Plan-and-Pretrain Approach for Knowledge Graph-to-Text Generation**](https://zhijing-jin.com/files/papers/P2_2020.pdf)" by Qipeng Guo, Zhijing Jin, Ning Dai, Xipeng Qiu, Xiangyang Xue, David Wipf, and Zheng Zhang. 

Our model achieves the [top #1](https://gerbil-nlg.dice-research.org/gerbil/webnlg2020results) performance at the English track of the [WebNLG 2020 Challenge](https://webnlg-challenge.loria.fr/challenge_2020/) at INLG 2020 Workshop. 

<hr>

## Model Introduction
Our P2 model consists of two steps:
- Planner by relational graph convolutional networks ([Zhao et al, 2020](https://www.aclweb.org/anthology/2020.acl-main.224/))
- Pretrained Seq2Seq model: T5 ([Raffel et al., 2020](https://arxiv.org/abs/1910.10683))
![](https://i.imgur.com/hJEQzPx.png)

<hr>

## How to run

Install the requirements using

``pip install -r requirements.txt``

After that run the ``run.sh`` or `` python main.py`` for the training and the fix\_nonenglish.py is a post-process script to map the character back to the original non-english one.

Our model output on WebNLG 2020 test set is available at [output.txt](output.txt).




