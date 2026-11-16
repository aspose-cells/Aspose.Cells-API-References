---
title: Class PivotFieldGroupOptions
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Pivot.PivotFieldGroupOptions class. Options for pivot field grouping settings
type: docs
url: /net/aspose.cells.pivot/pivotfieldgroupoptions/
---
## PivotFieldGroupOptions class

Options for pivot field grouping settings.

```csharp
public class PivotFieldGroupOptions
```

## Constructors

| Name | Description |
| --- | --- |
| [PivotFieldGroupOptions](pivotfieldgroupoptions/)() | The default constructor. |

## Properties

| Name | Description |
| --- | --- |
| [DiscreteGroupItems](../../aspose.cells.pivot/pivotfieldgroupoptions/discretegroupitems/) { get; set; } | Gets and sets discrete group items. |
| [EndDate](../../aspose.cells.pivot/pivotfieldgroupoptions/enddate/) { get; set; } | Gets or sets the end value of the grouping range. |
| [EndNumber](../../aspose.cells.pivot/pivotfieldgroupoptions/endnumber/) { get; set; } | Gets or sets the end value of the grouping range. |
| [GroupType](../../aspose.cells.pivot/pivotfieldgroupoptions/grouptype/) { get; set; } | Gets or sets the grouping type for pivot field. Only for grouping date time pivot field. |
| [GroupTypes](../../aspose.cells.pivot/pivotfieldgroupoptions/grouptypes/) { get; set; } | Gets or sets the grouping type for pivot field. |
| [Interval](../../aspose.cells.pivot/pivotfieldgroupoptions/interval/) { get; set; } | Gets or sets the interval size for each group. |
| [IsAutoEnd](../../aspose.cells.pivot/pivotfieldgroupoptions/isautoend/) { get; set; } | Gets or sets a value indicating whether the end value is automatically determined. |
| [IsAutoStart](../../aspose.cells.pivot/pivotfieldgroupoptions/isautostart/) { get; set; } | Gets or sets a value indicating whether the start value is automatically determined. |
| [NewPivotField](../../aspose.cells.pivot/pivotfieldgroupoptions/newpivotfield/) { get; set; } | Gets or sets a value indicating whether new pivot fields should be created after grouping. |
| [StartDate](../../aspose.cells.pivot/pivotfieldgroupoptions/startdate/) { get; set; } | Gets or sets the start value of the grouping range. |
| [StartNumber](../../aspose.cells.pivot/pivotfieldgroupoptions/startnumber/) { get; set; } | Gets or sets the start value of the grouping range. |

### Examples

```csharp

[C#]

// Load the sample workbook
Workbook wb = new Workbook("sampleGroupPivotFieldsInPivotTable.xlsx");
// Access the second worksheet and its pivot table
PivotTable pt = wb.Worksheets[1].PivotTables[0];
// Group the first row field (a date field) by months and quarters
PivotFieldGroupOptions options = new PivotFieldGroupOptions();
options.StartDate = new DateTime(2008, 1, 1);
options.EndDate = new DateTime(2008, 9, 5);
options.GroupTypes = new PivotGroupByType[] { PivotGroupByType.Months, PivotGroupByType.Quarters };
pt.RowFields[0].Group(options);
// Calculate the pivot table data and save the output file
pt.CalculateData();
wb.Save("outputGroupPivotFieldsInPivotTable.xlsx");

[Visual Basic]

'Load the sample workbook
Dim wb As New Workbook("sampleGroupPivotFieldsInPivotTable.xlsx")
'Access the second worksheet and its pivot table
Dim pt As PivotTable = wb.Worksheets(1).PivotTables(0)
'Group the first row field (a date field) by months and quarters
Dim options As New PivotFieldGroupOptions()
options.StartDate = New DateTime(2008, 1, 1)
options.EndDate = New DateTime(2008, 9, 5)
options.GroupTypes = New PivotGroupByType() {PivotGroupByType.Months, PivotGroupByType.Quarters}
pt.RowFields(0).Group(options)
'Calculate the pivot table data and save the output file
pt.CalculateData()
wb.Save("outputGroupPivotFieldsInPivotTable.xlsx")
```

### See Also

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


