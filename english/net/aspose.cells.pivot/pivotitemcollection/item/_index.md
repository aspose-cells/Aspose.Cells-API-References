---
title: PivotItemCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: PivotItemCollection property. Gets the PivotItem Object at the specific index
type: docs
url: /net/aspose.cells.pivot/pivotitemcollection/item/
---
## PivotItemCollection indexer (1 of 2)

Gets the PivotItem Object at the specific index.

```csharp
public PivotItem this[int index] { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual("Sum of d",workbook.Worksheets[0].PivotTables[0].RowFields[1].PivotItems[0].Name);
public void PivotItemCollection_Property_Item()
{
    Workbook workbook = new Workbook(Constants.PivotTableSourcePath + "example.xlsx");
    Assert.AreEqual("Sum of d",workbook.Worksheets[0].PivotTables[0].RowFields[1].PivotItems[0].Name);
}
```

### See Also

* class [PivotItem](../../pivotitem/)
* class [PivotItemCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## PivotItemCollection indexer (2 of 2)

Gets the [`PivotItem`](../../pivotitem/) by the specific name.

```csharp
public PivotItem this[string itemValue] { get; }
```

### Examples

```csharp
// Called: pvtTable.RowFields["Item"].PivotItems["CA32"].Move(0, true);
public void PivotItemCollection_Property_Item()
{
    string filePath = Constants.PivotTableSourcePath + @"NET43214And43215_";

    //Workbook workbook = new Workbook(filePath + "pivotTable_test.xls");
    //Worksheet worksheet = workbook.Worksheets[1];
    //PivotTable table = worksheet.PivotTables[0];
    //table.ColumnFields["Continent"].PivotItems["Africa"].Move(-5);//move up
    //table.RowFields["Product"].PivotItems["Maxilaku"].Move(1);//move down
    //workbook.Save(CreateFolder(filePath) + "pivotTable_test_output.xlsx");

    Workbook wb = new Workbook(filePath + @"PivotTest3.xlsx");
    Worksheet wsPivot = wb.Worksheets.Add("pvtNew Hardware");
    Worksheet wsData = wb.Worksheets["New Hardware - Yearly"];
    // get the pivottables collection for the pivot sheet
    PivotTableCollection pivotTables = wsPivot.PivotTables;
    // add PivotTable to the worksheet
    int index = pivotTables.Add("='New Hardware - Yearly'!A1:D621", "A3", "HWCounts_PivotTable");
    // get the PivotTable object
    PivotTable pvtTable = pivotTables[index];
    // add vendor row field
    pvtTable.AddFieldToArea(PivotFieldType.Row, "Vendor");
    // add item row field
    pvtTable.AddFieldToArea(PivotFieldType.Row, "Item");
    // add data field
    pvtTable.AddFieldToArea(PivotFieldType.Data, "2014");
    // turn off the subtotals for the vendor row field
    PivotField pivotField = pvtTable.RowFields["Vendor"];
    pivotField.SetSubtotals(PivotFieldSubtotalType.None, true);
    // turn off grand total
    pvtTable.ShowColumnGrandTotals = false;
    // THIS ONLY SEEMS TO MOVE 4H12 DOWN BY 1 POSITION??
    //pvtTable.RowFields["Item"].PivotItems["4H12"].Move(4);
    //Please call the PivotTable. RefreshData() and PivotTable. CalculateData() 
    //before using PivotItem.Position, PivotItem.PositionInSameParentNode  and PivotItem.Move(int count, bool isSameParent).

    pvtTable.RefreshData();
    pvtTable.CalculateData();

    pvtTable.RowFields["Item"].PivotItems["4H12"].Move(0, true);
    pvtTable.RowFields["Item"].PivotItems["DIF400"].Move(-1, true);
    //As a result of using PivotItem.PositionInSameParentNode,it will change the original sort sequence,
    //so when you use PivotItem.PositionInSameParentNode in another parent node,you need call the method named "CalculateData" again.
    pvtTable.CalculateData();
    pvtTable.RowFields["Item"].PivotItems["CA32"].Move(0, true);
    pvtTable.RowFields["Item"].PivotItems["AAA3"].Move(-1, true);
    Assert.AreEqual(wsPivot.Cells["B5"].StringValue, "4H12");
    Assert.AreEqual(wsPivot.Cells["B6"].StringValue, "DIF400");
    Assert.AreEqual(wsPivot.Cells["B11"].StringValue, "CA32");
    Assert.AreEqual(wsPivot.Cells["B12"].StringValue, "KL32");
    // save file
    wb.Save(Constants.PivotTableDestPath + @"example.xlsx");

    wb = new Workbook(filePath + @"PivotTest3.xlsx");
    wsPivot = wb.Worksheets.Add("pvtNew Hardware");
    wsData = wb.Worksheets["New Hardware - Yearly"];
    // get the pivottables collection for the pivot sheet
    pivotTables = wsPivot.PivotTables;
    // add PivotTable to the worksheet
    index = pivotTables.Add("='New Hardware - Yearly'!A1:D621", "A3", "HWCounts_PivotTable");
    // get the PivotTable object
    pvtTable = pivotTables[index];
    // add vendor row field
    pvtTable.AddFieldToArea(PivotFieldType.Row, "Vendor");
    // add item row field
    pvtTable.AddFieldToArea(PivotFieldType.Row, "Item");
    // add data field
    pvtTable.AddFieldToArea(PivotFieldType.Data, "2014");
    // turn off the subtotals for the vendor row field
    pivotField = pvtTable.RowFields["Vendor"];
    pivotField.SetSubtotals(PivotFieldSubtotalType.None, true);
    // turn off grand total
    pvtTable.ShowColumnGrandTotals = false;
    // THIS ONLY SEEMS TO MOVE 4H12 DOWN BY 1 POSITION??
    //pvtTable.RowFields["Item"].PivotItems["4H12"].Move(4);
    //Please call the PivotTable. RefreshData() and PivotTable. CalculateData() 
    //before using PivotItem.Position, PivotItem.PositionInSameParentNode  and PivotItem.Move(int count, bool isSameParent).

    pvtTable.RefreshData();
    pvtTable.CalculateData();
    pvtTable.RowFields["Item"].PivotItems["4H12"].PositionInSameParentNode = 1;
    pvtTable.RowFields["Item"].PivotItems["DIF400"].PositionInSameParentNode = 2;
    //As a result of using PivotItem.PositionInSameParentNode,it will change the original sort sequence,
    //so when you use PivotItem.PositionInSameParentNode in another parent node,you need call the method named "CalculateData" again.
    pvtTable.CalculateData();
    pvtTable.RowFields["Item"].PivotItems["CA32"].PositionInSameParentNode = 1;
    pvtTable.RowFields["Item"].PivotItems["AAA3"].PositionInSameParentNode = 2;
    Assert.AreEqual(wsPivot.Cells["B5"].StringValue, "4H12");
    Assert.AreEqual(wsPivot.Cells["B6"].StringValue, "DIF400");
    Assert.AreEqual(wsPivot.Cells["B11"].StringValue, "CA32");
    Assert.AreEqual(wsPivot.Cells["B12"].StringValue, "KL32");
    wb.Save(Constants.PivotTableDestPath + @"example.xlsx");
}
```

### See Also

* class [PivotItem](../../pivotitem/)
* class [PivotItemCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


