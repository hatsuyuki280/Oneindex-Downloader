# 这是一个用于对已知 Oneindex 站点进行全站下载的实用工具，目前仍然没有什么头绪就是了。。。

暂定目录结构大概长这样。。。

Oneindex-Downloader
| - install.sh  ## 用于安装所需的环境。。比如curl或者其他什么
| - onedownloader.sh  ## 用于实现基本输入输出，接收终端传入的参数，基本等于启动器
| - getdir.[py|sh]  ## 用于获取指定url下的每一层文件夹的所有文件。。也许到最后也不会出现这个文件。。。直接整合进onedownloader.sh也说不定。。。。

## 使用方法

目前暂定的是。。。
``` onedownloader [https://站点地址/?/目录] ```
然后就会自动把指定目录下的所有文件全部下载到当前文件夹。。。

TO DO ：

先随便写点简单的shell程序用来安装必要的文件和接收命令。。。（ install.sh onedownloader.sh ）（虽然感觉install.sh可有可无就是了）
实现简单的目录爬取。。。（getdir.sh/getdir.py ...并没有确定到底用py还是直接用shell script。。。）
支持按文件扩展名的筛选。。
自动丢给下载程序。。。比如aria2c。。。。比如wget。。。。比如其他什么。。。然后自动后台下载
支持下载到自定义目录。。。

咱也不知道还有什么需要的东西了。。。。。一步步看好了。。。。。