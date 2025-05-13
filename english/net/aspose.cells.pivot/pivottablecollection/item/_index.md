---
title: PivotTableCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: PivotTableCollection property. Gets the PivotTable report by index
type: docs
url: /net/aspose.cells.pivot/pivottablecollection/item/
---
## PivotTableCollection indexer (1 of 3)

Gets the PivotTable report by index.

```csharp
public PivotTable this[int index] { get; }
```

### Examples

```csharp
// Called: workbook.Worksheets[0].PivotTables[0].CalculateData();
public void PivotTableCollection_Property_Item()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    workbook.Worksheets[0].PivotTables[0].CalculateData();
    Assert.AreEqual(workbook.Worksheets[0].Cells["B3"].GetStyle().IsTextWrapped, true);
}
```

### See Also

* class [PivotTable](../../pivottable/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## PivotTableCollection indexer (2 of 3)

Gets the PivotTable report by pivottable's name.

```csharp
public PivotTable this[string name] { get; }
```

### Examples

```csharp
// Called: workbook.Worksheets["Sheet1"].PivotTables["PivotTable1"].CalculateData();
private void PivotTableCollection_Property_Item(string fileName, string outName)
        {
            Console.WriteLine(fileName);
            var workbook = new Workbook(fileName);
            Console.WriteLine("Current data source: {0}", string.Join(", ", workbook.Worksheets["Sheet1"].PivotTables["PivotTable1"].DataSource));

            workbook.Worksheets["Sheet1"].Cells["C2"].PutValue(1000000);
            workbook.Worksheets["Sheet1"].PivotTables["PivotTable1"].RefreshData();
            workbook.Worksheets["Sheet1"].PivotTables["PivotTable1"].CalculateData();
            workbook.Worksheets["Sheet1"].PivotTables["PivotTable1"].RefreshDataOnOpeningFile = true;
            Console.WriteLine("New B20 Value: {0}", workbook.Worksheets["Sheet1"].Cells["B20"].Value);

            //workbook.Worksheets.Names["MyRange"].RefersTo

            //workbook.Worksheets["Sheet1"].PivotTables["PivotTable1"].ChangeDataSource(new[] { workbook.Worksheets.Names["MyRange"].RefersTo });
            workbook.Worksheets["Sheet1"].PivotTables["PivotTable1"].ChangeDataSource(new[] { "MyRange" });

            Console.WriteLine("New data source: {0}", string.Join(", ", workbook.Worksheets["Sheet1"].PivotTables["PivotTable1"].DataSource));

            workbook.Worksheets["Sheet1"].Cells["C2"].PutValue(2000000);
            workbook.Worksheets["Sheet1"].PivotTables["PivotTable1"].RefreshData();
            workbook.Worksheets["Sheet1"].PivotTables["PivotTable1"].CalculateData();
            workbook.Worksheets["Sheet1"].PivotTables["PivotTable1"].RefreshDataOnOpeningFile = true;
            Console.WriteLine("New B20 Value: {0}", workbook.Worksheets["Sheet1"].Cells["B20"].Value);
            Console.WriteLine();

            workbook.Save(Constants.PIVOT_CHECK_FILE_PATH + outName);
        }
```

### See Also

* class [PivotTable](../../pivottable/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## PivotTableCollection indexer (3 of 3)

Gets the PivotTable report by pivottable's position.

```csharp
public PivotTable this[int row, int column] { get; }
```

### See Also

* class [PivotTable](../../pivottable/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


