---
title: Class CalculationOptions
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.CalculationOptions class. Represents options for calculation
type: docs
url: /net/aspose.cells/calculationoptions/
---
## CalculationOptions class

Represents options for calculation.

```csharp
public class CalculationOptions
```

## Constructors

| Name | Description |
| --- | --- |
| [CalculationOptions](calculationoptions/)() | The default constructor. |

## Properties

| Name | Description |
| --- | --- |
| [CalcStackSize](../../aspose.cells/calculationoptions/calcstacksize/) { get; set; } | The stack size for calculating cells recursively. Default value is 200. |
| [CalculationMonitor](../../aspose.cells/calculationoptions/calculationmonitor/) { get; set; } | The monitor for user to track the progress of formula calculation. |
| [CharacterEncoding](../../aspose.cells/calculationoptions/characterencoding/) { get; set; } | Specifies the encoding used for encoding/decoding characters when calculating formulas. For functions such as CHAR, CODE, the calculated result depends on the region settings and default charset of the environment. With this property user can specify the proper encoding used for those function to get the expected result. |
| [CustomEngine](../../aspose.cells/calculationoptions/customengine/) { get; set; } | The custom formula calculation engine to extend the default calculation engine of Aspose.Cells. |
| [CustomFunction](../../aspose.cells/calculationoptions/customfunction/) { get; set; } | (**Obsolete.**) The custom formula calculation functions to extend the calculation engine. |
| [IgnoreError](../../aspose.cells/calculationoptions/ignoreerror/) { get; set; } | Indicates whether errors encountered while calculating formulas should be ignored. The error may be unsupported function, external links, etc. The default value is true. |
| [LinkedDataSources](../../aspose.cells/calculationoptions/linkeddatasources/) { get; set; } | Specifies the data sources for external links used in formulas. |
| [PrecisionStrategy](../../aspose.cells/calculationoptions/precisionstrategy/) { get; set; } | Specifies the strategy for processing precision of calculation. |
| [Recursive](../../aspose.cells/calculationoptions/recursive/) { get; set; } | Indicates whether calculate the dependent cells recursively when calculating one cell and it depends on other cells. The default value is true. |

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


