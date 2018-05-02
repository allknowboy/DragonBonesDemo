# DragonBonesPro的动画编辑

> 使用龙骨开发的骨骼动画在cocoscretor中的效果

![](http://onb8jc081.bkt.clouddn.com/18-5-2/36568931.jpg)

### 图片资源

- 我们需要狗狗的身体
- 狗狗左边的翅膀
- 狗狗右边的翅膀(这个编辑器无法镜像 还是我没找到....)

![](http://onb8jc081.bkt.clouddn.com/18-5-2/59359394.jpg)


### 导入图片

- 直接放到项目的library目录下会自动刷新的

![](http://onb8jc081.bkt.clouddn.com/18-5-2/24094887.jpg)


### 拼凑主体

- 中间的是主体的骨骼
- 左右两边的分别为子骨骼 用于再添加翅膀的子骨骼
- 参考线是必须要有的 后期调动画定位十分方便  方法和ps一样

![](http://onb8jc081.bkt.clouddn.com/18-5-2/64564943.jpg)

![](http://onb8jc081.bkt.clouddn.com/18-5-2/63562202.jpg)

### 加入右边翅膀

- 使用一根骨骼作为翅膀的主骨骼
- 然后加入额外一根骨骼作为收缩翅膀的骨骼 **下面不挂载图槽**


![](http://onb8jc081.bkt.clouddn.com/18-5-2/61173653.jpg)

![](http://onb8jc081.bkt.clouddn.com/18-5-2/39509542.jpg)

![](http://onb8jc081.bkt.clouddn.com/18-5-2/99859774.jpg)


### 编辑翅膀的网格

- 选中翅膀的图槽 可以在编辑器的属性面板中编辑网格
- 勾选上网格
- 点击**添加绑定骨骼**加入两根翅膀的骨骼
- 点击**编辑网格**编辑翅膀的网格形状 一般点选自动就行

![](http://onb8jc081.bkt.clouddn.com/18-5-2/44740534.jpg)

![](http://onb8jc081.bkt.clouddn.com/18-5-2/9254355.jpg)

![](http://onb8jc081.bkt.clouddn.com/18-5-2/46296496.jpg)

### 编辑翅膀的骨骼权重

- 自动权重基本可以放弃了 没一次可以的...
- 点击一般在右上角的功能bar的权重工具
- 之前编辑的网格点开始有了颜色区分
- 点击网格点编辑各骨骼占的权重 就是骨骼移动网格的同步率

![](http://onb8jc081.bkt.clouddn.com/18-5-2/76211612.jpg)

![](http://onb8jc081.bkt.clouddn.com/18-5-2/10240690.jpg)

![](http://onb8jc081.bkt.clouddn.com/18-5-2/82296474.jpg)



==左侧翅膀就重复下右侧翅膀的工序就好了，还是吐槽没有翻转，非要干两次。==

### 编辑一个飞行的动画

#### 加关键帧的方法

- 一种是圈中的那个自动加入 你在那一帧操作 自动记录为关键帧
- 另一种是提示修改的属性 手动加入变化的关键帧
- **还是自动挡好**

![](http://onb8jc081.bkt.clouddn.com/18-5-2/81339590.jpg)

#### 编辑翅膀拍下的动作

- 自动关键帧是你要有改变才会记录 所以0帧的时间点是没有记录的
- 我们先编辑一个改变后的动作
- 此时翅膀张开到最大程度

![](http://onb8jc081.bkt.clouddn.com/18-5-2/97599480.jpg)

![](http://onb8jc081.bkt.clouddn.com/18-5-2/10143760.jpg)

#### 编辑翅膀收起的动作

- 这样我们就编辑好了第10帧和16帧
- **然后复制16帧的内容到第0帧**

![](http://onb8jc081.bkt.clouddn.com/18-5-2/39814362.jpg)

#### 编辑动画的曲线

- 点击前面的关键帧 编辑接下来的运动曲线

![](http://onb8jc081.bkt.clouddn.com/18-5-2/84725741.jpg)


#### 动画的导出

- cocoscreator支持的是4.5 (可能之后会更新运行库)
- json格式就好了

![](http://onb8jc081.bkt.clouddn.com/18-5-2/90401124.jpg)


![](http://onb8jc081.bkt.clouddn.com/18-5-2/6577244.jpg)


#### 在CocosCreator中使用

- 加入一个空节点
- 加入dragonbone的组件
- 将导出资源拖入
- 设置动画为fly

![](http://onb8jc081.bkt.clouddn.com/18-5-2/91196142.jpg)

![](http://onb8jc081.bkt.clouddn.com/18-5-2/30668999.jpg)


### 项目地址

[https://github.com/SeaPlanet/DragonBonesDemo](https://github.com/SeaPlanet/DragonBonesDemo)


### 博客地址

[https://allknowboy.com/posts/a79a675b/](https://allknowboy.com/posts/a79a675b/)