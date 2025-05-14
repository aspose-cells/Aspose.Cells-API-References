---
title: Cells.Find
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Finds the cell containing with the input object
type: docs
url: /net/aspose.cells/cells/find/
---
## Find(object, Cell) {#find}

Finds the cell containing with the input object.

```csharp
public Cell Find(object what, Cell previousCell)
```

| Parameter | Type | Description |
| --- | --- | --- |
| what | Object | The object to search for. The type should be int,double,DateTime,string,bool. |
| previousCell | Cell | Previous cell with the same object. This parameter can be set to null if searching from the start. |

### Return Value

Cell object.

### Remarks

Returns null (Nothing) if no cell is found.

### Examples

```csharp
// Called: cell = worksheet.Cells.Find("Marginal Tax Rate", null);
public void Cells_Method_Find()
{
    string filePath = Constants.PivotTableSourcePath + @"JAVA44628_";
    string savePath = CreateFolder(filePath);

    Workbook wb = new Workbook(filePath + "State Reconciliation.xlsx");
    Worksheet worksheet = wb.Worksheets[0];
    PivotTable pivotTable = worksheet.PivotTables[0];
    pivotTable.RefreshData();
    pivotTable.CalculateData();
    //Find the cell containing the row field text/label
    Cell cell = worksheet.Cells.Find("State Apport. Factor", null);

    //Create the style with your desired formatting
    Style style = wb.CreateStyle();
    style.Custom = "0.00%";
    style.Font.Name = "Calibri";
    style.Font.Size = 11;

    //format the row data
    pivotTable.FormatRow(cell.Row, style);

    cell = worksheet.Cells.Find("Marginal Tax Rate", null);
    //format the row data
    pivotTable.FormatRow(cell.Row, style);

    wb.Save(savePath + "out.xlsx");

    string pivotXml = GetEntryText(savePath + "out.xlsx", @"xl\pivotTables\pivotTable1.xml");
    Assert.AreNotEqual(pivotXml.IndexOf("<x v=\"6\" />"), -1);
    Assert.AreNotEqual(pivotXml.IndexOf("<x v=\"13\" />"), -1);

            
}
```

### See Also

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Find(object, Cell, FindOptions) {#find_1}

Finds the cell containing with the input object.

```csharp
public Cell Find(object what, Cell previousCell, FindOptions findOptions)
```

| Parameter | Type | Description |
| --- | --- | --- |
| what | Object | The object to search for. The type should be int,double,DateTime,string,bool. |
| previousCell | Cell | Previous cell with the same object. This parameter can be set to null if searching from the start. |
| findOptions | FindOptions | Find options |

### Return Value

Cell object.

### Remarks

Returns null (Nothing) if no cell is found.

### Examples

```csharp
// Called: Cell cell = cells.Find("abc ", null,options);
private void Cells_Method_Find(Workbook workbook)
        {
            Cells cells = workbook.Worksheets[0].Cells;
            Cell cell = cells.Find("abc ", null,options);
            testAreEqual(null, cell, caseName);
        }
```

### See Also

* class [Cell](../../cell/)
* class [FindOptions](../../findoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


