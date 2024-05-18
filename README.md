## 自用的Rime方案
主要用的是`oh-my-rime`（`薄荷输入法`）的方案，根据自己需要只保留了`小鹤双拼-薄荷定制 `，删除了其他的各种方案。
另外在`薄荷输入法`的方案上，加上了`小鹤音形`，小鹤音形来自 `凇鹤拼音` 


## 参考
- [薄荷输入法](https://www.mintimate.cc/zh/)
- [凇鹤拼音](https://github.com/kchen0x/rime-crane/tree/main)
- [雾凇拼音 | 长期维护的简体词库](https://github.com/iDvel/rime-ice)
- [Rime 官方定制指南](https://github.com/rime/home/wiki/CustomizationGuide)

## 本输入方案内包含 
- 小鹤双拼-薄荷定制: 基于小鹤双拼，添加定制内容。支持输入音形(形码)作为辅助输入；
- 凇鹤拼音-小鹤音形: 纯小鹤音形；

安装后可以使用『Ctrl』+『~』进行切换。

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



## 凇鹤拼音维护词库
```
- 小鹤音形的主码表：文件 "xhup.dict.yaml"，其中按需加载的码表分别如下：
  - "xhup_dicts/xhup.user.top"          # 用户置顶码表：可以按需自行添加置顶词汇
  - "xhup_dicts/xhup.primary"           # -0- 首选字词
  - "xhup_dicts/xhup.secondary"         # 1.1 次选字词
  - "xhup_dicts/xhup.whimsicality"      # 1.1 随心码
  - "xhup_dicts/xhup.fast.symbols"      # 1.2 快符
  - "xhup_dicts/xhup.single.code"       # 2.1 一简词：可以根据自己的情况选择使用一简词还是二重简码
  - "xhup_dicts/xhup.off-table"         # 2.2 表外字
  - "xhup_dicts/xhup.full.code.words"   # 2.3 全码词
  # - "xhup_dicts/xhup.symbols"           # 符号
  # - "xhup_dicts/xhup.full.code.chars"   # 全码字：在四码时出现在候选词中，不熟练时可开启增加拆词熟练度（默认关闭），应该尽量练习有简打简。
  - "xhup_dicts/xhup.user"              # 用户码表
  - "xhup_dicts/xhup.short.hints"       # 简码提示
  # - "xhup_dicts/xhup.secondary.simple"   # 二重简码：默认开启的是一简词
```  

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