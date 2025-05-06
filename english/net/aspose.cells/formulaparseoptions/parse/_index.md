---
title: FormulaParseOptions.Parse
second_title: Aspose.Cells for .NET API Reference
description: FormulaParseOptions property. Whether parse given formula. Default is true. If it is false then given formula string will be kept as it is for the cell until user call other methods to parse them or parsed formula data is required by other operations such as calculating formulas
type: docs
url: /net/aspose.cells/formulaparseoptions/parse/
---
## FormulaParseOptions.Parse property

Whether parse given formula. Default is true. If it is false, then given formula string will be kept as it is for the cell until user call other methods to parse them or parsed formula data is required by other operations such as calculating formulas.

```csharp
public bool Parse { get; set; }
```

### Examples

```csharp
// Called: cells[&amp;quot;B7&amp;quot;].SetFormula(&amp;quot;=A2&amp;quot;, new FormulaParseOptions() { Parse = false }, null);
[Test]
        public void Property_Parse()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            cells[&quot;B7&quot;].SetFormula(&quot;=A2&quot;, new FormulaParseOptions() { Parse = false }, null);
            cells[0, 1].SetFormula(&quot;=B7-C7&quot;, new FormulaParseOptions() { Parse = false }, null);
            cells[0, 1].GetDependents(true);
            cells[0, 1].GetPrecedents();
        }
```

### See Also

* class [FormulaParseOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


