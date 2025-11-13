---
title: Class GridWorkbookSettings
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.GridJs.GridWorkbookSettings class. Represents the settings of the workbook
type: docs
url: /net/aspose.cells.gridjs/gridworkbooksettings/
---
## GridWorkbookSettings class

Represents the settings of the workbook.

```csharp
public class GridWorkbookSettings
```

## Constructors

| Name | Description |
| --- | --- |
| [GridWorkbookSettings](gridworkbooksettings/)() | The default constructor. |

## Properties

| Name | Description |
| --- | --- |
| [Author](../../aspose.cells.gridjs/gridworkbooksettings/author/) { get; set; } | Gets/sets the author of the file. |
| [CheckCustomNumberFormat](../../aspose.cells.gridjs/gridworkbooksettings/checkcustomnumberformat/) { get; set; } | Indicates whether checking custom number format when setting Style.Custom, default is false. |
| [CheckExcelRestriction](../../aspose.cells.gridjs/gridworkbooksettings/checkexcelrestriction/) { get; set; } | Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception. If this property is false, we will accept your input string value as the cell's value so that later you can output the complete string value for other file formats such as CSV. However, if you have set such kind of value that is invalid for excel file format, you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file. default is false. |
| [CreateCalcChain](../../aspose.cells.gridjs/gridworkbooksettings/createcalcchain/) { get; set; } | Indicates whether create calculated formulas chain. Default is false. |
| [Date1904](../../aspose.cells.gridjs/gridworkbooksettings/date1904/) { get; set; } | Gets or sets a value which represents if the workbook uses the 1904 date system. |
| [EnableMacros](../../aspose.cells.gridjs/gridworkbooksettings/enablemacros/) { get; set; } | Enable macros; Now it only works when copying a worksheet to other worksheet in a workbook. |
| [ForceFullCalculate](../../aspose.cells.gridjs/gridworkbooksettings/forcefullcalculate/) { get; set; } | Indicates whether fully calculates every time when a calculation is triggered. |
| [Iteration](../../aspose.cells.gridjs/gridworkbooksettings/iteration/) { get; set; } | Indicates whether use iteration to resolve circular references. |
| [MaxIteration](../../aspose.cells.gridjs/gridworkbooksettings/maxiteration/) { get; set; } | Returns or sets the maximum number of iterations to resolve a circular reference, the default value is 100. |
| [PrecisionAsDisplayed](../../aspose.cells.gridjs/gridworkbooksettings/precisionasdisplayed/) { get; set; } | True if calculations in this workbook will be done using only the precision of the numbers as they're displayed |
| [ReCalculateOnOpen](../../aspose.cells.gridjs/gridworkbooksettings/recalculateonopen/) { get; set; } | Indicates whether re-calculate all formulas on opening file. Default is true. |

### Examples

```csharp
[C#]

GridJsWorkbook g = new GridJsWorkbook();

GridWorkbookSettings gsettings = new GridWorkbookSettings();
g.Settings=gsettings;

//do your business

[Visual Basic]
Dim g as GridJsWorkbook = new GridJsWorkbook()

Dim gsettings as GridWorkbookSettings = new GridWorkbookSettings()
 g.Settings=gsettings;
 
'do your business
```

### See Also

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


