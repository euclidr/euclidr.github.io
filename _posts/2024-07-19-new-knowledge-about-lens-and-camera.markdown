---
layout: custom_post
title:  "最近对相机和镜头的新认识"
date:   2024-07-19 16:03:53 +0800
categories: new_knowledge
tags: new_knowledge
---

这两年不是玩矿吗，手上一堆漂亮的矿矿用手机拍不出好看的照片，所以又想起了相机。因为这次要用相机的目的很明确 -- 拍近距离小物体，加上矿友们也在群里提起过他们用的镜头，我就顺藤摸瓜了解了一番。

拍近距离小物体，就是希望将那个小物体完全清晰地占满整张照片。这就涉及到物体的大小和在传感器中的像的大小的比例，这个比例在拍人和风景的时候是很少考虑的，但微距摄影中很注重镜头的这个参数。

{% include image.html url="/assets/images/2024-07-19/imaging-drawing.jpg" description="手绘成像示意图" %}

认真留意过摄影的人都知道，拍有近有远的物体的时候，画面里只有特定距离的一部分是清晰的，其它距离的物体是虚的模糊的。这是物理上的限制。如果你要整个画面都清晰，那就需要对焦 1 米，2 米，4 米 ... 无限远，每个点拍一张照片，然后用专业的图片工具将这些照片合成一张前后完全清晰的照片。这叫`景深堆叠` `Focus stacking`。

{% include image.html url="/assets/images/2024-07-19/focus-stacking.png" description="Focus stacking 图片来自: https://userguide.skylum.com/hc/en-us/articles/11541319110930-Focus-Stacking" %}

一般场景下，一两千万像素已经非常够用了，但有些地方是非常期望有高像素的（4 千万，6 千万）。比如微距摄影，拍跳蚤，如果没有显微镜，就算镜头能将物体放大两三倍成像到传感器上，也挺小。但在像素特别高的情况下，我们可以截取出比较高分辨率的图片。在要打印出巨大图片的情况下，高像素也很有必要。

还有就是镜头如何影响成像，在我看了一些学习视频后，感到真的博大精深！但我也没法说清楚，只能列举一些零碎的东西。

* 不同波长的光线通过凸透镜的折射率是不一样的，会导致不同颜色的焦点并不一样，形成球差，色差，慧差（我的理解还比较模糊）。所以镜头需要一系列的矫正设计才能让像的焦点汇聚。

<figure class="img">
    <iframe width="560" height="315" src="https://www.youtube.com/embed/EL9J3Km6wxI?si=WL7RfvCA_BzneRk8" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
    <figcaption>How Lenses Function</figcaption>
</figure>

* 但是不同镜头汇聚焦点的能力并不一样，有些汇聚得极好，那个焦点甚至小于相机传感器的一个像素（请和相机传感器像素数联系起来），这样照片就能极清晰，瓶颈落在了传感器。

最后，我还发现了一些人用光学仿真的方式去评估镜头设计的好坏，他们根据公开的镜头设计专利，将数据设置到专业的光学仿真软件里就可以知道这个镜头设计的锐度如何，畸变怎样。也是从他们的相关视频我才知道有些镜头的成像是远远超越相机传感器的测量范围的。

<figure class="img">
    <iframe width="560" height="315" src="//player.bilibili.com/player.html?isOutside=true&aid=1955969874&bvid=BV1Xy411q7PB&cid=1590044124&p=1" scrolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true"></iframe>
    <figcaption>Anvcor 的相关镜头仿真视频：https://space.bilibili.com/364758776</figcaption>
</figure>
