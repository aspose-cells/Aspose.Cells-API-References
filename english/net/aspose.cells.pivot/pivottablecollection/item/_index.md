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
// Called: PivotTable pt = workbook.Worksheets[0].PivotTables[0];
[Test]
        public void Property_Int32_()
        {
            var workbook = new Workbook(Constants.PivotTableSourcePath + "CELLSNET43395.xlsx");

            PivotTable pt = workbook.Worksheets[0].PivotTables[0];
            pt.DataFields[0].DisplayName = "MyTotal of " + pt.DataFields[0].Name;
            pt.CalculateData();
            Assert.AreEqual("MyTotal of c", workbook.Worksheets[0].Cells["F9"].StringValue);
           // workbook.Save(Constants.destPath + "dest.html");
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
// Called: workbook.Worksheets["Sheet1"].PivotTables["PivotTable1"].ChangeDataSource(new[] { "'" + workbook.FileName + "'!MyRange" }); //workbook.Worksheets["Sheet1"].PivotTables["PivotTable1"].ChangeDataSource(new[] { "MyRange" });
[Test]
        public void Property_String_()
        {

            var workbook = new Workbook(Constants.PivotTableSourcePath + "CellsNet44854.xlsx");
            Console.WriteLine("Current data source: {0}", string.Join(", ", workbook.Worksheets["Sheet1"].PivotTables["PivotTable1"].DataSource));

            workbook.Worksheets["Sheet1"].Cells["C2"].PutValue(1000000);
           workbook.Worksheets["Sheet1"].PivotTables["PivotTable1"].RefreshData();
           workbook.Worksheets["Sheet1"].PivotTables["PivotTable1"].CalculateData();
            Console.WriteLine("New B20 Value: {0}", workbook.Worksheets["Sheet1"].Cells["B20"].Value);

            workbook.Worksheets["Sheet1"].PivotTables["PivotTable1"].ChangeDataSource(new[] { "'" + workbook.FileName + "'!MyRange" }); //workbook.Worksheets["Sheet1"].PivotTables["PivotTable1"].ChangeDataSource(new[] { "MyRange" });


            Console.WriteLine("New data source: {0}", string.Join(", ", workbook.Worksheets["Sheet1"].PivotTables["PivotTable1"].DataSource));

            workbook.Worksheets["Sheet1"].Cells["C2"].PutValue(2000000);
            workbook.Worksheets["Sheet1"].PivotTables["PivotTable1"].RefreshData();
           workbook.Worksheets["Sheet1"].PivotTables["PivotTable1"].CalculateData();
            Console.WriteLine("New B20 Value: {0}", workbook.Worksheets["Sheet1"].Cells["B20"].Value);
            Console.WriteLine();
            Assert.AreEqual(workbook.Worksheets["Sheet1"].PivotTables["PivotTable1"].GetSource()[0], "CellsNet44854.xlsx!MyRange");
            workbook.Save(Constants.PivotTableDestPath + "CellsNet44854.xlsx");
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


