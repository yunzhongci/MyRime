## 自用的Rime方案
用的是`oh-my-rime`（`薄荷输入法`）的方案，根据自己需要只保留了自己需要的方案，删除了其他的各种方案。



## 参考
- [薄荷输入法](https://www.mintimate.cc/zh/)
- [Rime 官方定制指南](https://github.com/rime/home/wiki/CustomizationGuide)

## 本输入方案内包含：

- 薄荷拼音-全拼输入: 全拼输入，适合的人群最多，所以也是默认的输入；
- 小鹤双拼-薄荷定制: 基于小鹤双拼，添加定制内容。支持输入音形(形码)、自然码辅助码或墨奇辅助码作为辅助输入；
- 薄荷拼音-小鹤混输: 全拼输入的同时，支持小鹤双拼；
  
安装后可以使用『Ctrl』+『~』进行切换。

## lua脚本
- 支持输入R后输入数字，进行数字转换，
- 支持输入week、date、time和lunar分别输入当前星期、日期、时间以及农历日期，以词定字

## 安装

以下教程，适用于Linux、macOS和Windows（Xp~）

1. 安装[Rime输入法](https://rime.im/)并注销或重启电脑；
2. 下载本仓库所有配置文件到本地rime配置文件；
3. 重新部署Rime
4. 开始使用
5. 根据自己习惯，进行二次修改

## 配置文件说明

- `default.yaml` 设置输入法、如何切换输入法、翻页等；建议自行创建`default.custom.yaml`来覆写薄荷配置的`default.yaml`.
- `squirrel.yaml` 鼠须管( Mac 版本 )设置哪些软件默认英文输入，输入法皮肤等；如需自定义，建议自行创建`squirrel.custom.yaml`来覆写。 
- `weasel.yaml` 小狼毫( Win 版本 )设置哪些软件默认英文输入，输入法皮肤等；如需自定义，建议自行创建`weasel.custom.yaml`来覆写。

## 薄荷输入法维护词库
可以下载[oh-my-rime仓库](https://github.com/Mintimate/oh-my-rime/)dicts内的文件，除了custom_simple.dict.yaml的文件，其他都进行覆盖替换即可。


## 软链接安装（推荐）

克隆本仓库到本地（不要删除）。

`~/Code/MyRime`  为我的仓库路径

```
rm -rf ~/Library/Rime && ln -s ~/Code/MyRime ~/Library/Rime

```
## 卸载rime

```
rm -rf "/Library/Input Methods/Squirrel.app" 
rm -rf ~/Library/Rime
```