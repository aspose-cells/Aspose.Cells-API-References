---
title: PivotField.IsAscendSort
second_title: Aspose.Cells for .NET API Reference
description: PivotField property. Indicates whether the specified PivotTable field is autosorted ascending
type: docs
url: /net/aspose.cells.pivot/pivotfield/isascendsort/
---
## PivotField.IsAscendSort property

Indicates whether the specified PivotTable field is autosorted ascending.

```csharp
public bool IsAscendSort { get; set; }
```

### Examples

```csharp
// Called: pivotField.IsAscendSort = true;
[Test]
        public void Property_IsAscendSort()
        {

            Workbook workbook = new Workbook(Constants.PivotTableSourcePath + &quot;TestUserPivot158653.xls&quot;);//source sheet

            Worksheet failuresheet = workbook.Worksheets[&quot;Failures&quot;];

            PivotTableCollection pivotTables = failuresheet.PivotTables;

            int index = pivotTables.Add(&quot;=A1:U142&quot;, &quot;A150&quot;, &quot;PivotTable2&quot;);

            PivotTable pivotTable = pivotTables[index];

            pivotTable.AddFieldToArea(PivotFieldType.Row, 8);

            pivotTable.AddFieldToArea(PivotFieldType.Data, 9);



            PivotFieldCollection pivotFields = pivotTable.RowFields;

            PivotField pivotField = pivotFields[0];



            pivotField.IsAutoSort = true;

            pivotField.IsAscendSort = true;

            pivotField.AutoSortField = 0;



            workbook.Save(Constants.PivotTableDestPath + &quot;TestUserPivot158653.xls&quot;);
        }
```

### See Also

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


