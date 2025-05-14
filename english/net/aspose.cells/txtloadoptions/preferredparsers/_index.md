---
title: TxtLoadOptions.PreferredParsers
second_title: Aspose.Cells for .NET API Reference
description: TxtLoadOptions property. Gets and sets preferred value parsers for loading text file
type: docs
url: /net/aspose.cells/txtloadoptions/preferredparsers/
---
## TxtLoadOptions.PreferredParsers property

Gets and sets preferred value parsers for loading text file.

```csharp
public ICustomParser[] PreferredParsers { get; set; }
```

### Remarks

parsers[0] is the parser will be used for the first column in text template file, parsers[1] is the parser will be used for the second column, ...etc. The last one(parsers[parsers.length-1]) will be used for all other columns start from parsers.length-1. If one item is null, the corresponding column will be parsed by the default parser of Aspose.Cells.

### Examples

```csharp
// Called: tlo.PreferredParsers = new ICustomParser[]{ new MyParser(), null, };
public void TxtLoadOptions_Property_PreferredParsers()
{ //CELLSNET-46382
    TxtLoadOptions tlo = new TxtLoadOptions(LoadFormat.Csv);
    tlo.PreferredParsers = new ICustomParser[]{ new MyParser(), null, };
    Workbook wb = LoadAsCsv("\"2018-10-08\",2018-10-08\n\"2018-10-08\",2018-10-08", tlo);
    Cells cells = wb.Worksheets[0].Cells;
    Cell cell = cells[0, 0];
    Assert.AreEqual(CellValueType.IsString, cell.Type, "A1.Type");
    Assert.AreEqual("2018-10-08", cell.Value, "A1.Value");
    cell = cells[0, 1];
    Assert.AreEqual(CellValueType.IsDateTime, cell.Type, "B1.Type");
    Assert.AreEqual(43381, cell.IntValue, "B1.IntValue");
    cell = cells[1, 0];
    Assert.AreEqual(CellValueType.IsString, cell.Type, "A2.Type");
    Assert.AreEqual("2018-10-08", cell.Value, "A2.Value");
    cell = cells[1, 1];
    Assert.AreEqual(CellValueType.IsDateTime, cell.Type, "B2.Type");
    Assert.AreEqual(43381, cell.IntValue, "B2.IntValue");
}
```

### See Also

* interface [ICustomParser](../../icustomparser/)
* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


