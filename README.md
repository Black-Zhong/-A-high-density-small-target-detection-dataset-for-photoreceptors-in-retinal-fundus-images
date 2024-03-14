# A-high-density-small-target-detection-dataset-for-photoreceptors-in-retinal-fundus-images
针对视网膜眼底图像中光感受器的高密度小目标检测数据集 A high-density small target detection dataset for photoreceptors in retinal fundus images

# 高密度小目标的定义
Definition of High-Density Small Objects

本数据集中“小目标”的定义：从绝对尺寸角度来看：所占区域内的像素少于80个，尺寸通常小于9×9像素，且半径小于5像素的目标；对于整幅图像的尺寸而言，如果目标的尺寸小于等于图像尺寸的0.15%，则可认为目标为小目标。

In this dataset, the definition of “small objects” is as follows: from the perspective of absolute size, the objects whose areas occupy less than 80 pixels, usually smaller than 9x9 pixels in size, and with a radius of less than 5 pixels; in terms of the entire image size, if the size of the object is less than or equal to 0.15% of the image size, it can be considered as a small object.

本数据集中“高密度”的定义：在图像中，若小目标的分布密度超过每100像素平方内2个目标；或者所有小目标中心点至其最近邻目标的中心平均距离低于10像素，则此类目标被认定为“高密度小目标”

In this dataset, “high density” is defined as: in an image, if the distribution density of small objects exceeds 2 objects per 100 square pixels; or if the average distance from the center of all small objects to the center of their nearest neighboring object is less than 10 pixels, then these objects are classified as “high-density small objects”.

# 眼底视网膜图像以及光感受器
Retinal fundus images and photoreceptors

本数据集中的图像是通过加装了海德堡高倍高清放大模组（Heidelberg high-magnification module，HMM）的共焦激光眼底镜采集得到的。
其中亮度较高的小目标点被认为是光感受器（包括视锥细胞和视杆细胞）

The images in this dataset were captured using a confocal laser ophthalmoscope equipped with a Heidelberg high-magnification module (HMM). The brighter small dots are considered to be photoreceptors, including both cone cells and rod cells.

# 数据格式
Data Format

本数据集提供多种不同格式的图片和标注文件格式。
This dataset provides images and annotation files in various formats. 

其中png+xml格式文件，可以直接通过Fiji（imageJ）结合其自带的Cell Counter插件打开使用；

the png+xml format files can be directly opened and used with Fiji (ImageJ) in combination with its built-in Cell Counter plugin;

![image](https://github.com/Black-Zhong/-A-high-density-small-target-detection-dataset-for-photoreceptors-in-retinal-fundus-images/assets/50744401/ccc5c959-5ac0-43e9-bdec-0925a03c718a)
jpg+txt格式文件，可以通过YOLOv8使用

jpg+txt format files can be utilized with YOLOv8.

![image](https://github.com/Black-Zhong/-A-high-density-small-target-detection-dataset-for-photoreceptors-in-retinal-fundus-images/assets/50744401/45afe392-dafb-4938-b2f8-db976b6d8460)

# 分度取图 数据集
Grading Sampling Dataset

这个数据集共有154张图片，采集自多名实验参与人员，且一般4-5张图片取自一名参与人员眼底图像中距离黄斑中心凹不同尺度，因此可以作为研究眼底视网膜图像中距离黄斑中心凹不同尺度距离的光感受器密度分布等问题的素材。

This dataset consists of 154 images, collected from multiple experimental participants, with typically 4-5 images taken from varying scales of distance from the fovea in the fundus images of a single participant. Therefore, it can serve as material for research on issues such as the distribution of photoreceptor density at different scale distances from the foveal center in fundus retinal images.

# 随机取图 数据集
Random Sampling Dataset

这个数据集共有286张图片，与“分度取图”数据集不同，此数据集采集图片的标准仅为图像质量。

This dataset consists of 286 images. Unlike the “Grading Sampling” dataset, the criterion for collecting images in this dataset is solely based on image quality.
