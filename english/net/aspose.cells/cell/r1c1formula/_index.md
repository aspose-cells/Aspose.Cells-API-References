---
title: Cell.R1C1Formula
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Gets or sets a R1C1 formula of the Cell
type: docs
url: /net/aspose.cells/cell/r1c1formula/
---
## Cell.R1C1Formula property

Gets or sets a R1C1 formula of the [`Cell`](../).

```csharp
public string R1C1Formula { get; set; }
```

### Examples

```csharp
// Called: cell.R1C1Formula = "=INDIRECT(R1C1,true)";
[Test]
        public void Property_R1C1Formula()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            cells[0, 0].PutValue("R1C2");
            cells[0, 1].PutValue(1.333);
            Cell cell = cells[0, 2];
            cell.R1C1Formula = "=INDIRECT(R1C1,true)";
            workbook.CalculateFormula();
            Assert.AreEqual("#REF!", cell.StringValue);
        }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


