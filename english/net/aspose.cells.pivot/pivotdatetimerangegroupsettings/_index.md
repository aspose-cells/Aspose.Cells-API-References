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
// Called: PivotDateTimeRangeGroupSettings dateTimeGroup = (PivotDateTimeRangeGroupSettings)settings;
[Test]
        public void Type_PivotDateTimeRangeGroupSettings()
        {
            Workbook wb = new Workbook(Constants.openPivottablePath + "AsposeShowCompact.xls");
            PivotTable table = wb.Worksheets[1].PivotTables[0];
            PivotField field = table.RowFields[0];

            //Assert.AreEqual(field.ShowCompact, true);


            wb = new Workbook(Constants.openPivottablePath + "AsposeGroup.xls");
            table = wb.Worksheets[0].PivotTables[0];
            field = table.RowFields[0];

            //Assert.AreEqual(field.Range.IsAutoStart, false);
            //Assert.AreEqual(field.Range.IsAutoEnd, true);
           PivotFieldGroupSettings settings = field.GroupSettings;
            Assert.AreEqual(PivotFieldGroupType.DateTimeRange, settings.Type);
            PivotDateTimeRangeGroupSettings dateTimeGroup = (PivotDateTimeRangeGroupSettings)settings;
           
            Assert.AreEqual(PivotGroupByType.Months, dateTimeGroup.GroupByTypes[0]);
            Assert.IsTrue(dateTimeGroup.IsGroupedBy(PivotGroupByType.Months));
        }
```

### See Also

* class [PivotFieldGroupSettings](../pivotfieldgroupsettings/)
* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


