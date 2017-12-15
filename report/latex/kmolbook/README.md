Leo-editor-report-template
===

使用 Leo-editor 套用 latex 模板，將 Markdown 轉換為 PDF 格式。

安裝
===

下載並安裝 Pandoc：

<https://github.com/jgm/pandoc/releases/>

Ubuntu
---

安裝 texlive

```bash
sudo apt install texlive texlive-xetex texlive-lang-chinese etoolbox
```

Windows
---

安裝 Miktex

<http://www.texts.io/support/0002/>

接著使用 MikTex Package Manager 搜尋並安裝以下套件：

+ etoolbox
+ cjk（中文、日文、韓文語法支援，包含漢字數字）
+ xecjk（基本的 CJK 支援）
+ makecmds（Latex 的自定義函式，提供自訂與複寫參數）

協同規則
===

所有 Leo 專案檔皆有所職，以 master 為主，負責控管封面、摘要、模板檔案。

組員根據 contributor1.leo 的樣式創建負責的 Markdown 文件，命名規則為 paragraph 加上章節順序。

**最後 Pandoc 合併時會以 `master`+`paragraph1`+`paragraph2` 的順序合併。**

Leo 專案中，直接點擊 report-pdf 按鈕即可開始轉檔。
