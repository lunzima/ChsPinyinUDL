# 拼音输入法词典（全拼方案）
本项目提供一套全拼拼音输入法词典，覆盖从单字到长词组的完整词表，词频数据来自多个独立来源融合校准而成，具体方法见[`merge_pipeline.md`](merge_pipeline.md)。针对不同输入法引擎提供了多种格式，按需下载即可。

## 文件说明
1. **pinyin.dict.yaml**
Rime 拼音方案源码词典，全量版，约53.4万条，含单字。放入 Rime 用户目录参与编译即可，覆盖面最全。
2. **pinyin_lite.dict.yaml**
Rime 拼音方案源码词典，精简版，约23.6万条，含单字。词表更保守，适合追求响应速度或对词库体积有限制的场景。
3. **pinyin_fcitx5.dict**
预编译好的 fcitx5/libime 二进制词库，对应全量版。放入 fcitx5 词典目录即可加载，不需要自己编译。
4. **pinyin_lite_fcitx4.mb**
预编译好的二进制词库，对应精简版，适配 fcitx4 等旧版引擎。
5. **dict.txt**
纯文本词频表，只收≥2字的词组、不含单字，约52.5万条。适用于支持浮点型词频的输入法引擎（如Fcitx5的libime模块），词频列为浮点数。
6. **dict_intrank.txt**
内容和 dict.txt 一致，适配采用整数词频机制的主流拼音输入法，词频列为整数。
7. **merge_pipeline.md**
词典是怎么从多个互相独立的词频来源清洗、去冗余、检测离群点、校准、合并出来的，完整思路都写在这里。

## 使用指南
1. 根据自己用的输入法引擎，从上面选对应文件下载。Rime 用户下载 `.dict.yaml` 放进用户目录重新部署；fcitx5/fcitx4 用户直接用预编译的 `.dict`/`.mb`，不需要额外编译；想自己导入纯文本词典的，参考输入法软件的词库导入说明，注意选择跟文件类型匹配的词频格式。

## 参与共建
欢迎各位用户提交Issue反馈问题，或通过Pull Request贡献优质词汇数据。由于个人精力有限，词典更新频率可能不高，但会持续关注社区反馈。

## 开源协议
本项目采用[MIT开源协议](https://opensource.org/licenses/MIT)，您可以自由使用和修改代码。

---
如有疑问或建议，可通过GitHub Issues联系作者，或发送邮件至 lunzima@lunzima.net 。

祝您输入愉快！

---
# Pinyin Input Method Dictionary (Full Pinyin)
This repository provides a full-pinyin input method dictionary covering everything from single characters to long phrases. The frequency data is merged and calibrated from several independent sources; see [`merge_pipeline.md`](merge_pipeline.md) for the full methodology. Several formats are provided for different input method engines — pick what you need.

## Files Included
1. **pinyin.dict.yaml**: Rime schema source dictionary, full version, about 534K entries, includes single characters. Drop it into your Rime user directory and redeploy for the widest coverage.
2. **pinyin_lite.dict.yaml**: Rime schema source dictionary, lite version, about 236K entries, includes single characters. A more conservative word list, useful when you want faster response time or a smaller footprint.
3. **pinyin_fcitx5.dict**: Precompiled fcitx5/libime binary dictionary, corresponding to the full version. Drop it into fcitx5's dictionary directory — no compilation needed.
4. **pinyin_lite_fcitx4.mb**: Precompiled binary dictionary corresponding to the lite version, for fcitx4 and other legacy engines.
5. **dict.txt**: Plain-text frequency listing, ≥2-character phrases only (no single characters), about 525K entries. Suitable for engines that use floating-point word frequencies (e.g. fcitx5's libime module).
6. **dict_intrank.txt**: Same content as dict.txt, for mainstream pinyin IMEs that use integer-based frequencies.
7. **merge_pipeline.md**: How the dictionary was built — cleaning, redundancy removal, outlier detection, cross-source calibration and merging of several independent frequency sources.

## Usage Instructions
1. Pick the file matching your input method engine. Rime users: place the `.dict.yaml` file in your user directory and redeploy. fcitx5/fcitx4 users: use the precompiled `.dict`/`.mb` file directly, no compilation needed. If importing the plain-text listings manually, follow your IME's dictionary import instructions and pick the matching frequency format.

## Contribution Guidelines
Contributions are welcome! If you find any issues or would like to suggest improvements, please open an issue or submit a pull request on this repository. However, note that updates may not be actively maintained by the author.

## License
This project is licensed under the [MIT License](https://opensource.org/licenses/MIT). Feel free to use and modify it as per your needs.

---
For further support or inquiries, feel free to reach out via issues or by contacting me directly at lunzima@lunzima.net.

Happy typing!
