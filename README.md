# Bilibili-Auto-Seek
自定义B站电视剧跳过开头。根据视频标题自动跳转到指定时间位置。

## 特性
- 根据视频标题自动跳转到指定时间位置。
- 提供确认弹窗，允许用户选择是否跳转。
- 可以自定义不同的电视剧跳转位置。

## 支持的网站
- [哔哩哔哩](https://www.bilibili.com/bangumi/play/*)

## 安装说明
1. 安装油猴（Tampermonkey）浏览器扩展。
2. 点击油猴扩展图标，选择“创建新脚本”。
3. 将本仓库中的脚本代码复制并粘贴到新脚本中。
4. 保存脚本，油猴会自动安装并启用该脚本。

## 使用说明
1. 打开哔哩哔哩网站并播放支持的视频。
2. 当视频加载完成后，会弹出一个确认框，询问是否跳转到指定的时间位置。
3. 选择“是”进行跳转，选择“否”则不进行跳转。
4. 自定义跳转位置

如果您希望为其他视频设置自定义的跳转位置，可以编辑脚本中的 `videoTitleToTimeMap` 对象。例如：

```javascript
// 视频标题与跳转时间的映射表
const videoTitleToTimeMap = {
    '铠甲勇士刑天': 3 * 60, // 3分钟
    '三国演义': 13 * 60, // 13分钟
    '新视频标题': 5 * 60 // 5分钟
};
```
在这个示例中，您可以添加新的视频标题和对应的跳转时间（以秒为单位）。保存脚本后，新设置将生效。

## 如何贡献
1. Fork 本仓库。
2. 创建您的特性分支 (`git checkout -b feature/AmazingFeature`)。
3. 提交您的更改 (`git commit -m 'Add some AmazingFeature'`)。
4. 将更改推送到分支 (`git push origin feature/AmazingFeature`)。
5. 创建一个新的 Pull Request。

## 许可证
本项目采用 MIT 许可证，详情请参阅 [LICENSE](LICENSE) 文件。

## 联系
如果您有任何问题或建议，请通过 [GitHub Issues](https://github.com/) 联系我。
