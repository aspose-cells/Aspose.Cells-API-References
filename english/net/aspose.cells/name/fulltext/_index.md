---
title: Name.FullText
second_title: Aspose.Cells for .NET API Reference
description: Name property. Gets the name full text of the object with the scope setting
type: docs
url: /net/aspose.cells/name/fulltext/
---
## Name.FullText property

Gets the name full text of the object with the scope setting.

```csharp
public string FullText { get; }
```

### Examples

```csharp
// Called: var sourceRange = workbook.Worksheets.GetRangeByName(stockPriceRow.FullText);
[Test]
        public void Property_FullText()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET-54113.xlsx&quot;);
            Worksheet model = workbook.Worksheets[&quot;Model&quot;];

            var stockPriceRow = workbook.Worksheets.Names[&quot;MO_VA_StockPrice_TradingCurrency&quot;];
            var sourceRange = workbook.Worksheets.GetRangeByName(stockPriceRow.FullText);
            var destinationRange = workbook.Worksheets[&quot;Model&quot;].Cells.CreateRange(&quot;9:9&quot;);

            model.Cells.InsertCutCells(sourceRange, destinationRange.FirstRow, destinationRange.FirstColumn, ShiftType.Down);

            Assert.AreEqual(&quot;=SUM(E5,E6,E7,E5:E7)&quot;, model.Cells[&quot;E8&quot;].Formula);
            var calculationOptions = new CalculationOptions { IgnoreError = true };
            workbook.CalculateFormula(calculationOptions);

            Assert.AreEqual(&quot;12&quot;, model.Cells[&quot;E8&quot;].StringValue);
        }
```

### See Also

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


