---
title: TxtLoadOptions.HasFormula
second_title: Aspose.Cells for .NET API Reference
description: TxtLoadOptions property. Indicates whether the text is formula if it starts with 
type: docs
url: /net/aspose.cells/txtloadoptions/hasformula/
---
## TxtLoadOptions.HasFormula property

Indicates whether the text is formula if it starts with "=".

```csharp
public bool HasFormula { get; set; }
```

### Examples

```csharp
// Called: HasFormula = true,
[Test]
        public void Property_HasFormula()
        {
            CsvLightCellsHandler handler = new CsvLightCellsHandler();
            Workbook wb = CSVTest.LoadAsCsv(&quot;a,1.20,b,1.3,c,true,=B1+D1\na,1.20,b,1.3,c,true,=B1+D1&quot;, new TxtLoadOptions()
            {
                LightCellsDataHandler = handler,
                HasFormula = true,
            });
            Assert.AreEqual(14, handler._cellCount, &quot;CellCount&quot;);
            Cells cells = wb.Worksheets[0].Cells;
            Assert.AreEqual(0, cells.Count, &quot;After reading, cell count in model&quot;);
        }
```

### See Also

* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


