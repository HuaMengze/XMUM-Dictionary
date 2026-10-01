# 厦门大学马来西亚分校 物理学 英汉词典
# XMUM Physics English–Chinese Dictionary

**作者 / Author：Hua Mengze · PHY2609012**

面向物理学大一课程的英汉词汇查询与复习工具。内置 310 个关键词，支持英文、中文双向检索、学科分类浏览，以及后续词库扩充。

An English–Chinese vocabulary tool for first-year physics studies. It includes 310 keywords, supports lookup in either language and browsing by subject, and allows you to expand the dictionary with new entries.

---

## 中文

### 项目简介

本词典根据本周五门课程的课件整理，涵盖微积分、线性代数、力学、热力学和 Python。除课件关键词外，也收录少量与上下文紧密相关的补充词汇，便于理解和记忆。

每个词条展示 **英文、中文、解释和所属组别**。解释以简明定义、公式或符号为主，不包含例句。跨学科重复术语尽量归入最相关的学科。

### 词库构成

| 学科 | 初始词条数 |
| --- | ---: |
| 微积分 | 78 |
| 线性代数 | 64 |
| 力学 | 60 |
| 热力学 | 37 |
| Python | 71 |
| **合计** | **310** |

### 主要功能

- **英汉互查**：输入英文或中文关键词，也可以切换为仅英文或仅中文检索；支持部分匹配，英文不区分大小写。
- **完整词库浏览**：查看全部词条，或按五门学科筛选。
- **排序与分页**：支持默认排序、英文 A–Z 排序、最新添加优先，以及每页 30 条、60 条或全部显示。
- **手动添加**：填写英文、中文、解释和组别，可使用已有学科或创建新组别。
- **批量导入**：支持 `.xlsx`、`.csv`、`.tsv` 和 `.json` 文件，导入前显示预览与重复项数量。
- **保存完整网页**：将当前词库与页面一起下载为独立 HTML 文件。
- **离线使用**：单个 HTML 文件包含页面所需的代码和初始词库，无需账户或后端服务。

### 使用方法

1. 下载词典 HTML 文件。已有文件名为 `厦门大学马来西亚分校_物理学英汉词典.html`；如仓库将它命名为 `index.html`，下载该文件即可。
2. 使用现代浏览器打开文件。
3. 在搜索框中输入英文或中文，或点击学科分类浏览词条。
4. 添加或导入词条后，点击 **“保存网页”**，下载包含更新词库的 HTML 文件。
5. 下次使用时，打开新下载的文件。

**新增内容不会自动写回原文件，也不会同步到 GitHub。刷新或关闭网页前，请先保存更新后的网页。**

### 扩充词库

CSV、TSV 和 Excel 推荐使用以下表头：

| 英文 | 中文 | 解释 | 组别 |
| --- | --- | --- | --- |
| angular momentum | 角动量 | L = r × p | 力学 |

也可使用英文表头 `english`、`chinese`、`explanation`、`group`。Excel 未填写组别时，使用工作表名称作为组别；CSV、TSV 和 JSON 未填写组别时，使用导入窗口指定的默认组别。

JSON 使用如下结构：

```json
[
  {
    "english": "angular momentum",
    "chinese": "角动量",
    "explanation": "L = r × p",
    "group": "力学"
  }
]
```

导入时，**英文与组别均相同**的词条会被视为重复项并跳过；比较前会统一大小写、空白及部分字符形式。不同组别中的同一英文术语不会自动合并，跨学科归类仍需整理者判断。

### 技术实现

页面使用 HTML、CSS 和原生 JavaScript，词库以内嵌 JSON 保存，Excel 导入使用内嵌的 pako 解压组件。桌面与窄屏设备采用不同布局，无需安装应用即可使用。

### 作者

**Hua Mengze**  
**学号：PHY2609012**  
厦门大学马来西亚分校

这是个人学习项目，用于课程词汇复习，并非学校官方词典。欢迎通过 GitHub Issues 提交词条纠错或补充建议；请附上英文、中文、解释及建议所属学科。

---

## English

### About

This dictionary was compiled from one week of materials across five first-year subjects: Calculus, Linear Algebra, Mechanics, Thermodynamics, and Python. It also includes a small number of closely related supplementary terms to support understanding and memorization.

Each entry displays an **English term, Chinese translation, explanation, and subject group**. Explanations focus on concise definitions, formulas, or symbols, without example sentences. Terms shared across subjects are assigned to the most relevant subject where possible.

### Initial vocabulary

| Subject | Entries |
| --- | ---: |
| Calculus | 78 |
| Linear Algebra | 64 |
| Mechanics | 60 |
| Thermodynamics | 37 |
| Python | 71 |
| **Total** | **310** |

### Features

- **Lookup in either language:** Search English or Chinese terms, with optional English-only or Chinese-only modes. Partial matching is supported, and English search is case-insensitive.
- **Browse the full dictionary:** View all entries or filter by subject.
- **Sorting and pagination:** Use the default order, English A–Z, or newest-first order. Display 30, 60, or all entries per page.
- **Add entries manually:** Enter a term, translation, explanation, and subject. Existing or new subject groups can be used.
- **Import vocabulary:** Load `.xlsx`, `.csv`, `.tsv`, or `.json` files, with a preview and duplicate count before confirmation.
- **Save the complete page:** Download the current dictionary as a self-contained HTML file.
- **Offline access:** The HTML file contains the required page code and initial vocabulary. No account or backend service is required.

### Getting started

1. Download the dictionary HTML file, currently named `厦门大学马来西亚分校_物理学英汉词典.html`. If the repository uses `index.html` instead, download that file.
2. Open it in a modern browser.
3. Search for an English or Chinese term, or choose a subject to browse.
4. After adding or importing entries, click **“保存网页” (Save webpage)** to download an updated HTML file.
5. Open that newly downloaded file for your next session.

**New entries are not automatically written back to the original file or synchronized with GitHub. Save the updated webpage before refreshing or closing it.**

### Extending the dictionary

For CSV, TSV, or Excel imports, the recommended columns are:

| english | chinese | explanation | group |
| --- | --- | --- | --- |
| angular momentum | 角动量 | L = r × p | 力学 |

Chinese column names—`英文`, `中文`, `解释`, and `组别`—are also supported. If a group is omitted in Excel, the worksheet name is used. For CSV, TSV, and JSON, the default group selected in the import dialog is used.

JSON files can contain an array of entry objects:

```json
[
  {
    "english": "angular momentum",
    "chinese": "角动量",
    "explanation": "L = r × p",
    "group": "力学"
  }
]
```

Entries with the **same English term and subject group** are skipped as duplicates after normalization of case, whitespace, and certain character forms. Identical English terms in different groups are not automatically merged; cross-subject classification requires editorial judgment.

### Implementation

The page uses HTML, CSS, and vanilla JavaScript, with an embedded JSON dictionary and bundled pako decompression for Excel imports. Responsive layouts support desktop and narrow screens without installing an application.

### Author

**Hua Mengze**  
**Student ID: PHY2609012**  
Xiamen University Malaysia

This is a personal learning project for course vocabulary revision, not an official university dictionary. Corrections and vocabulary suggestions are welcome through GitHub Issues. Please include the English term, Chinese translation, explanation, and suggested subject.
