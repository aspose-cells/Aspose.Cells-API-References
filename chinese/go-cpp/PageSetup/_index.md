---
title: "PageSetup 类"
linktitle: "PageSetup"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "PageSetup 类。封装表示 Go 中 pagesetup 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/pagesetup/
---

## PageSetup class

封装表示页面设置描述的对象。PageSetup 对象包含所有页面设置选项。

```go

type PageSetup struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetODSPageBackground](./getodspagebackground/) | 获取 ODS 的背景。 |
| [Copy](./copy/) | 复制页面设置的配置。 |
| [GetPrintArea](./getprintarea/) | 表示要打印的范围。 |
| [SetPrintArea](./setprintarea/) | 表示要打印的范围。 |
| [GetPrintTitleColumns](./getprinttitlecolumns/) | 表示包含要在每页左侧重复的单元格的列。 |
| [SetPrintTitleColumns](./setprinttitlecolumns/) | 表示包含要在每页左侧重复的单元格的列。 |
| [GetPrintTitleRows](./getprinttitlerows/) | 表示包含要在每页顶部重复的单元格的行。 |
| [SetPrintTitleRows](./setprinttitlerows/) | 表示包含要在每页顶部重复的单元格的行。 |
| [GetBlackAndWhite](./getblackandwhite/) | 表示文档元素是否以黑白方式打印。 |
| [SetBlackAndWhite](./setblackandwhite/) | 表示文档元素是否以黑白方式打印。 |
| [GetCenterHorizontally](./getcenterhorizontally/) | 表示工作表是否水平居中打印。 |
| [SetCenterHorizontally](./setcenterhorizontally/) | 表示工作表是否水平居中打印。 |
| [GetCenterVertically](./getcentervertically/) | 表示工作表是否垂直居中打印。 |
| [SetCenterVertically](./setcentervertically/) | 表示工作表是否垂直居中打印。 |
| [GetPrintDraft](./getprintdraft/) | 表示工作表是否将在不包含图形的情况下打印。 |
| [SetPrintDraft](./setprintdraft/) | 表示工作表是否将在不包含图形的情况下打印。 |
| [GetFooterMargin](./getfootermargin/) | 表示页面底部到页脚的距离，单位为厘米。 |
| [SetFooterMargin](./setfootermargin/) | 表示页面底部到页脚的距离，单位为厘米。 |
| [GetFooterMarginInch](./getfootermargininch/) | 表示页面底部到页脚的距离，单位为英寸。 |
| [SetFooterMarginInch](./setfootermargininch/) | 表示页面底部到页脚的距离，单位为英寸。 |
| [GetHeaderMargin](./getheadermargin/) | 表示页面顶部到页眉的距离，单位为厘米。 |
| [SetHeaderMargin](./setheadermargin/) | 表示页面顶部到页眉的距离，单位为厘米。 |
| [GetHeaderMarginInch](./getheadermargininch/) | 表示页面顶部到页眉的距离，单位为英寸。 |
| [SetHeaderMarginInch](./setheadermargininch/) | 表示页面顶部到页眉的距离，单位为英寸。 |
| [GetPrinterSettings](./getprintersettings/) | 获取并设置默认打印机的设置。 |
| [SetPrinterSettings](./setprintersettings/) | 获取并设置默认打印机的设置。 |
| [GetLeftMargin](./getleftmargin/) | 表示左边距的大小，单位为厘米。 |
| [SetLeftMargin](./setleftmargin/) | 表示左边距的大小，单位为厘米。 |
| [GetLeftMarginInch](./getleftmargininch/) | 表示左边距的大小，单位为英寸。 |
| [SetLeftMarginInch](./setleftmargininch/) | 表示左边距的大小，单位为英寸。 |
| [GetRightMargin](./getrightmargin/) | 表示右边距的大小，单位为厘米。 |
| [SetRightMargin](./setrightmargin/) | 表示右边距的大小，单位为厘米。 |
| [GetRightMarginInch](./getrightmargininch/) | 表示右边距的大小，单位为英寸。 |
| [SetRightMarginInch](./setrightmargininch/) | 表示右边距的大小，单位为英寸。 |
| [GetTopMargin](./gettopmargin/) | 表示上边距的大小，单位为厘米。 |
| [SetTopMargin](./settopmargin/) | 表示上边距的大小，单位为厘米。 |
| [GetTopMarginInch](./gettopmargininch/) | 表示上边距的大小，单位为英寸。 |
| [SetTopMarginInch](./settopmargininch/) | 表示上边距的大小，单位为英寸。 |
| [GetBottomMargin](./getbottommargin/) | 表示下边距的大小，单位为厘米。 |
| [SetBottomMargin](./setbottommargin/) | 表示下边距的大小，单位为厘米。 |
| [GetBottomMarginInch](./getbottommargininch/) | 表示下边距的大小，单位为英寸。 |
| [SetBottomMarginInch](./setbottommargininch/) | 表示下边距的大小，单位为英寸。 |
| [GetFirstPageNumber](./getfirstpagenumber/) | 表示打印此工作表时使用的起始页码。 |
| [SetFirstPageNumber](./setfirstpagenumber/) | 表示打印此工作表时使用的起始页码。 |
| [SetFitToPages](./setfittopages/) | 设置打印时工作表缩放到的页数。 |
| [GetFitToPagesTall](./getfittopagestall/) | 表示打印时工作表在纵向上缩放到的页数。默认值为 1。 |
| [SetFitToPagesTall](./setfittopagestall/) | 表示打印时工作表在纵向上缩放到的页数。默认值为 1。 |
| [GetFitToPagesWide](./getfittopageswide/) | 表示打印时工作表在横向上缩放到的页数。默认值为 1。 |
| [SetFitToPagesWide](./setfittopageswide/) | 表示打印时工作表在横向上缩放到的页数。默认值为 1。 |
| [IsPercentScale](./ispercentscale/) | 如果此属性为 False，则 FitToPagesWide 和 FitToPagesTall 属性控制工作表的缩放方式。 |
| [SetIsPercentScale](./setispercentscale/) | 如果此属性为 False，则 FitToPagesWide 和 FitToPagesTall 属性控制工作表的缩放方式。 |
| [GetOrder](./getorder/) | 表示 Microsoft Excel 在打印大型工作表时对页码进行排序的方式。 |
| [SetOrder](./setorder/) | 表示 Microsoft Excel 在打印大型工作表时对页码进行排序的方式。 |
| [IsAutomaticPaperSize](./isautomaticpapersize/) | 指示纸张尺寸是否为自动。 |
| [GetPaperSize](./getpapersize/) | 表示纸张的尺寸。 |
| [SetPaperSize](./setpapersize/) | 表示纸张的尺寸。 |
| [GetPaperWidth](./getpaperwidth/) | 获取纸张的宽度，单位为英寸，考虑页面方向。 |
| [GetPaperHeight](./getpaperheight/) | 获取纸张的高度，单位为英寸，考虑页面方向。 |
| [CustomPaperSize](./custompapersize/) | 设置自定义纸张尺寸，单位为英寸。 |
| [GetOrientation](./getorientation/) | 表示页面打印方向。 |
| [SetOrientation](./setorientation/) | 表示页面打印方向。 |
| [GetPrintComments](./getprintcomments/) | 表示注释随工作表打印的方式。 |
| [SetPrintComments](./setprintcomments/) | 表示注释随工作表打印的方式。 |
| [GetPrintErrors](./getprinterrors/) | 指定显示的打印错误类型。 |
| [SetPrintErrors](./setprinterrors/) | 指定显示的打印错误类型。 |
| [GetPrintHeadings](./getprintheadings/) | 表示是否在此页面上打印行和列标题。 |
| [SetPrintHeadings](./setprintheadings/) | 表示是否在此页面上打印行和列标题。 |
| [GetPrintGridlines](./getprintgridlines/) | 表示是否在页面上打印单元格网格线。 |
| [SetPrintGridlines](./setprintgridlines/) | 表示是否在页面上打印单元格网格线。 |
| [GetZoom](./getzoom/) | 表示以百分比计的缩放比例。应在 10 到 400 之间。 |
| [SetZoom](./setzoom/) | 表示以百分比计的缩放比例。应在 10 到 400 之间。 |
| [IsAutoFirstPageNumber](./isautofirstpagenumber/) | 指示是否自动分配首页页码。 |
| [SetIsAutoFirstPageNumber](./setisautofirstpagenumber/) | 指示是否自动分配首页页码。 |
| [GetPrintQuality](./getprintquality/) | 表示打印质量。 |
| [SetPrintQuality](./setprintquality/) | 表示打印质量。 |
| [GetPrintCopies](./getprintcopies/) | 获取并设置要打印的副本数。 |
| [SetPrintCopies](./setprintcopies/) | 获取并设置要打印的副本数。 |
| [ClearHeaderFooter](./clearheaderfooter/) | 清除页眉和页脚设置。 |
| [GetHeader](./getheader/) | 获取用于格式化 Excel 文件页眉的脚本。 |
| [GetCommands](./getcommands/) | 获取页眉或页脚的所有命令。 |
| [GetFooter](./getfooter/) | 获取用于格式化 Excel 文件页脚的脚本。 |
| [SetHeader](./setheader/) | 设置用于格式化 Excel 文件页眉的脚本。 |
| [SetFooter](./setfooter/) | 设置用于格式化 Excel 文件页脚的脚本。 |
| [SetEvenHeader](./setevenheader/) | 设置用于格式化 Excel 文件偶数页页眉的脚本。仅在 IsHFDiffOddEven 为 true 时对 Excel 2007 生效。 |
| [GetEvenHeader](./getevenheader/) | 获取用于格式化 Excel 文件偶数页页眉的脚本。 |
| [SetEvenFooter](./setevenfooter/) | 设置用于格式化 Excel 文件偶数页页脚的脚本。仅在 IsHFDiffOddEven 为 true 时对 Excel 2007 生效。 |
| [GetEvenFooter](./getevenfooter/) | 获取用于格式化 Excel 文件偶数页页脚的脚本。 |
| [SetFirstPageHeader](./setfirstpageheader/) | 设置用于格式化 Excel 文件首页页眉的脚本。仅在 IsHFDiffFirst 为 true 时对 Excel 2007 生效。 |
| [GetFirstPageHeader](./getfirstpageheader/) | 获取用于格式化 Excel 文件首页页眉的脚本。 |
| [SetFirstPageFooter](./setfirstpagefooter/) | 设置用于格式化 Excel 文件首页页脚的脚本。 |
| [GetFirstPageFooter](./getfirstpagefooter/) | 获取用于格式化 Excel 文件首页页脚的脚本。 |
| [IsHFDiffOddEven](./ishfdiffoddeven/) | True 表示奇数页的页眉/页脚与偶数页不同。 |
| [SetIsHFDiffOddEven](./setishfdiffoddeven/) | True 表示奇数页的页眉/页脚与偶数页不同。 |
| [IsHFDiffFirst](./ishfdifffirst/) | True 表示首页的页眉/页脚与其他页不同。 |
| [SetIsHFDiffFirst](./setishfdifffirst/) | True 表示首页的页眉/页脚与其他页不同。 |
| [IsHFScaleWithDoc](./ishfscalewithdoc/) | 指示页眉和页脚是否随文档缩放而缩放。仅适用于 Excel 2007。 |
| [SetIsHFScaleWithDoc](./setishfscalewithdoc/) | 指示页眉和页脚是否随文档缩放而缩放。仅适用于 Excel 2007。 |
| [IsHFAlignMargins](./ishfalignmargins/) | 指示页眉和页脚的边距是否与页面边距对齐。如果此属性为 true，左侧页眉和页脚将与左边距对齐，右侧页眉和页脚将与右边距对齐。此选项默认启用。 |
| [SetIsHFAlignMargins](./setishfalignmargins/) | 指示页眉和页脚的边距是否与页面边距对齐。如果此属性为 true，左侧页眉和页脚将与左边距对齐，右侧页眉和页脚将与右边距对齐。此选项默认启用。 |
| [SetHeaderPicture](./setheaderpicture/) | 在工作表的页眉中设置图像。 |
| [SetFooterPicture](./setfooterpicture/) | 在工作表的页脚中设置图像。 |
| [SetPicture](./setpicture/) | 在工作表的页眉/页脚中设置图像。 |
| [GetPicture_Bool_Int](./getpicture_bool_int/) | 获取页眉/页脚的 Picture 对象。 |
| [GetPicture_Bool_Bool_Bool_Int](./getpicture_bool_bool_bool_int/) | 获取页眉/页脚的 Picture 对象。 |
