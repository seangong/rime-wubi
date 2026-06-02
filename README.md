# 五笔字库

> 支持五笔和拼音混输，遇到不会拆的字。直接输入拼音即可，无需按特殊键触发。同时支持拼音反查五笔。
> `squirrel.custom.yaml` 中带有多有种主题皮肤。

默认支持输入法：
- 86版五笔 + 拼音 混输
- 新世纪五笔 + 拼音 混输
- 新世纪五笔，纯五笔
- 袖珍简化字拼音

macOS 版鼠须管（可直接移植到 windows 等其它系统）：

- 支持字库：新世纪五笔，86版本五笔，86版本简入繁出，袖珍简化字拼音。
- 支持五笔和拼音混输，默认 2 码是五笔，不会触发拼音输入。防止五笔一级简码和二级简码被覆盖。
- 拼音混输超过 3 码，会自动切换到拼音输入模式，不需要特殊键触发。
- 使用 `（即 1 左侧那个键） 触发 **拼音反查五笔**。

![Xnip2026-05-29_17-11-26.jpg](https://github.com/seangong/Rime-wubi06/blob/master/doc/Xnip2026-05-29_17-11-26.jpg)

![Xnip2026-05-29_17-11-47.jpg](https://github.com/seangong/Rime-wubi06/blob/master/doc/Xnip2026-05-29_17-11-47.jpg)

- 使用 Ctrl + `（即 1 左侧那个键） 触发不同输入法切换选择菜单。

![Xnip2026-05-29_17-10-11.jpg](https://github.com/seangong/Rime-wubi06/blob/master/doc/Xnip2026-05-29_17-10-11.jpg)


# 鼠须管词库挂载配置

1、点击 输入法 ---> 用户设定，会打开输入法配置目录。

2、将下载的字库解压到这个目录，字库不要创建子目录放字库。直接将 yml 文件全扔到 ~/Library/Rime 目录即可。

3、如果不想覆盖自己的配置，在 default.custom.yaml 配置文件加上 wubi06_pinyin 即可。
　
```yml
# default.custom.yaml
# save it to:
#   ~/.config/ibus/rime  (linux)
#   ~/Library/Rime       (macos)
#   %APPDATA%\Rime       (windows)

patch:
  schema_list:
    - schema: wubi06          # 新世纪五笔，纯五笔。支持拼音反查五笔
    - schema: wubi06_pinyin   # 新世纪五笔+拼音混输，支持拼音反查五笔
    - schema: wubi86_pinyin   # 86版五笔+拼音混输，支持拼音反查五笔
    - schema: pinyin_simp
```

4、重启部署即可。

> 词库取自（新世紀五筆通規詞庫版(CNMan)） https://github.com/CNMan/rime-data.git


# 新世纪五笔字根
![新世纪字根图.jpg](https://github.com/seangong/Rime-wubi06/blob/master/doc/%E6%96%B0%E4%B8%96%E7%BA%AA%E5%AD%97%E6%A0%B9%E5%9B%BE.jpg)

# 新世纪版与86版字根变动表
![新世纪版与86版字根变动表.jpg](https://github.com/seangong/Rime-wubi06/blob/master/doc/%E6%96%B0%E4%B8%96%E7%BA%AA%E7%89%88%E4%B8%8E86%E7%89%88%E5%AD%97%E6%A0%B9%E5%8F%98%E5%8A%A8%E8%A1%A8.jpg)

# 新世纪版五笔字型字根总表及助记词
![新世纪版五笔字型字根总表及助记词.jpg](https://github.com/seangong/rime-wubi/blob/master/doc/%E6%96%B0%E4%B8%96%E7%BA%AA%E7%89%88%E4%BA%94%E7%AC%94%E5%AD%97%E5%9E%8B%E5%AD%97%E6%A0%B9%E6%80%BB%E8%A1%A8%E5%8F%8A%E5%8A%A9%E8%AE%B0%E8%AF%8D.jpg)

# 汉字编码方法及流程.jpg
![汉字编码方法及流程.jpg](https://github.com/seangong/rime-wubi/blob/master/doc/%E6%B1%89%E5%AD%97%E7%BC%96%E7%A0%81%E6%96%B9%E6%B3%95%E5%8F%8A%E6%B5%81%E7%A8%8B.jpg)

# 汉字笔顺规则表
![汉字笔顺规则表.jpg](https://github.com/seangong/Rime-wubi06/blob/master/doc/%E6%B1%89%E5%AD%97%E7%AC%94%E9%A1%BA%E8%A7%84%E5%88%99%E8%A1%A8.jpg)

