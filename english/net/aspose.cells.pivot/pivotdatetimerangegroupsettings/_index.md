---
title: Class PivotDateTimeRangeGroupSettings
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Pivot.PivotDateTimeRangeGroupSettings class. Represents the field grouped by date time range
type: docs
url: /net/aspose.cells.pivot/pivotdatetimerangegroupsettings/
---
## PivotDateTimeRangeGroupSettings class

Represents the field grouped by date time range.

```csharp
public class PivotDateTimeRangeGroupSettings : PivotFieldGroupSettings
```

## Properties

| Name | Description |
| --- | --- |
| [End](../../aspose.cells.pivot/pivotdatetimerangegroupsettings/end/) { get; } | Gets the end date time of the group. |
| [GroupByTypes](../../aspose.cells.pivot/pivotdatetimerangegroupsettings/groupbytypes/) { get; } | Gets the types of grouping by date time. |
| [Interval](../../aspose.cells.pivot/pivotdatetimerangegroupsettings/interval/) { get; } | Gets the internal of the group. |
| [Start](../../aspose.cells.pivot/pivotdatetimerangegroupsettings/start/) { get; } | Gets the start date time of the group. |
| override [Type](../../aspose.cells.pivot/pivotdatetimerangegroupsettings/type/) { get; } | Gets the data time group type. |

## Methods

| Name | Description |
| --- | --- |
| [IsGroupedBy](../../aspose.cells.pivot/pivotdatetimerangegroupsettings/isgroupedby/)(PivotGroupByType) | Check whether the field is grouped by the type. |

### Examples

```csharp
// Called: PivotDateTimeRangeGroupSettings columnRange =(PivotDateTimeRangeGroupSettings) pivotTable.ColumnFields[0].GroupSettings;
private static void Pivot_Type_PivotDateTimeRangeGroupSettings(string header, PivotTable pivotTable)
        {
            PivotDateTimeRangeGroupSettings columnRange =(PivotDateTimeRangeGroupSettings) pivotTable.ColumnFields[0].GroupSettings;

            Console.WriteLine(@"=============== {header} ================");
            if (columnRange != null)
            {

                Console.WriteLine(string.Format("Start: {0}", columnRange.Start));//"Start: {columnRange?.Start}");
                Console.WriteLine(string.Format("End: {0}", columnRange.End));//@"End: {columnRange?.End}");
                Console.WriteLine(string.Format("By: {0}", columnRange.Interval));//@"By: {columnRange?.By}");
                Console.WriteLine(string.Format("Types:{0}", String.Join(", ", columnRange.GroupByTypes)));//"Types: {String.Join(", ", columnRange?.GroupByTypes)}");
            }
            Console.WriteLine(@"=============== {header} DONE ===========");

        }
```

### See Also

* class [PivotFieldGroupSettings](../pivotfieldgroupsettings/)
* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


