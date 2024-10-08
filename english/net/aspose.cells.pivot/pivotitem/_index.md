---
title: Class PivotItem
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Pivot.PivotItem class. Represents a item in a PivotField report
type: docs
url: /net/aspose.cells.pivot/pivotitem/
---
## PivotItem class

Represents a item in a PivotField report.

```csharp
public class PivotItem
```

## Properties

| Name | Description |
| --- | --- |
| [Index](../../aspose.cells.pivot/pivotitem/index/) { get; set; } | Gets the index of the pivot item in cache field. |
| [IsFormula](../../aspose.cells.pivot/pivotitem/isformula/) { get; set; } | Indicates whether this pivot item is a calculated formula item. |
| [IsHidden](../../aspose.cells.pivot/pivotitem/ishidden/) { get; set; } | Gets and Sets whether the pivot item is hidden. |
| [IsHideDetail](../../aspose.cells.pivot/pivotitem/ishidedetail/) { get; set; } | Gets and Sets whether the pivot item hides detail. |
| [IsMissing](../../aspose.cells.pivot/pivotitem/ismissing/) { get; } | Indicates whether the item is removed from the data source. |
| [Name](../../aspose.cells.pivot/pivotitem/name/) { get; set; } |  |
| [Position](../../aspose.cells.pivot/pivotitem/position/) { get; set; } | Specifying the position index in all the PivotItems,not the PivotItems under the same parent node. |
| [PositionInSameParentNode](../../aspose.cells.pivot/pivotitem/positioninsameparentnode/) { get; set; } | Specifying the position index in the PivotItems under the same parent node. |
| [Value](../../aspose.cells.pivot/pivotitem/value/) { get; } | Gets the value of the pivot item |

## Methods

| Name | Description |
| --- | --- |
| [GetDateTimeValue](../../aspose.cells.pivot/pivotitem/getdatetimevalue/)() | Gets the date time value of the pivot item If the value is null ,it will return DateTime.MinValue |
| [GetDoubleValue](../../aspose.cells.pivot/pivotitem/getdoublevalue/)() | Gets the double value of the pivot item If the value is null or not number ,it will return 0 |
| [GetFormula](../../aspose.cells.pivot/pivotitem/getformula/)() | Gets the formula of this calculated item. Only works when this item is calculated item. |
| [GetStringValue](../../aspose.cells.pivot/pivotitem/getstringvalue/)() | Gets the string value of the pivot item If the value is null, it will return "" |
| [Move](../../aspose.cells.pivot/pivotitem/move/)(int, bool) | Moves the item up or down |

### See Also

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


