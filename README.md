# RIME个人配置

## 说明

本项目基于RIME、薄荷输入法二次配置

------

## 安装

以下教程，适用于Linux、macOS和Windows（Xp~）

1. 安装[Rime输入法](https://rime.im/)并注销或重启电脑；
2. 下载本仓库所有配置文件到本地rime配置文件；
3. 重新部署Rime
4. 开始使用
5. 根据自己习惯，进行二次修改

## 输入法切换

你可以在安装后，使用『Ctrl』+『~』进行切换。（默认激活的是『薄荷拼音-全拼输入』）

## 配置文件说明

- `default.custom.yaml` 设置输入法、如何切换输入法、翻页等
- `squirrel.custom.yaml` 鼠须管( Mac 版本 )设置哪些软件默认英文输入，输入法皮肤等；
- `rime_mint.custom.yaml` 设置rime_mint的具体配置
- `rime_mint.custom.dict.yaml` 设置词典配置
- `custom_phrase.txt` 设置自定义短语

> `custom_phrase.txt` 自定义短语太个人，在`.gitignore`中忽略了，请自定义创建

### custom_phrase.txt 示例

> 存放位置：RIME根目录

```txt
# Rime table
# coding: utf-8
# 自定义文本
# 1. 一定要用<tab>分割
# 2. 尽量用单词，为了避免级联地狱，关闭了首字母优先级，所以首字母不一定有别的高，容易不出现
# 此行之后不能写注释

啥	wtf
在开会，等下找你	meet
😂😂😂	xs
你是人吗	fuck
做个人吧	cao
```

------

## 集成
- 集成了 oh-my-rime，[文档](https://www.mintimate.cc)
  - 默认输入法：薄荷拼音-全拼输入
- 集成了 [雾凇拼音](https://github.com/iDvel/rime-ice)

## Tips

本地rime配置文件默认地址，如下

- Windows
  - Weasel: `%APPDATA%\Rime`
- Mac OS X
  - Squirrel: `~/Library/Rime`
- Linux
  - iBus:` ~/.config/ibus/rime`
  - Fcitx5: `~/.local/share/fcitx5/rime`
- Fctix5 Android(小企鹅入法): `/storage/emulated/0/Android/data/org.fcitx.fcitx5.android/files/data/rime/`

本地rime日志文件默认地址如下：

- Windows
  - Weasel: `%TEMP%`
- Mac OS X
  - Squirrel: `$TMPDIR`
- Linux
  - iBus:` /tmp`


## 词库定制以及更新

本仓库的词库目录[dicts](dicts)，主要有：
- [雾凇拼音词库](https://github.com/iDvel/rime-ice)
- [98五笔词库](https://github.com/yanhuacuo/98wubi-tables)

详细说明：
```txt
dicts
├── custom_simple.dict.yaml    # 自定义词库（建议自己添加的词库可以放这里）
├── other_emoji.dict.yaml      # emoji 词库
├── other_kaomoji.dict.yaml    # 颜文字词库（按vv进行激活）
├── rime_ice.41448.dict.yaml   # 雾凇词库（GitHub action自动更新）
├── rime_ice.8105.dict.yaml    # 雾凇词库（GitHub action自动更新）
├── rime_ice.base.dict.yaml    # 雾凇词库（GitHub action自动更新）
├── rime_ice.ext.dict.yaml     # 雾凇词库（GitHub action自动更新）
├── rime_ice.cn_en.txt         # 雾凇词库（GitHub action自动更新）
├── rime_ice.en.dict.yaml      # 雾凇词库（GitHub action自动更新）
├── rime_ice.en_ext.dict.yaml  # 雾凇词库（GitHub action自动更新）
├── rime_ice.others.dict.yaml  # 雾凇词库（GitHub action自动更新）
├── terra_pinyin_base.dict.yaml     # 地球拼音自带词库
├── terra_pinyin_ext.dict.yaml      # 地球拼音自带词库
├── terra_rime_ice.base.dict.yaml   # 基于Python脚本自动转换雾凇并Action自动更新
└── wubi98_base.dict.yaml           # 五笔基础词库
```

后续更新词库；可以下载本仓库`dicts`内的文件，除了`custom_simple.dict.yaml`的文件，其他都进行覆盖替换即可。

如果想自己扩展词库，可以在输入法的字典配置文件内进行导入

------

## 参考/致谢

1. [Rime-RimeWithSchemata](https://github.com/rime/home/wiki/RimeWithSchemata)
2. [Rime/小狼豪/鼠须管 输入法配置记](https://chenhe.me/post/oh-my-rime)
3. [rime-setting](https://github.com/Iorest/rime-setting)
4. [雾凇拼音 | 长期维护的简体词库](https://github.com/iDvel/rime-ice)
5. [rime-radical-pinyin | Rime 部件拆字输入方案（全拼双拼）](https://github.com/mirtlecn/rime-radical-pinyin)
6. [oh-my-rime](https://github.com/Mintimate/oh-my-rime)
