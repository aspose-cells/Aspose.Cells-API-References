---
title: PivotDateTimeRangeGroupSettings.IsGroupedBy
second_title: Aspose.Cells for .NET API Reference
description: PivotDateTimeRangeGroupSettings method. Check whether the field is grouped by the type
type: docs
url: /net/aspose.cells.pivot/pivotdatetimerangegroupsettings/isgroupedby/
---
## PivotDateTimeRangeGroupSettings.IsGroupedBy method

Check whether the field is grouped by the type.

```csharp
public bool IsGroupedBy(PivotGroupByType type)
```

| Parameter | Type | Description |
| --- | --- | --- |
| type | PivotGroupByType | The group type |

### Examples

```csharp
// Called: Assert.IsTrue(dateTimeGroup.IsGroupedBy(PivotGroupByType.Months));
[Test]
        public void Method_PivotGroupByType_()
        {
            Workbook wb = new Workbook(Constants.openPivottablePath + &quot;AsposeShowCompact.xls&quot;);
            PivotTable table = wb.Worksheets[1].PivotTables[0];
            PivotField field = table.RowFields[0];

            //Assert.AreEqual(field.ShowCompact, true);


            wb = new Workbook(Constants.openPivottablePath + &quot;AsposeGroup.xls&quot;);
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


