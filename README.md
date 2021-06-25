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
### Loss chart
![Biểu đồ Loss của model trong quá trình train 5000 epoches](./report/loss.png)

### Test

#### Test với pre-train
Với mỗi style ảnh (Cezanne, Monet, Ukio-e, Van Gogh), nhóm đem test với 4 ảnh và thu được kết quả như sau:

![](./report/test_pretrain.png)

#### Test với model tự custom

<h4 align="center"><em>Danh sách các ảnh Input</em></h4>
<div align="center">
  <span>
    <img alt="Ảnh test 1" title="Ảnh test 1" src="./report/test1.jpg" height="175px" />
  </span>
  <span>
    <img alt="Ảnh test 2" title="Ảnh test 2" src="./report/test2.jpg" height="175px" />
  </span>
</div>

<div align="center">
  <span>
    <img alt="Ảnh test 3" title="Ảnh test 3" src="./report/test3.jpg" height="175px" />
  </span>
  <span>
    <img alt="Ảnh test 4" title="Ảnh test 4" src="./report/test4.jpg" height="175px" />
  </span>
</div>

Cứ 50 epoches trong tổng số 5000 epoches, nhóm sẽ lấy ra 1 checkpoint để test. Thu được kết quả như sau:

- Kết quả Test với ảnh Test 1 ứng với các epoch 0 – 5000 (step: 50):
![](./report/test1.gif)

<div align="center">
  <span>
    <img src="./report/test1/test1.1.jpg" height="175px" />
  </span>
  <span>
    <img src="./report/test1/test1.2.jpg" height="175px" />
  </span>
  <span>
    <img src="./report/test1/test1.3.jpg" height="175px" />
  </span>
</div>
<div align="center">
  <span>
    <img src="./report/test1/test1.4.jpg" height="175px" />
  </span>
  <span>
    <img src="./report/test1/test1.5.jpg" height="175px" />
  </span>
  <span>
    <img src="./report/test1/test1.6.jpg" height="175px" />
  </span>
</div>

- Kết quả Test với ảnh Test 2 ứng với các epoch 0 – 5000 (step: 50):
![](./report/test2.gif)

<div align="center">
  <span>
    <img src="./report/test2/test2.1.jpg" height="175px" />
  </span>
  <span>
    <img src="./report/test2/test2.2.jpg" height="175px" />
  </span>
  <span>
    <img src="./report/test2/test2.3.jpg" height="175px" />
  </span>
</div>
<div align="center">
  <span>
    <img src="./report/test2/test2.4.jpg" height="175px" />
  </span>
  <span>
    <img src="./report/test2/test2.5.jpg" height="175px" />
  </span>
  <span>
    <img src="./report/test2/test2.6.jpg" height="175px" />
  </span>
</div>

- Kết quả Test với ảnh Test 3 ứng với các epoch 3000 – 4000 (step: 10):
![](./report/test3.gif)

<div align="center">
  <span>
    <img src="./report/test3/test3.1.jpg" height="175px" />
  </span>
  <span>
    <img src="./report/test3/test3.2.jpg" height="175px" />
  </span>
  <span>
    <img src="./report/test3/test3.3.jpg" height="175px" />
  </span>
</div>
<div align="center">
  <span>
    <img src="./report/test3/test3.4.jpg" height="175px" />
  </span>
  <span>
    <img src="./report/test3/test3.5.jpg" height="175px" />
  </span>
  <span>
    <img src="./report/test3/test3.6.jpg" height="175px" />
  </span>
</div>
<div align="center">
  <span>
    <img src="./report/test3/test3.7.jpg" height="175px" />
  </span>
  <span>
    <img src="./report/test3/test3.8.jpg" height="175px" />
  </span>
  <span>
    <img src="./report/test3/test3.9.jpg" height="175px" />
  </span>
</div>

- Kết quả Test với ảnh Test 4 ứng với các epoch 3000 – 4000 (step: 10):
![](./report/test4.gif)

<div align="center">
  <span>
    <img src="./report/test4/test4.1.jpg" height="175px" />
  </span>
  <span>
    <img src="./report/test4/test4.2.jpg" height="175px" />
  </span>
  <span>
    <img src="./report/test4/test4.3.jpg" height="175px" />
  </span>
</div>
<div align="center">
  <span>
    <img src="./report/test4/test4.4.jpg" height="175px" />
  </span>
  <span>
    <img src="./report/test4/test4.5.jpg" height="175px" />
  </span>
  <span>
    <img src="./report/test4/test4.6.jpg" height="175px" />
  </span>
</div>
<div align="center">
  <span>
    <img src="./report/test4/test4.7.jpg" height="175px" />
  </span>
  <span>
    <img src="./report/test4/test4.8.jpg" height="175px" />
  </span>
  <span>
    <img src="./report/test4/test4.9.jpg" height="175px" />
  </span>
</div>

## References
- [**Rahul Bhalley**](https://github.com/rahulbhalley) and [Jianlin Su](https://github.com/bojone)
- https://github.com/rahulbhalley/cyclegan-qp
