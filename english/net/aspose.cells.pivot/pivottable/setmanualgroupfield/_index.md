---
title: PivotTable.SetManualGroupField
second_title: Aspose.Cells for .NET API Reference
description: PivotTable method. Sets manual field group by the PivotTable
type: docs
url: /net/aspose.cells.pivot/pivottable/setmanualgroupfield/
---
## SetManualGroupField(int, double, double, ArrayList, double) {#setmanualgroupfield_2}

Sets manual field group by the PivotTable.

```csharp
[Obsolete("Use PivotField.GroupBy() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void SetManualGroupField(int baseFieldIndex, double startVal, double endVal, 
    ArrayList groupByList, double intervalNum)
```

| Parameter | Type | Description |
| --- | --- | --- |
| baseFieldIndex | Int32 | The row or column field index in the base fields |
| startVal | Double | Specifies the starting value for numeric grouping. |
| endVal | Double | Specifies the ending value for numeric grouping. |
| groupByList | ArrayList | Specifies the grouping type list. Specified by PivotTableGroupType |
| intervalNum | Double | Specifies the interval number group by numeric grouping. |

### Remarks

NOTE: This method is now obsolete. Instead, please use PivotField.GroupBy() method. This method will be removed 12 months later since October 2023. Aspose apologizes for any inconvenience you may have experienced.

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## SetManualGroupField(PivotField, double, double, ArrayList, double) {#setmanualgroupfield}

Sets manual field group by the PivotTable.

```csharp
[Obsolete("Use PivotField.GroupBy() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void SetManualGroupField(PivotField pivotField, double startVal, double endVal, 
    ArrayList groupByList, double intervalNum)
```

| Parameter | Type | Description |
| --- | --- | --- |
| pivotField | PivotField | The row or column field in the base fields |
| startVal | Double | Specifies the starting value for numeric grouping. |
| endVal | Double | Specifies the ending value for numeric grouping. |
| groupByList | ArrayList | Specifies the grouping type list. Specified by PivotTableGroupType |
| intervalNum | Double | Specifies the interval number group by numeric grouping. |

### Remarks

NOTE: This method is now obsolete. Instead, please use PivotField.GroupBy() method. This method will be removed 12 months later since October 2023. Aspose apologizes for any inconvenience you may have experienced.

### See Also

* class [PivotField](../../pivotfield/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## SetManualGroupField(int, DateTime, DateTime, ArrayList, int) {#setmanualgroupfield_3}

Sets manual field group by the PivotTable.

```csharp
[Obsolete("Use PivotField.GroupBy() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void SetManualGroupField(int baseFieldIndex, DateTime startVal, DateTime endVal, 
    ArrayList groupByList, int intervalNum)
```

| Parameter | Type | Description |
| --- | --- | --- |
| baseFieldIndex | Int32 | The row or column field index in the base fields |
| startVal | DateTime | Specifies the starting value for date grouping. |
| endVal | DateTime | Specifies the ending value for date grouping. |
| groupByList | ArrayList | Specifies the grouping type list. Specified by PivotTableGroupType |
| intervalNum | Int32 | Specifies the interval number group by in days grouping.The number of days must be positive integer of nonzero |

### Remarks

NOTE: This method is now obsolete. Instead, please use PivotField.GroupBy() method. This method will be removed 12 months later since October 2023. Aspose apologizes for any inconvenience you may have experienced.

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## SetManualGroupField(PivotField, DateTime, DateTime, ArrayList, int) {#setmanualgroupfield_1}

Sets manual field group by the PivotTable.

```csharp
[Obsolete("Use PivotField.GroupBy() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void SetManualGroupField(PivotField pivotField, DateTime startVal, DateTime endVal, 
    ArrayList groupByList, int intervalNum)
```

| Parameter | Type | Description |
| --- | --- | --- |
| pivotField | PivotField | The row or column field in the base fields |
| startVal | DateTime | Specifies the starting value for date grouping. |
| endVal | DateTime | Specifies the ending value for date grouping. |
| groupByList | ArrayList | Specifies the grouping type list. Specified by PivotTableGroupType |
| intervalNum | Int32 | Specifies the interval number group by in days grouping.The number of days must be positive integer of nonzero |

### Remarks

NOTE: This method is now obsolete. Instead, please use PivotField.GroupBy() method. This method will be removed 12 months later since October 2023. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
// Called: pivotTable.SetManualGroupField(pivotTable.BaseFields[1], startDate, endDate, groupByList, 1);
[Test]
        public void Method_Int32_()
        {
            Workbook workbook = new Workbook(Constants.PivotTableSourcePath + &quot;CELLSJAVA45772.xlsx&quot;);
            Worksheet sheet = workbook.Worksheets[0];
            PivotTableCollection pivotTables = sheet.PivotTables;

            int index = pivotTables.Add(&quot;=Sheet1!A1:D6&quot;, &quot;I1&quot;, &quot;PivotTable1&quot;);

            PivotTable pivotTable = pivotTables[index];

            pivotTable.AddFieldToArea(PivotFieldType.Data, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Page, 2);
            int rowFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, 1);
            int columnFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Column, 3);

            pivotTable.RowFields[rowFieldIndex].ShowInOutlineForm = (true);
            pivotTable.RowFields[rowFieldIndex].ShowCompact = (true);
            pivotTable.ColumnFields[columnFieldIndex].ShowInOutlineForm = (true);
            pivotTable.ColumnFields[columnFieldIndex].ShowCompact = (true);

            ArrayList groupByList = new ArrayList();
            groupByList.Add(PivotGroupByType.Hours);
            groupByList.Add(PivotGroupByType.Months);
            groupByList.Add(PivotGroupByType.Minutes);
            groupByList.Add(PivotGroupByType.Quarters);
            groupByList.Add(PivotGroupByType.Seconds);
            groupByList.Add(PivotGroupByType.Days);
            groupByList.Add(PivotGroupByType.Years);

            DateTime startDate = new DateTime(2008, 1, 13, 0, 32, 14);//     sdf.parse(&quot;1/13/2008 00:32:14&quot;));
            DateTime endDate = new DateTime(2014, 7, 5, 1, 0, 0);// sdf.parse(&quot;7/5/2014 01:00:00&quot;));
            pivotTable.SetManualGroupField(pivotTable.BaseFields[1], startDate, endDate, groupByList, 1);
            Assert.AreEqual(&quot;&lt;2008-01-13&quot;, pivotTable.BaseFields[6].PivotItems[0].GetStringValue());
            //groupByList = new ArrayList();
            //groupByList.Add(PivotGroupByType.RangeOfValues);
            //pivotTable.SetManualGroupField(pivotTable.BaseFields[3], 1.1, 9.54, groupByList, 0.235);
            workbook.Save(Constants.PivotTableDestPath + &quot;CELLSJAVA45772.xlsx&quot;);
        }
```

### See Also

* class [PivotField](../../pivotfield/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


