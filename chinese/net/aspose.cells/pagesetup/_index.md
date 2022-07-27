---
title: PageSetup
second_title: Aspose.Cells for .NET API 参考
description: 封装表示页面设置描述的对象 PageSetup 对象包含所有页面设置选项
type: docs
weight: 4420
url: /zh/net/aspose.cells/pagesetup/
---
## PageSetup class

封装表示页面设置描述的对象。 PageSetup 对象包含所有页面设置选项。

```csharp
public class PageSetup
```

## 特性

| 姓名 | 描述 |
| --- | --- |
| [BlackAndWhite](../../aspose.cells/pagesetup/blackandwhite) { get; set; } | 表示文档的元素是否将以黑白方式打印。 |
| [BottomMargin](../../aspose.cells/pagesetup/bottommargin) { get; set; } | 表示下边距的大小，单位为厘米。 |
| [BottomMarginInch](../../aspose.cells/pagesetup/bottommargininch) { get; set; } | 表示下边距的大小，单位为英寸。 |
| [CenterHorizontally](../../aspose.cells/pagesetup/centerhorizontally) { get; set; } | 表示纸张是否水平居中打印。 |
| [CenterVertically](../../aspose.cells/pagesetup/centervertically) { get; set; } | 表示纸张是否垂直居中打印。 |
| [FirstPageNumber](../../aspose.cells/pagesetup/firstpagenumber) { get; set; } | 表示打印此工作表时将使用的第一页码。 |
| [FitToPagesTall](../../aspose.cells/pagesetup/fittopagestall) { get; set; } | 表示工作表在打印时将缩放到的页数。 默认值为 1。 |
| [FitToPagesWide](../../aspose.cells/pagesetup/fittopageswide) { get; set; } | 表示工作表在打印时将缩放到的页数。 默认值为 1。 |
| [FooterMargin](../../aspose.cells/pagesetup/footermargin) { get; set; } | 表示页面底部到页脚的距离，单位为厘米。 |
| [FooterMarginInch](../../aspose.cells/pagesetup/footermargininch) { get; set; } | 表示页面底部到页脚的距离，单位为英寸。 |
| [HeaderMargin](../../aspose.cells/pagesetup/headermargin) { get; set; } | 表示页面顶部到页眉的距离，单位为厘米。 |
| [HeaderMarginInch](../../aspose.cells/pagesetup/headermargininch) { get; set; } | 表示页面顶部到页眉的距离，单位为英寸。 |
| [IsAutoFirstPageNumber](../../aspose.cells/pagesetup/isautofirstpagenumber) { get; set; } | 表示是否自动分配第一个页码。 |
| [IsAutomaticPaperSize](../../aspose.cells/pagesetup/isautomaticpapersize) { get; } | 表示纸张大小是否自动。 |
| [IsHFAlignMargins](../../aspose.cells/pagesetup/ishfalignmargins) { get; set; } | 表示页眉和页脚边距是否与页边距对齐。 如果该属性为true，则左侧页眉和页脚将与左边距对齐， 右侧页眉和页脚将与右侧边距对齐。 此选项默认启用。 |
| [IsHFDiffFirst](../../aspose.cells/pagesetup/ishfdifffirst) { get; set; } | true 表示第一页的页眉/页脚与其他页面不同。 |
| [IsHFDiffOddEven](../../aspose.cells/pagesetup/ishfdiffoddeven) { get; set; } | True 表示奇数页的页眉/页脚与奇数页不同。 |
| [IsHFScaleWithDoc](../../aspose.cells/pagesetup/ishfscalewithdoc) { get; set; } | 表示页眉和页脚是否随文档缩放而缩放。 仅适用于 Excel 2007。 |
| [IsPercentScale](../../aspose.cells/pagesetup/ispercentscale) { get; set; } | 如果此属性为 False，FitToPagesWide 和 FitToPagesTall 属性控制工作表的缩放方式。 |
| [LeftMargin](../../aspose.cells/pagesetup/leftmargin) { get; set; } | 表示左边距的大小，单位为厘米。 |
| [LeftMarginInch](../../aspose.cells/pagesetup/leftmargininch) { get; set; } | 表示左边距的大小，单位为英寸。 |
| [ODSPageBackground](../../aspose.cells/pagesetup/odspagebackground) { get; } | 获取ODS的背景。 |
| [Order](../../aspose.cells/pagesetup/order) { get; set; } | 表示 Microsoft Excel 在打印大型工作表时使用的页码顺序。 |
| [Orientation](../../aspose.cells/pagesetup/orientation) { get; set; } | 表示页面打印方向。 |
| [PaperHeight](../../aspose.cells/pagesetup/paperheight) { get; } | 以英寸为单位获取纸张的高度，考虑页面方向。 |
| [PaperSize](../../aspose.cells/pagesetup/papersize) { get; set; } | 代表纸张的大小。 |
| [PaperWidth](../../aspose.cells/pagesetup/paperwidth) { get; } | 以英寸为单位获取纸张的宽度，考虑页面方向。 |
| [PrintArea](../../aspose.cells/pagesetup/printarea) { get; set; } | 表示要打印的范围。 |
| [PrintComments](../../aspose.cells/pagesetup/printcomments) { get; set; } | 表示使用工作表打印注释的方式。 |
| [PrintCopies](../../aspose.cells/pagesetup/printcopies) { get; set; } | 获取并设置要打印的份数。 |
| [PrintDraft](../../aspose.cells/pagesetup/printdraft) { get; set; } | 表示是否打印不带图形的工作表。 |
| [PrintErrors](../../aspose.cells/pagesetup/printerrors) { get; set; } | 指定显示的打印错误类型。 |
| [PrinterSettings](../../aspose.cells/pagesetup/printersettings) { get; set; } | 获取和设置默认打印机的设置。 |
| [PrintGridlines](../../aspose.cells/pagesetup/printgridlines) { get; set; } | 表示页面上是否打印单元格网格线。 |
| [PrintHeadings](../../aspose.cells/pagesetup/printheadings) { get; set; } | 表示此页是否打印行和列标题。 |
| [PrintQuality](../../aspose.cells/pagesetup/printquality) { get; set; } | 代表打印质量。 |
| [PrintTitleColumns](../../aspose.cells/pagesetup/printtitlecolumns) { get; set; } | 表示包含要在每页左侧重复的单元格的列。 |
| [PrintTitleRows](../../aspose.cells/pagesetup/printtitlerows) { get; set; } | 表示包含要在每页顶部重复的单元格的行。 |
| [RightMargin](../../aspose.cells/pagesetup/rightmargin) { get; set; } | 表示右边距的大小，单位为厘米。 |
| [RightMarginInch](../../aspose.cells/pagesetup/rightmargininch) { get; set; } | 表示右边距的大小，单位为英寸。 |
| [TopMargin](../../aspose.cells/pagesetup/topmargin) { get; set; } | 表示上边距的大小，单位为厘米。 |
| [TopMarginInch](../../aspose.cells/pagesetup/topmargininch) { get; set; } | 表示上边距的大小，单位为英寸。 |
| [Zoom](../../aspose.cells/pagesetup/zoom) { get; set; } | 以百分比表示比例因子。它应该在 10 到 400 之间。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [ClearHeaderFooter](../../aspose.cells/pagesetup/clearheaderfooter)() | 清除页眉和页脚设置。 |
| [Copy](../../aspose.cells/pagesetup/copy)(PageSetup, CopyOptions) | 复制页面设置的设置。 |
| [CustomPaperSize](../../aspose.cells/pagesetup/custompapersize)(double, double) | 设置自定义纸张尺寸，以英寸为单位。 |
| [GetCommands](../../aspose.cells/pagesetup/getcommands)(string) | 获取页眉或页脚的所有命令。 |
| [GetEvenFooter](../../aspose.cells/pagesetup/getevenfooter)(int) | 获取格式化 Excel 文件偶数页脚的脚本。 |
| [GetEvenHeader](../../aspose.cells/pagesetup/getevenheader)(int) | 获取格式化 Excel 文件偶数标头的脚本。 |
| [GetFirstPageFooter](../../aspose.cells/pagesetup/getfirstpagefooter)(int) | 获取格式化 Excel 文件首页页脚的脚本。 |
| [GetFirstPageHeader](../../aspose.cells/pagesetup/getfirstpageheader)(int) | 获取格式化 Excel 文件第一页标题的脚本。 |
| [GetFooter](../../aspose.cells/pagesetup/getfooter)(int) | 获取格式化 Excel 文件页脚的脚本。 |
| [GetHeader](../../aspose.cells/pagesetup/getheader)(int) | 获取格式化 Excel 文件标题的脚本。 |
| [GetPicture](../../aspose.cells/pagesetup/getpicture#getpicture_1)(bool, int) | 获取[`Picture`](../../aspose.cells.drawing/picture)页眉/页脚的对象. |
| [GetPicture](../../aspose.cells/pagesetup/getpicture#getpicture)(bool, bool, bool, int) | 获取[`Picture`](../../aspose.cells.drawing/picture)页眉/页脚的对象. |
| [SetEvenFooter](../../aspose.cells/pagesetup/setevenfooter)(int, string) | 设置脚本格式化 Excel 文件的偶数页脚。 仅当 IsHFDiffOddEven 为 true 时在 Excel 2007 中有效。 |
| [SetEvenHeader](../../aspose.cells/pagesetup/setevenheader)(int, string) | 设置脚本格式化 Excel 文件的偶数页标题。 仅当 IsHFDiffOddEven 为 true 时在 Excel 2007 中有效。 |
| [SetFirstPageFooter](../../aspose.cells/pagesetup/setfirstpagefooter)(int, string) | 设置格式化 Excel 文件首页页脚的脚本。 |
| [SetFirstPageHeader](../../aspose.cells/pagesetup/setfirstpageheader)(int, string) | 设置格式化 Excel 文件首页页眉的脚本。 仅当 IsHFDiffFirst 为 true 时在 Excel 2007 中有效。 |
| [SetFitToPages](../../aspose.cells/pagesetup/setfittopages)(int, int) | 设置工作表在打印时将缩放到的页数。 |
| [SetFooter](../../aspose.cells/pagesetup/setfooter)(int, string) | 设置格式化 Excel 文件页脚的脚本。 |
| [SetFooterPicture](../../aspose.cells/pagesetup/setfooterpicture)(int, byte[]) | 在工作表的页脚中设置图像。 |
| [SetHeader](../../aspose.cells/pagesetup/setheader)(int, string) | 设置格式化 Excel 文件标题的脚本。 |
| [SetHeaderPicture](../../aspose.cells/pagesetup/setheaderpicture)(int, byte[]) | 在工作表的标题中设置图像。 |
| [SetPicture](../../aspose.cells/pagesetup/setpicture)(bool, bool, bool, int, byte[]) | 在工作表的页眉/页脚中设置图像。 |

### 例子

```csharp
[C#]

Workbook workbook = new Workbook();

WorksheetCollection sheets = workbook.Worksheets;

//添加工作表
sheets.Add();
Worksheet sheet = sheets[1];
PageSetup pageSetup = sheet.PageSetup;
pageSetup.PrintArea = "D1:K13";

//做你的事

[Visual Basic]
Dim excel as Workbook = new Workbook()

Dim sheets as WorksheetCollection = excel.Worksheets

'添加工作表
sheets.Add()
Dim sheet as Worksheet = sheets(1)
Dim pageSetup as PageSetup = sheet.PageSetup
pageSetup.PrintArea = "D1:K13"
```

### 也可以看看

* 命名空间 [Aspose.Cells](../../aspose.cells)
* 部件 [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
