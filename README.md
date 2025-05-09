# 拼音输入法词典（全拼方案）
本项目提供了一份精心整理的全拼拼音输入法词典，内含丰富的词汇频率数据。通过这套词典，可以显著提升输入时的候选词准确度，让打字更高效流畅。

## 文件说明
1. **dict.txt**  
适用于支持浮点型词频的输入法引擎（如Fcitx5的libime模块）。该文件不仅涵盖完整的拼音映射关系，还包含精细的词频统计，有助于提高高频词的输入预测能力。
2. **dict_intrank.txt**  
适配采用整数词频机制的主流拼音输入法。在保持格式兼容性的同时，确保候选词排序的准确性与实用性。

## 使用指南
1. 根据输入法类型选择对应词典文件下载  
2. 参考输入法软件的词库导入说明进行操作  
3. 导入时请注意选择与文件类型匹配的词频格式

## 参与共建
欢迎各位用户提交Issue反馈问题，或通过Pull Request贡献优质词汇数据。由于个人精力有限，词典更新频率可能不高，但会持续关注社区反馈。

## 开源协议
本项目采用[MIT开源协议](https://opensource.org/licenses/MIT)，您可以自由使用和修改代码。

---
如有疑问或建议，可通过GitHub Issues联系作者，或发送邮件至 lunzima@lunzima.net 。

祝您输入愉快！

---
# Pinyin Input Method Dictionary (Full Pinyin)
This GitHub repository provides a custom-made pinyin input method dictionary that includes word frequency information. The dictionary is designed to enhance the typing experience by offering more accurate and relevant suggestions based on common usage patterns.

## Files Included
1. **dict.txt**: This file contains a libime formatted dictionary suitable for use with fcitx5 and other input methods that utilize floating-point numbers as word frequencies. It includes comprehensive pinyin mappings along with precise word frequency data, which helps in predicting frequently used words.
2. **dict_intrank.txt**: This file is tailored for other popular pinyin input methods that utilize integer-based word frequency information. The format ensures compatibility while maintaining the accuracy and relevance of the suggestions provided by the dictionary.

## Usage Instructions
1. Download either `dict_intrank.txt` or `dict.txt`.
2. Follow the specific instructions provided by your pinyin input method regarding dictionary importation.
3. Ensure that you select the correct format (integer-based frequency) during the import process.

## Contribution Guidelines
Contributions are welcome! If you find any issues or would like to suggest improvements, please open an issue or submit a pull request on this repository. However, note that updates may not be actively maintained by the author.

## License
This project is licensed under the [MIT License](https://opensource.org/licenses/MIT). Feel free to use and modify it as per your needs.

---
For further support or inquiries, feel free to reach out via issues or by contacting me directly at lunzima@lunzima.net.

Happy typing!
