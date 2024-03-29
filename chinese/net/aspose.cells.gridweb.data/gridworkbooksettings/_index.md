---
title: GridWorkbookSettings
second_title: Aspose.Cells for .NET API 参考
description: 表示工作簿的设置
type: docs
weight: 560
url: /zh/net/aspose.cells.gridweb.data/gridworkbooksettings/
---
## GridWorkbookSettings class

表示工作簿的设置。

```csharp
public class GridWorkbookSettings
```

## 构造函数

| 姓名 | 描述 |
| --- | --- |
| [GridWorkbookSettings](gridworkbooksettings)() | 默认构造函数。 |

## 特性

| 姓名 | 描述 |
| --- | --- |
| [Author](../../aspose.cells.gridweb.data/gridworkbooksettings/author) { get; set; } | 获取和设置文件的作者。 |
| [CheckCustomNumberFormat](../../aspose.cells.gridweb.data/gridworkbooksettings/checkcustomnumberformat) { get; set; } | 获取或设置设置Style.Custom. 时是否检查自定义数字格式 |
| [CreateCalcChain](../../aspose.cells.gridweb.data/gridworkbooksettings/createcalcchain) { get; set; } | 获取或设置是否创建计算公式链。默认为假。 |
| [Date1904](../../aspose.cells.gridweb.data/gridworkbooksettings/date1904) { get; set; } | 获取或设置表示工作簿是否使用 1904 日期系统的值。 |
| [EnableMacros](../../aspose.cells.gridweb.data/gridworkbooksettings/enablemacros) { get; set; } | 获取或设置是否启用宏；现在它仅在将工作表复制到工作簿中的其他工作表时才有效。 |
| [ForceFullCalculate](../../aspose.cells.gridweb.data/gridworkbooksettings/forcefullcalculate) { get; set; } | 获取或设置每次触发计算时是否完全计算。 |
| [Iteration](../../aspose.cells.gridweb.data/gridworkbooksettings/iteration) { get; set; } | 获取或设置是否使用迭代来解析循环引用。 |
| [MaxIteration](../../aspose.cells.gridweb.data/gridworkbooksettings/maxiteration) { get; set; } | 获取或设置解析循环引用的最大迭代次数，默认值为100。 |
| [PrecisionAsDisplayed](../../aspose.cells.gridweb.data/gridworkbooksettings/precisionasdisplayed) { get; set; } | 如果本工作簿中的计算仅使用所显示数字的精度来完成，则为真 |
| [ReCalculateOnOpen](../../aspose.cells.gridweb.data/gridworkbooksettings/recalculateonopen) { get; set; } | 获取或设置是否在打开文件时重新计算所有公式。 |

### 例子

```csharp
[C#]

 

GridWorkbookSettings gsettings = new GridWorkbookSettings();
gridweb.Settings=gsettings;

//做你的事

[Visual Basic]


Dim gsettings as GridWorkbookSettings = new GridWorkbookSettings()
 gridweb..Settings=gsettings;
 
'做你的事
```

### 也可以看看

* 命名空间 [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data)
* 部件 [Aspose.Cells.GridWeb](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridWeb.dll -->
