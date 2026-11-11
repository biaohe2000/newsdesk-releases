# NewsDesk

NewsDesk is a Windows desktop app that builds a ten-story news digest from international and Chinese news feeds,
in English and Chinese. A language model that you connect with your own API key ranks the stories, writes the
summaries and, on request, a full report on a story from the outlets' articles. The app learns your interests from
the 1-5 star ratings you give.

NewsDesk 是一款 Windows 桌面应用：从国际和中文新闻源中选出十条要闻，提供中英文两种语言。排序、摘要以及按需生成的完整报道由你自己接入的大模型（需自备 API 密钥）完成；应用会根据你的 1-5 星评分学习你的兴趣。

This repository holds the installers only. 本仓库只存放安装包。

## Download / 下载

Open the [latest release](https://github.com/biaohe2000/newsdesk-releases/releases/latest) and take one of:

| File | Use |
|---|---|
| `NewsDesk-x.y.z-setup.exe` | Setup wizard. Installs for the current user, no administrator rights needed. Recommended: this version can update itself. 安装向导（推荐，可在应用内更新）。 |
| `NewsDesk-x.y.z-portable-win64.zip` | Unzip anywhere and run `NewsDesk.exe`. Updates are downloaded by hand. 免安装版，更新需手动下载。 |
| `SHA256SUMS.txt` | SHA-256 checksums of the two files above. 上述文件的校验值。 |

Requirements: Windows 10 or 11, 64-bit, and an API key from a supported model provider.

The installers are not code-signed. Windows SmartScreen may show "Windows protected your PC"; choose **More info**,
then **Run anyway**. Security software on managed computers may block unsigned programs; in that case ask your IT
administrator rather than switching protection off.

安装包没有代码签名。Windows SmartScreen 可能提示“Windows 已保护你的电脑”，请点击“更多信息”→“仍要运行”。

## Updates / 更新

At start-up NewsDesk asks this repository whether a newer release exists and shows a notice if so. Nothing is
installed without your click, and the check can be switched off in Settings. The request goes to GitHub and
contains no personal data or API keys. Before running a downloaded installer, the app compares its SHA-256 checksum
with the one published here.

启动时，NewsDesk 会向本仓库查询是否有新版本，如有则显示提示；未经你点击不会安装，可在“设置”中关闭检查。请求发送至 GitHub，不包含个人数据或 API 密钥。运行下载的安装包之前，应用会核对其 SHA-256 校验值。

## Licences / 许可

NewsDesk includes open-source components; see [THIRD-PARTY-NOTICES.md](THIRD-PARTY-NOTICES.md).
News photos shown in the app are loaded from the publishers and remain their property.
