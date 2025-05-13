---
title: PivotFieldCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: PivotFieldCollection property. Gets the PivotField Object at the specific index
type: docs
url: /net/aspose.cells.pivot/pivotfieldcollection/item/
---
## PivotFieldCollection indexer (1 of 2)

Gets the PivotField Object at the specific index.

```csharp
public PivotField this[int index] { get; }
```

### Examples

```csharp
// Called: pt.RowFields[0].IsAutoSort = true;
public void PivotFieldCollection_Property_Item()
{
    Workbook workbook = new Workbook(Constants.openPivottablePath + "SR3.xls");

    Worksheet ws = workbook.Worksheets[1];
    PivotTable pt = ws.PivotTables[(ws.PivotTables.Add("'Grid Results'!B4:E8", 2, 0, "Hello"))];
    pt.AddFieldToArea(PivotFieldType.Row, 1);
    pt.AddFieldToArea(PivotFieldType.Data, 0);
    pt.RowFields[0].IsAutoSort = true;
    workbook.Save(Constants.savePivottablePath + "c.xls");
    //workbook.Save("D:\\c.xlsx", FileFormatType.Xlsx);
}
```

### See Also

* class [PivotField](../../pivotfield/)
* class [PivotFieldCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## PivotFieldCollection indexer (2 of 2)

Gets the PivotField Object of the specific name.

```csharp
public PivotField this[string name] { get; }
```

### Examples

```csharp
// Called: pTable.DataFields["LTM Jan-17"].IsAutoSort = true;
public void PivotFieldCollection_Property_Item()
{
    string filePath = Constants.PivotTableSourcePath + @"NET46387_";

    Workbook wb = new Workbook(filePath + @"UnsortedSamleData1.xlsb");
    Worksheet ws = wb.Worksheets[1];
    var pTable = ws.PivotTables[0];
    //pTable.RefreshData();
    //Sort column LTM Jan-17 by Account Description row 
    pTable.RowFields[2].IsAutoSort = true;
    pTable.RowFields[2].IsAscendSort = false;
    pTable.RowFields[2].AutoSortField = 43;


    pTable.DataFields["LTM Jan-17"].IsAscendSort = false;
    pTable.DataFields["LTM Jan-17"].IsAutoSort = true;

    pTable.RefreshDataOnOpeningFile = true;
    pTable.CalculateData();

    string savePath = CreateFolder(filePath);
    wb.Save(savePath + @"out.Xlsb", SaveFormat.Xlsb);
    wb.Save(savePath + @"out.Xlsx", SaveFormat.Xlsx);

    wb = new Workbook(savePath + "out.Xlsb");
    Assert.AreEqual(wb.Worksheets[1].PivotTables[0].RowFields[2].IsAscendSort, false);
    Assert.AreEqual(wb.Worksheets[1].PivotTables[0].RowFields[2].AutoSortField, 43);
}
```

### See Also

* class [PivotField](../../pivotfield/)
* class [PivotFieldCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


