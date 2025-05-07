---
title: PivotTable.CalculateData
second_title: Aspose.Cells for .NET API Reference
description: PivotTable method. Calculates pivottables data to cells
type: docs
url: /net/aspose.cells.pivot/pivottable/calculatedata/
---
## CalculateData() {#calculatedata}

Calculates pivottable's data to cells.

```csharp
public void CalculateData()
```

### Remarks

Cell.Value in the pivot range could not return the correct result if the method is not been called. This method calculates data with an inner pivot cache,not original data source. So if the data source is changed, please call RefreshData() method first.

### Examples

```csharp
// Called: pivot.CalculateData();
[Test]
        public void Method_CalculateData()
        {
            Workbook book = new Workbook();
            PivotTable pivot = CreateWithBlank(book);
            PivotField field = pivot.ColumnFields[0];
            field.FilterByLabel(PivotFilterType.CaptionNotEqual, "", "");

            pivot.RefreshData();
            pivot.CalculateData();
            pivot.RefreshDataOnOpeningFile = false;
            Assert.AreEqual("(blank)", book.Worksheets[0].Cells["D13"].StringValue);

            field.FilterByLabel(PivotFilterType.CaptionNotEqual, "(blank)", "");
            pivot.CalculateData();
            Assert.AreEqual("Grand Total", book.Worksheets[0].Cells["D13"].StringValue);

            field.FilterByLabel(PivotFilterType.CaptionNotContains, "(blank)", "");
            pivot.CalculateData();
            Assert.AreEqual("Grand Total", book.Worksheets[0].Cells["D13"].StringValue);
        }
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## CalculateData(PivotTableCalculateOption) {#calculatedata_1}

Calculating pivot tables with options

```csharp
public void CalculateData(PivotTableCalculateOption option)
```

| Parameter | Type | Description |
| --- | --- | --- |
| option | PivotTableCalculateOption |  |

### Examples

```csharp
// Called: pivotTable.CalculateData(calculateOption);
public static void Method_PivotTableCalculateOption_()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Add some data for the pivot table
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Amount");
            sheet.Cells["A2"].PutValue("Fruit");
            sheet.Cells["B2"].PutValue(50);
            sheet.Cells["A3"].PutValue("Vegetable");
            sheet.Cells["B3"].PutValue(30);
            sheet.Cells["A4"].PutValue("Fruit");
            sheet.Cells["B4"].PutValue(70);
            sheet.Cells["A5"].PutValue("Vegetable");
            sheet.Cells["B5"].PutValue(40);

            // Add a pivot table to the worksheet
            int pivotIndex = sheet.PivotTables.Add("A1:B5", "D1", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];

            // Configure the pivot table
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Category
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Amount

            // Create a PivotTableCalculateOption object
            PivotTableCalculateOption calculateOption = new PivotTableCalculateOption
            {
                RefreshData = true,
                RefreshCharts = true,
                ReserveMissingPivotItemType = ReserveMissingPivotItemType.All
            };

            // Calculate the pivot table data with the specified options
            pivotTable.CalculateData(calculateOption);

            // Save the workbook
            workbook.Save("PivotTableCalculateOptionExample.xlsx");
        }
```

### See Also

* class [PivotTableCalculateOption](../../pivottablecalculateoption/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


