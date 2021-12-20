# BUAA_Dissertation_Template
北航硕博研究生毕业论文模板（Word）


## 特点

- ✅参照了[《北京航空航天大学研究生撰写学位论文的规定》](http://graduate.buaa.edu.cn/info/1039/7831.htm)2021年11月的最新修订要求
  
- ✅专业/学术学位，硕士/博士，尽在一套模板
  
- ✅按顺序组织了论文结构，开箱即用
  
- ✅自动修改题注格式，无需操心这里那里的空格
  
- ✅搭配NoteExpress使用，自动排版参考文献
  
- ……


## 模板使用说明

- 模板基于Microsoft Office 2013，如有兼容问题，请提Issues。

- 请在审阅-修订中显示所有批注，并将显示标注方式改为“在批注框中显示修订”；按照批注进行更改即可，更改完后，审阅-删除下拉按钮-删除文档中的所有批注。

- 注意区分专业/学术学位硕/博士的中/英文封面和提名页，删除不需要的中/英文封面和提名页。

- 请在选项-信任中心-信任中心设置-宏设置-启用宏中启用所有宏，如果你不明白[使用宏所带来的风险的信息](https://support.microsoft.com/zh-cn/office/%E5%90%AF%E7%94%A8%E6%88%96%E7%A6%81%E7%94%A8-office-%E6%96%87%E4%BB%B6%E4%B8%AD%E7%9A%84%E5%AE%8F-12b036fd-d140-4e74-b45e-16fed1a7e5c6)，不建议启用，你将需要手动创建“图”“表”这两个题注标签，以及手动修改每一个插入的题注格式。详细见[其他事项](#macro)。
  
- 对图/表插入题注：插入时，选中图/表，引用-插入题注，选择图/表标签以及题注位置；正文中引用时，引用-交叉引用，选择引用类型以及引用内容。
  
- 对于目录以及全部图/表清单、域的自动更新，可以Ctrl+A全选然后F9更新，也可以逐个右键然后更新域。

- Word公式编辑可以使用[这个工具](https://github.com/ixzhao/ixzhao.github.io)。
  
- 参考文献的自动排版，可以借助NoteExpress的样式文件，如果你平时用NoteExpress管理你的文献。但是NoteExpress自带的北航硕博论文样式已经很久不更新了，可以用本仓库中的“北航硕博论文.nes”替换。  
  
  用仓库里的nes文件直接替换 C:\Users\你的用户名\AppData\Roaming\NoteExpress\Styles 路径里的原文件“北京航空航天大学博硕士论文.nes”（记得先备份）；如果在授权IP范围以外，可以先将文件重命名为7个默认样式之一然后再替换。
    ```
    NoteExpress的个人标准版是不允许在授权IP范围以外使用的，而且限制只能使用7个默认的样式，样式格式也不能编辑。所以推荐使用集团版，可以在学校图书馆首页-右侧快速链接-常用工具下载。或者到 http://www.inoteexpress.com/download_chs.htm#Downloads 找一个可以在授权IP范围外下载的高校集团版本，比如北大版 http://www.inoteexpress.com/support/cgi-bin/download_sch.cgi?code=BeiDa（该途径低调下载使用，说不定哪天页面就打不开了）。
    ```
  
- 建议在开始-段落-显示编辑标记、在状态栏右键勾选“节”。❗❗❗注意❗❗❗打印时很有可能会在3个地方分别多出一页空白页，个人建议将Word文件输出为PDF文件，然后使用Adobe Acrobat等工具删除多余的空白页。具体原因见[其他事项](#blankpage)。
  
- 其他内容可参照《规定》填写。
  
  📌在线乞讨环节：
  如果本仓库大大地节省了你的时间，何尝不请我喝一杯小小的Coffee？

  <span><img src="https://raw.githubusercontent.com/ixzhao/BUAA_Dissertation_Template/main/image/alipay.jpg" width="40%"/>&nbsp;&nbsp;&nbsp;&nbsp;<img src="https://raw.githubusercontent.com/ixzhao/BUAA_Dissertation_Template/main/image/wechat.jpg" width="40%"/></span>



## 其他事项

- <span><a name="macro"></a></span>模板是启用宏的Word文件，主要考虑2个方面：  
  
  一是题注标签只能保存到本机上Office默认的Normal.dotm模板里（参考[这里](https://www.msofficeforums.com/word/15715-captions-self-defined.html#2)），所以只能通过宏（现查的VBA的编程规范，头发掉了一把😢），在每次打开文档时自动添加“图”和“表”这两个题注标签。如果不需要，可以进入宏工程后，在左侧窗口Project-ThisDocument双击，清空内容。  

  二是《规定》要求的题注格式为“图1空格空格XXX”，这与Word默认的题注格式不同，手动更改太麻烦，所以还是通过宏（借鉴的[这里](http://blog.sina.com.cn/s/blog_51817ae50102w8mz.html)），插入题注时自动删除标签与编号前的空格，自动在编号后添加2个空格。如果不需要，直接在查看宏界面删除即可。  
  
- <span><a name="blankpage"></a></span>由于使用了分节符、（页眉页脚）奇偶页不同等选项，导致Word会强制将每一节的第一页显示在纸的右页（正面），即新的一节总是从奇数页开始，如果上一节结束在奇数页，那么将多出一页偶数页，具体见[这个页面最下边的Important Warning](http://wordfaqs.ssbarnhill.com/BlankPage.htm#True_blank_pages)。  
虽然可以通过更改分节符的类型规避空白页，但是如果文档有新的修改后都可能改变奇偶页的布局，因此建议的方式是将Word文件输出为PDF后删除多余的空白页。[这里](https://answers.microsoft.com/en-us/msoffice/forum/all/word-print-preview-adds-extra-blank-pages/05710a98-838f-4b74-9b7c-e57b8c63eda3)给出的建议也是对导出的PDF文件进行修改。
  
- 感谢 [heckBoxStudio/BUAAThesis](https://github.com/CheckBoxStudio/BUAAThesis)。
  
- 待补充。
  

















