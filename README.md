# PCA-SVM-for-LFW
. Labeled Faces in the Wild (LFW)是 University of Massachusetts 从网络上搜集的自然
条件下的人脸图像数据库，其中包括 13233 张人脸图像，5749 个不同的人，其中
1680 人有 2 张以上的脸部图像。 针对其中一个结果预处理过的数据集
lfw_funneled，提取了其中每人有 70 张以上照片的一个子集，包含 7 个人的 1288
张人脸），Scikit-learn 网站给出了采用主成分分析降维之后通过支持向量机 SVM
分类人脸的方法代码：http://scikit-learn.org/stable/auto_examples/applications/plot_face_recognition.html#sphx-glr-auto-examples-applications-plot-face-recognition-py

#### 编写主成分分析PCA函数my_PCA
替换Scikit-learn网站代码中的PCA函数。my_PCA分别采用协方差矩阵求特征值，和奇异值分解(SVD)两种方法，比较它们的计算速度。

#### 通过SVM进行分类
