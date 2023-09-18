# Code for 'Introduction to transfer learning' book 《迁移学习导论》(第二版)代码

This folder contains the codes for the book [Introduction to Transfer Learning: Algorithms and Practice](http://jd92.wang/tlbook). [迁移学习导论](http://jd92.wang/tlbook).

Links for the Chinese book (2nd edition) can be found at: [`links.md`](./links.md). 中文第二版书中的链接请见[这里](./links.md)。

## Dataset

1. For algorithm chapters (chapters 1 ~ 11), we mainly use Office-31 dataset, download [HERE](https://github.com/jindongwang/transferlearning/tree/master/data#office-31):
- For non-deep learning methods (chapters 1~7), we use ResNet-50 pre-trained features. Thus, download the ResNet-50 features.
- For deep learning methods (chapters 8~11), we use Office-31 original dataset. Thus, download the raw images.

2. For application chapters (chapters 15~19), the datasets download link can be found at respective chapters.

## Requirements

The following is a basic environment to run most experiments. No special tricky packages are needed. Just `pip install -r requirements.txt`.
- Python 3.x
- scikit-learn
- numpy
- scipy
- torch
- torchvision

## Citation

If you find the code or the book helpful, please consider citing our book as:

```
@book{tlbook,
 author = {Wang, Jindong and Chen, Yiqiang},
 title = {Introduction to Transfer Learning: Algorithms and Practice},
 year = {2023},
 url = {jd92.wang/tlbook},
 publisher = {Springer Nature}
}

@book{tlbookchinese,
 author = {王晋东 and 陈益强},
 title = {迁移学习导论},
 year = {2021},
 url = {jd92.wang/tlbook}
}
```

## Recommended Repo
My unified transfer learning repo (and **the most popular** transfer learning repo on Github) has everything you need for transfer learning: https://github.com/jindongwang/transferlearning. Including: Papers, codes, datasets, benchmarks, applications etc. 


## Tips

迁移学习的核心是，找到源领域和目标领域之间的相似性，举一个杨强教授经常举的例子来说明：我们都知道在中国大陆开车时，驾驶员坐在左边，靠马路右侧行驶。这是基本的规则。
然而，如果在英国、香港等地区开车，驾驶员是坐在右边，需要靠马路左侧行驶。那么，如果我们从中国大陆到了香港，应该如何快速地适应 他们的开车方式呢？诀窍就是找到这里的不变量：不论在哪个地区，驾驶员都是紧靠马路中间。这就是我们这个开车问题中的不变量。 找到相似性 (不变量)，是进行迁移学习的核心。
