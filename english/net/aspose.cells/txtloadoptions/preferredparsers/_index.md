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
[Test]
        public void Property_PreferredParsers()
        { //CELLSNET-46382
            TxtLoadOptions tlo = new TxtLoadOptions(LoadFormat.Csv);
            tlo.PreferredParsers = new ICustomParser[]{ new MyParser(), null, };
            Workbook wb = LoadAsCsv(&quot;\&quot;2018-10-08\&quot;,2018-10-08\n\&quot;2018-10-08\&quot;,2018-10-08&quot;, tlo);
            Cells cells = wb.Worksheets[0].Cells;
            Cell cell = cells[0, 0];
            Assert.AreEqual(CellValueType.IsString, cell.Type, &quot;A1.Type&quot;);
            Assert.AreEqual(&quot;2018-10-08&quot;, cell.Value, &quot;A1.Value&quot;);
            cell = cells[0, 1];
            Assert.AreEqual(CellValueType.IsDateTime, cell.Type, &quot;B1.Type&quot;);
            Assert.AreEqual(43381, cell.IntValue, &quot;B1.IntValue&quot;);
            cell = cells[1, 0];
            Assert.AreEqual(CellValueType.IsString, cell.Type, &quot;A2.Type&quot;);
            Assert.AreEqual(&quot;2018-10-08&quot;, cell.Value, &quot;A2.Value&quot;);
            cell = cells[1, 1];
            Assert.AreEqual(CellValueType.IsDateTime, cell.Type, &quot;B2.Type&quot;);
            Assert.AreEqual(43381, cell.IntValue, &quot;B2.IntValue&quot;);
        }
```

### See Also

* interface [ICustomParser](../../icustomparser/)
* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


