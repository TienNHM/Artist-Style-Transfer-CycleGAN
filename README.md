# Artist Style Transfer CycleGAN

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

## References
- [**Rahul Bhalley**](https://github.com/rahulbhalley) and [Jianlin Su](https://github.com/bojone)
- https://github.com/rahulbhalley/cyclegan-qp
