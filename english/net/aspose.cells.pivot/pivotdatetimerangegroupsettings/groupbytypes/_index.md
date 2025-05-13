---
title: PivotDateTimeRangeGroupSettings.GroupByTypes
second_title: Aspose.Cells for .NET API Reference
description: PivotDateTimeRangeGroupSettings property. Gets the types of grouping by date time
type: docs
url: /net/aspose.cells.pivot/pivotdatetimerangegroupsettings/groupbytypes/
---
## PivotDateTimeRangeGroupSettings.GroupByTypes property

Gets the types of grouping by date time.

```csharp
public PivotGroupByType[] GroupByTypes { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(PivotGroupByType.Months, dateTimeGroup.GroupByTypes[0]);
public void PivotDateTimeRangeGroupSettings_Property_GroupByTypes()
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

* enum [PivotGroupByType](../../pivotgroupbytype/)
* class [PivotDateTimeRangeGroupSettings](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


