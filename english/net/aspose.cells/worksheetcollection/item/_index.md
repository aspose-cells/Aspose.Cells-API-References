---
title: WorksheetCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: WorksheetCollection property. Gets the Worksheet element at the specified index
type: docs
url: /net/aspose.cells/worksheetcollection/item/
---
## WorksheetCollection indexer (1 of 2)

Gets the [`Worksheet`](../../worksheet/) element at the specified index.

```csharp
public Worksheet this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The zero based index of the element. |

### Return Value

The element at the specified index.

### Examples

```csharp
// Called: Cells cells = workbook.Worksheets[0].Cells;
public void WorksheetCollection_Property_Item()
{
    Workbook workbook = new Workbook();
    Cells cells = workbook.Worksheets[0].Cells;
    Cell cell = cells[0, 0];
    cell.Formula = "=DATEDIF(\"2001-6-1\",\"2002-8-15\",\"YD\")";
    Console.WriteLine("=DATEDIF(\"2001-6-1\",\"2002-8-15\",\"YD\")");
    workbook.CalculateFormula();
    Assert.AreEqual(75, cell.IntValue); //=DATEDIF("2001-6-1","2002-8-15","YD")
}
```

### See Also

* class [Worksheet](../../worksheet/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## WorksheetCollection indexer (2 of 2)

Gets the [`Worksheet`](../../worksheet/) element with the specified name.

```csharp
public Worksheet this[string sheetName] { get; }
```

| Parameter | Description |
| --- | --- |
| sheetName | Worksheet name |

### Return Value

The element with the specified name.

### Examples

```csharp
// Called: Cells cells = workbook.Worksheets["AsposeResult"].Cells;
public void WorksheetCollection_Property_Item()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xls");
    Cells cells = workbook.Worksheets["AsposeResult"].Cells;
    cells.InsertColumn(5);

    CheckInsertColumn_Hyperlink_001(workbook);
    workbook.Save(Constants.destPath + " testInsertColumn.xls");
    workbook = new Workbook(Constants.destPath + " testInsertColumn.xls");
    CheckInsertColumn_Hyperlink_001(workbook);
    workbook.Save(Constants.destPath + " testInsertColumn.xlsx");
    workbook = new Workbook(Constants.destPath + " testInsertColumn.xlsx");
    CheckInsertColumn_Hyperlink_001(workbook);
    workbook.Save(Constants.destPath + " testInsertColumn.xml", SaveFormat.SpreadsheetML);
    workbook = new Workbook(Constants.destPath + " testInsertColumn.xml");
    CheckInsertColumn_Hyperlink_001(workbook);
    workbook.Save(Constants.destPath + " testInsertColumn.xls");
}
```

### See Also

* class [Worksheet](../../worksheet/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


