# PHP 傀儡图创建器
## 类似 DummyImage.com


### 2014-08-08 调整

按照自己的需求进行了一些调整

- 修改了 image.php 不再判断文件格式参数，直接输出 png
- 所以也修改了 .htaccess ，重写 url 的时候，不再处理 文件格式参数
- 现在 url 和 DummyImage.com 一样了，确保在本地没有配置傀儡图工具的情况下，直接访问 DummyImage.com 能看到一模一样的图
- 不过，还缺少 text 参数


### 例子:

- `//dummyimage.com/180x290/f0f0f0/666` //本地配置的域名/尺寸/背景色/前景色

<s>
 * image.php?size=250x850&type=jpg&bg=ff8800&color=000000 <br>- 创建250像素宽，800像素高，橙色背景黑色文字的jpg图片
 * image.php?size=250 <br>- 创建宽高都是250像素黑色背景白色文字，png格式的图片
</s>