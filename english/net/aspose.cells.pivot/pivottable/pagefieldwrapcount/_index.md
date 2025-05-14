---
title: PivotTable.PageFieldWrapCount
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Gets the number of page fields in each column or row in the PivotTable report
type: docs
url: /net/aspose.cells.pivot/pivottable/pagefieldwrapcount/
---
## PivotTable.PageFieldWrapCount property

Gets the number of page fields in each column or row in the PivotTable report.

```csharp
public int PageFieldWrapCount { get; set; }
```

### Examples

```csharp
// Called: pivotTable.PageFieldWrapCount = (0);
public void PivotTable_Property_PageFieldWrapCount()
{
    Workbook workbook = new Workbook();

    // put in data
    Worksheet data = workbook.Worksheets.Add("data");
    data.Cells["A1"].PutValue("Country");
    data.Cells["B1"].PutValue("Product");
    data.Cells["C1"].PutValue("Vendor");
    data.Cells["D1"].PutValue("Value");
    data.Cells["E1"].PutValue("Units");
    data.Cells["A2"].PutValue("USA");
    data.Cells["B2"].PutValue("Car");
    data.Cells["C2"].PutValue("Ford");
    data.Cells["D2"].PutValue(1200.987654321);
    data.Cells["E2"].PutValue(3);
    data.Cells["A3"].PutValue("Japan");
    data.Cells["B3"].PutValue("Bike");
    data.Cells["C3"].PutValue("Yamaha");
    data.Cells["D3"].PutValue(985.123456789);
    data.Cells["E3"].PutValue(2);

    // create pivot
    Worksheet pivot = workbook.Worksheets.Add("pivot");
    PivotTableCollection pivotTables = pivot.PivotTables;
    int index = pivotTables.Add("=data!A1:E3", "A1", "pivotTable1",false,true);
    PivotTable pivotTable = pivotTables[index];
    pivotTable.ShowRowGrandTotals = (false);
    pivotTable.ShowColumnGrandTotals = (true);
    pivotTable.IsGridDropZones = (true);
    pivotTable.RefreshDataOnOpeningFile = (false);
    pivotTable.AddFieldToArea(PivotFieldType.Row, "Country");
    pivotTable.AddFieldToArea(PivotFieldType.Column, "Product");
    pivotTable.AddFieldToArea(PivotFieldType.Page, "Vendor");
    pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
    pivotTable.AddFieldToArea(PivotFieldType.Data, "Units");



    pivotTable.AddCalculatedField("Price", "'Value' / 'Units'");
    Assert.IsFalse(pivotTable.BaseFields[5].ShowCompact);
    // recalculate data in pivot according to new setup
    pivotTable.CalculateRange();
    pivotTable.CalculateData();
    pivotTable.PageFieldWrapCount = (0);
    Assert.AreEqual("Country", pivot.Cells["A4"].StringValue);
    workbook.Save(Constants.PivotTableDestPath + "example.xlsx");
}
```

### See Also

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


