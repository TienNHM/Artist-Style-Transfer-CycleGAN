# Artist Style Transfer CycleGAN

[![GitHub contributors](https://img.shields.io/github/contributors/TienNHM/Artist-Style-Transfer-CycleGAN)](https://github.com/TienNHM/Artist-Style-Transfer-CycleGAN/graphs/contributors)
[![GitHub issues](https://img.shields.io/github/issues/TienNHM/Artist-Style-Transfer-CycleGAN?color=red)](https://github.com/TienNHM/Artist-Style-Transfer-CycleGAN/issues)
![GitHub top language](https://img.shields.io/github/languages/top/TienNHM/Artist-Style-Transfer-CycleGAN?color=cyan)
![GitHub repo size](https://img.shields.io/github/repo-size/TienNHM/Artist-Style-Transfer-CycleGAN)
![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/TienNHM/Artist-Style-Transfer-CycleGAN)
![Github total lines](https://sloc.xyz/github/TienNHM/Artist-Style-Transfer-CycleGAN)
[![GitHub commit activity](https://img.shields.io/github/commit-activity/m/TienNHM/Artist-Style-Transfer-CycleGAN?color=g)](https://github.com/TienNHM/Artist-Style-Transfer-CycleGAN/graphs/code-frequency)
![GitHub last commit](https://img.shields.io/github/last-commit/TienNHM/Artist-Style-Transfer-CycleGAN?color=yellow)
[![GitHub release (latest by date)](https://img.shields.io/github/v/release/TienNHM/Artist-Style-Transfer-CycleGAN)](https://github.com/TienNHM/Artist-Style-Transfer-CycleGAN/releases)

## Ngôn ngữ lập trình
![](https://img.icons8.com/color/48/000000/python.png)
![](https://img.icons8.com/doodle/48/000000/console--v2.png)

## Công nghệ sử dụng
<img src="https://pytorch.org/docs/stable/_static/images/logo-icon.svg" width="30px"> <img src="https://colab.research.google.com/img/colab_favicon_256px.png" width="48px">

## Project Structure
<details>
<summary>Mở rộng</summary>
```
├───assets
├───checkpoints
│   ├───ce
│   ├───mo
│   ├───uk
│   └───vg
├───datasets
│   ├───cezanne2photo
│   │   ├───testA
│   │   ├───testB
│   │   ├───trainA
│   │   │   └───A
│   │   └───trainB
│   │       └───B
│   ├───monet2photo
│   │   ├───testA
│   │   ├───testB
│   │   ├───trainA
│   │   │   └───A
│   │   └───trainB
│   │       └───B
│   ├───ukiyoe2photo
│   │   ├───testA
│   │   ├───testB
│   │   ├───trainA
│   │   │   └───A
│   │   └───trainB
│   │       └───B
│   └───vangogh2photo
│       ├───testA
│       ├───testB
│       ├───trainA
│       │   └───A
│       └───trainB
│           └───B
├───images
└───out
```
</details>

## Datasets
Download vào thư mục `datasets\`:
- [Monet](https://people.eecs.berkeley.edu/~taesung_park/CycleGAN/datasets/monet2photo.zip)
- [Cezanne](https://people.eecs.berkeley.edu/~taesung_park/CycleGAN/datasets/cezanne2photo.zip)
- [Ukiyo-e](https://people.eecs.berkeley.edu/~taesung_park/CycleGAN/datasets/ukiyoe2photo.zip)
- [Vangogh](https://people.eecs.berkeley.edu/~taesung_park/CycleGAN/datasets/vangogh2photo.zip)

Lưu ý: sau khi download và giải nén, phải sửa cấu trúc thư mục theo định dạng:
```shell
datasets
└───vangogh2photo
    ├───testA
    ├───testB
    ├───trainA
    │   └───A
    └───trainB
        └───B
```

## Results
### Input
![](./images/meow.jpg)

### Output
![](./out/output.png)

## References
- [**Rahul Bhalley**](https://github.com/rahulbhalley) and [Jianlin Su](https://github.com/bojone)
- https://github.com/rahulbhalley/cyclegan-qp
