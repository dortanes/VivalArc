## 🗓️ 2024.11.03 | v1.1.0
Vivaldi 最近更新了 7.0 版本。变化还挺大的，比较明显的是 UI 的几个改动——图标更加精致、UI也变得更现代了一些，还有就是侧边栏选中的Tab的投影变得更加细腻。这个改动非常推荐大家升级，因为这个版本也使得 VivalArc 变得更加好看了。幸运的是，Vivaldi 的大版本升级，并没有带来 VivalArc 的任何问题。不过尽管如此，这次更新还是想解决一下 Github Issues 积累的几个问题。这些更新的列表如下：

1. 用户反馈 Footer 无论如何设置都看不到了，于是新版本的 VivalArc 不隐藏这个 Footer 了。（当然，你还是可以在设置中，把它隐藏）[#28](https://github.com/tovifun/VivalArc/issues/28)@IamMiao
2. 用户反馈的弹出是的页面，无法拖拽顶部的地址栏，新版本中，加入了 @Zettry 提供的，在地址栏加入拖拽的功能 [#30](https://github.com/tovifun/VivalArc/issues/30)
3. 在标签栏超过1屏出现滚动条的时候，之前我是隐藏了滚动条的，这样导致标签栏宽度无法缩小到图标的宽度。所以还是先放出来滚动条，滚动条有点影响美观，目前只能等官方优化滚动条样式，或者是后续有方法再来优化 [#31](https://github.com/tovifun/VivalArc/issues/31)
4. 也是本次更新最重要的变化(同时也是最多用户反馈的)，自动隐藏的 Tabbar。此方法还是来自 @Zettry [#21](https://github.com/tovifun/VivalArc/issues/21) [#29](https://github.com/tovifun/VivalArc/issues/29)
   1. 不过目前感觉还不是特别完美（后续如果继续优化之后变得稳定，会考虑作为默认样式），所以我还是新开了一个文件作为 VivalArc 的一个变体，如果你想体验自动隐藏的标签栏，可以选择使用（位于根目录/vivalarc-autobab）。

## 🗓️ 2024.08.17 | v1.0.4
### 1. 针对 Vivaldi 6.9 的优化
Vivaldi Snapshot 6.9（Vivaldi 的 Beta 版）最近发布了更新，这次更新引发了 VivalArc 的一个小问题——侧边栏的背景多了一层半透明效果 #24。此次优化的重点是解决这个问题。

### 2. 如何使用 VivalArc 的不同版本
有些用户询问如何使用带有标题栏的样式 #26。实际上，我已经设置了几个不同版本的变体，用户可以根据自己的喜好选择使用。详细信息请参阅：[如何使用 Vivaldi Arc 的不同版本](./vivalarc-variants-cn.md)。

### 3. Reflect New Tab 主题
最近，我发现了一个名为 [Reflect New Tab](https://chromewebstore.google.com/detail/reflect-new-tab/jnhdkfampckckkmbanadkkjlcaemdkob) 的新标签页插件，其渐变背景非常美观。于是，我将这个插件的背景图制作成了 [Vivaldi 的主题](./curated-themes-cn.md)。效果出乎意料地好，让 VivalArc 的外观焕然一新，尤其是粉色主题，我个人非常喜欢。强烈推荐大家试试。

## 🗓️ 2024.06.29 | v1.0.3
1. 这个版本主要优化 Vivaldi 6.8 更新之后的一个小问题——“[Issue#20左侧标签栏后，工作区下的分割线与第一个标签页有重合](https://github.com/tovifun/VivalArc/issues/20)”。（感谢 @NextEcho 细心提供 CSS，虽然最后我采取的方法和他的不完全一致
2. 在之前的版本里面，我为了模仿 Arc 的样式，做了几个渐变的 Vivaldi 主题放在了项目文件里供大家使用。然后我前几天去逛了一下 Vivald Community 的 Themes 专区，发现上面就有很多合适的主题。我就在想，我何必舍近求远自己自制主题，于是我在 Community 尝试了一些热门主题，并挑选了几个我觉得合适的主题提供大家直接使用。使用的方式很简单：
   1. 打开[推荐的主题链接](./curated-themes-cn.md)
   2. 点击主题名字跳转到主题页面
   3. 点击主题下方的安装按钮

## 🗓️ 2024.05.12 | v1.0.2
- 这一版本的VivalArc主要针对 于Vivaldi6.7 进行以下两个方面的优化：
  - macOS 左上角的的窗口按钮不能够自定义样式了，于是造成了窗口按钮对 Tabbar 的元素的遮挡
  - 新建标签页的「添加按钮」移动到了窗口的最下方

## 🗓️ 2024.03.30
- 优化顶部的标签栏的按钮大小

## 🗓️ 2023.11.09
- 增加 Tabbar 左右两边的间隙（感谢B站用户 `@godknows1` 和 `@&nbsp;&nbsp;` 提出这个修改建议。
- Tabbar 默认可以拖动（如果不想要拖动，可以在 `main_arc.css` 里将 `.tabbar-wrapper` 改为  `no-drag`
- 弹出式的设置页，现在有正常的标题栏（之前版本关闭按钮很小，感谢B站用户 `@Night子龙`
- 增加了两个主题， `theme-gradientGreenLight` 和 `theme-gradientPinkLight`
- 目前还有一个比较想要修改的是 Tabbar，目前还是稍微有点粗糙，后面的版本应该会专门优化这个

## 🗓️ 2023.09.17
- 本次更新了许多内容，我检查了每一行样式，将样式变得更加细腻
- 主要更新有：
  - 网页区域投影优化
  - Panel 优化，在各种配置下都有比较一致的样式
  - 统一了 Tabbar 和 Menubar 的颜色
- 对于想要自定义的朋友，我本来是打算出个视频来演示一下的，不过视频还没录好。可以关注一下我的 [📺Bilibili](https://www.bilibili.com/video/BV1fe4y1a7WQ)，演示视频做好的之后，我会第一时间在上面发布。目前来说，你可以打开 css/main.css 进行一些额外的配置，简单的说明如下：
  - `--window-border` 可以设置四周边框的粗细，建议设置尺寸为 4px ~ 16px (如果设置为0，就是无边框啦)
  - `--window-button-opacity` 可以设置 Windows 用户顶部右上角三个按钮的透明度，默认我设置为了0.3。可以设置的范围是 0~1，设置得高一些按钮会变得更加明显，如果设置为0.1左右，就几乎是不可见的，不过鼠标悬停还是可以看到的，如果想要一个更加简洁的header，则可以设置到0.1以下
  - 对于觉得顶部header的拖拽区域太小的朋友，可以将 `--window-header` 设置得高一些，或者使用下一个方式
  - tabbar-wrapper 的 `webkit-app-region` 的 nodrag 改为 drag，整个tabbar 就可以设置为可拖拽，不过这个之前有用户反馈这个区域的拖拽会造成对左侧 panel 区域的污染（右侧panel应该就问题不大，我自己也是将panel设置为右侧的），如果有朋友测试有问题的可以反馈一下
  - 需要注意的是，如果将 tabbar 区域变为可拖拽，tabbar 区域的双击新建 Tab 的功能就失效了，可以将上方的 display new tab button 注释掉，tabbar区域就会有一个新建tab的按钮
- **注意：修改 CSS 之后需要重启浏览器生效**

 ![Annotation](./images/annotate-config.png)

## 🗓️ 2023.07.23
- Windows上好几个小伙伴反馈看不到那三个窗口操作按钮，表示非常别扭，于是这次还是加了回去。（感谢B站的 @吅子 同学，他给我提供了这一块的CSS参考。
- Mac上左上角的三个按钮也加了回来，不过为了美观做了灰色弱化显示，鼠标悬停时才是彩色的
- 主要就是这两个，还有一些别的小更新就不说了

## 🗓️ 2023.03.12
距离第一次发布这个Vivaldi配置已经过了半年多，这次更新修复了几个大家提到比较多的问题，包括：
- 全屏时隐藏四周的边框；
- 显示了标题栏，左上角的三个按钮常驻了（这个最多人反馈说找不到；
- 去除了Tab bar的拖拽（之前开启拖拽导致了很多意想不到的bug；
- 简化了样式表
    - 之前的CSS样式为了尽可能接进Arc的外观而自订了太多，这样导致Vivaldi更新时，会有些样式失效。所以这次定了一个原则，不一昧追求样式完美，而是尽可能使用用少的CSS ；

## 🗓️ 2022.08.28 起因：为什么做这个

大概说一下背景，我主力使用 Vivaldi 浏览器应该有一年，前段时间体验了还在内测中的 Arc 浏览器，差不多两个星期。这两个星期的 Arc 使用体验确实挺好的，交互很符合直觉，UI也非常的好看。

不过最后还是换回去了 Vivaldi，主要原因是在使用Arc 的过程中，它崩溃了几次。

后来了解到 Vivaldi 居然还可以使用 CSS 自定义 UI ，于是尝试了一下，最后就有了这个网页所介绍的配置。

虽然最后的效果比不上 Arc 的 UI 和细节，但是这套配置体验下来，我觉得能够大致还原 Arc 的使用体验。所以想将这套配置分享给大家，如果你还在等待 Arc 的测试，或者因为 Arc 过于占内存，想试试别的选择，那么可以尝试使用一下我的这个配置。