# 示例

以将图片转换为 PNG 格式为例

## 最简实现

```text
1 打开共享表单，选择图像
2 转换图像，设置为 PNG
3 保存到相簿
```

最简实现的优点：

快速

最简实现的缺点：

无法从其他位置（如快捷指令 App 内、小组件）调用快捷指令功能
无法选择保存位置

## 风格化实现

```text
1 打开共享表单，选择图像
2.1 如果-判断共享表单是否传入了图像
2.2 否则-如果没有传入图像，则弹出菜单
3.1 菜单-从文件选择-获取文件
3.2 菜单-从照片中选择-选择照片
4 从菜单结果获取图像
5 转换图像，设置为 PNG
6 将变量 png 设为转换后的图像
7.1 菜单-保存到照片
7.2 菜单-保存到文件

```

风格化实现的优点：

可以从多个位置启动并调用快捷指令功能
可以选择存储位置

风格化实现缺点：

步骤增多，使用判断和选择导致运行时间的增加

