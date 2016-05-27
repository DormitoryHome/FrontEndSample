# FrontEndSample
前端代码组件的目录模型，可用于快速构建前端组件
默认采用UTF8

# 目录含义
css         用于存放组件的所有CSS文件(包括组件间公用的和自定义的)
js          用于存放组件的所有js文件(包括组件间公用的和自定义的，有可能直接把数据写到js文件中，这部分不在这里面)
img         用于存放组件自身所必需的图片
resource    用于存放组件可以使用的数据文件（js，图片等文件）
share       用于存放多个组件公用的任何文件（但是这个项目中该文件不许添加代码）

# 这样做的原因
1.组件化的管理基本可以避免组件间互相干扰
2.目录一致在合并项目的时候非常好用

# 如何创建一个组件
1.将FrontEndSample拉取下来
2.将所有文件名，HTML文件中的所有Sample改为你的组件名
3.将共享文件和代码添加到组件中

# 在css/js/img文件中应该注意的地方
文件命名的时候应该遵循：
1.对于相应种类只有单个组件特有文件的，采用组件名+.js/.css/.jpg的方式命名；
2.对于相应种类有多个组件特有文件的，采用组件名_XXX+.js/.css/.jpg的方式命名；

# 如何合并组件位一个html
1.拉取所有组件
2.合并所有组件的文件夹（重复文件选择覆盖）
3.编辑HTML,将组件的引入文件声明，主体，分别添加到对应的位置（包含标记注释）
4.将共享文件和代码添加到组件中