# common_command_in_python
some useful hint

1.  read image and show it:

import matplotlib.pyplot as plt # plt 用于显示图片
import matplotlib.image as mpimg # mpimg 用于读取图片
import numpy as np

### load
img = mpimg.imread('cat.jpg') 
# 此时 img 就已经是一个 np.array 了，可以对它进行任意处理
# height, width, channel=(360, 480, 3)
h,w,c = img.shape 

# show
plt.imshow(img) # 显示图片
plt.axis('off') # 不显示坐标轴
plt.show()

# save
# 适用于保存任何 matplotlib 画出的图像，相当于一个 screencapture
plt.savefig('fig_cat.png')

