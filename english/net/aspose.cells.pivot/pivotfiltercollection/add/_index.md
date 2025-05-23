---
title: PivotFilterCollection.Add
second_title: Aspose.Cells for .NET API Reference
description: PivotFilterCollection method. Adds a PivotFilter Object to the specific type
type: docs
url: /net/aspose.cells.pivot/pivotfiltercollection/add/
---
## PivotFilterCollection.Add method

Adds a PivotFilter Object to the specific type

```csharp
[Obsolete("Use PivotFilterCollection.AddValueFilter(),AddTop10Filter(),AddLabelFilter() and AddDateFilter() methods,instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(int fieldIndex, PivotFilterType type)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | Int32 | the PivotField index |
| type | PivotFilterType | the PivotFilter type |

### Return Value

the index of the PivotFilter Object in this PivotFilterCollection.

### Remarks

NOTE: This method is now obsolete. Instead, please use PivotFilterCollection.AddValueFilter(),AddTop10Filter(),AddLabelFilter() and AddDateFilter() methods. This method will be removed 12 months later since November 2024. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
// Called: int filterIndex = pivot.PivotFilters.Add(0, PivotFilterType.Count);
public static void PivotFilterCollection_Method_Add()
        {
            // Create a new workbook
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            Cells cells = sheet.Cells;

            // Populate the worksheet with sample data
            cells[0, 0].Value = "fruit";
            cells[1, 0].Value = "grape";
            cells[2, 0].Value = "blueberry";
            cells[3, 0].Value = "kiwi";
            cells[4, 0].Value = "cherry";
            cells[5, 0].Value = "grape";
            cells[6, 0].Value = "blueberry";
            cells[7, 0].Value = "kiwi";
            cells[8, 0].Value = "cherry";

            cells[0, 1].Value = "year";
            cells[1, 1].Value = 2020;
            cells[2, 1].Value = 2020;
            cells[3, 1].Value = 2020;
            cells[4, 1].Value = 2020;
            cells[5, 1].Value = 2021;
            cells[6, 1].Value = 2021;
            cells[7, 1].Value = 2021;
            cells[8, 1].Value = 2021;

            cells[0, 2].Value = "amount";
            cells[1, 2].Value = 50;
            cells[2, 2].Value = 60;
            cells[3, 2].Value = 70;
            cells[4, 2].Value = 80;
            cells[5, 2].Value = 90;
            cells[6, 2].Value = 100;
            cells[7, 2].Value = 110;
            cells[8, 2].Value = 120;

            // Add a pivot table to the worksheet
            PivotTableCollection pivots = sheet.PivotTables;
            int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
            PivotTable pivot = pivots[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
            pivot.AddFieldToArea(PivotFieldType.Column, "year");
            pivot.AddFieldToArea(PivotFieldType.Data, "amount");

            // Set pivot table style
            pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

            // Add a pivot filter
            int filterIndex = pivot.PivotFilters.Add(0, PivotFilterType.Count);
            PivotFilter filter = pivot.PivotFilters[filterIndex];
            filter.AutoFilter.FilterTop10(0, false, false, 2);

            // Set additional properties for the pivot filter
            filter.Value1 = "SampleValue1";
            filter.Value2 = "SampleValue2";
            filter.MeasureFldIndex = 1;
            filter.MemberPropertyFieldIndex = 2;
            filter.Name = "SampleFilter";
            filter.EvaluationOrder = 1;

            // Refresh and calculate the pivot table data
            pivot.RefreshData();
            pivot.CalculateData();

            // Save the workbook
            book.Save("PivotFilterExample.xlsx");
        }
```

### See Also

* enum [PivotFilterType](../../pivotfiltertype/)
* class [PivotFilterCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


