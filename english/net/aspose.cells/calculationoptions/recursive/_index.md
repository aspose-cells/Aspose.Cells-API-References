---
title: CalculationOptions.Recursive
second_title: Aspose.Cells for .NET API Reference
description: CalculationOptions property. Indicates whether calculate the dependent cells recursively when calculating one cell and it depends on other cells. The default value is true
type: docs
url: /net/aspose.cells/calculationoptions/recursive/
---
## CalculationOptions.Recursive property

Indicates whether calculate the dependent cells recursively when calculating one cell and it depends on other cells. The default value is true.

```csharp
public bool Recursive { get; set; }
```

### Examples

```csharp
// Called: opt.Recursive = false;
public void Property_Recursive()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            cells["A1"].PutValue("A");
            cells["A2"].PutValue("B");
            cells["A3"].PutValue("C");
            cells["C1"].Formula = "=INDEX(MyFunction(\"A1:A3\"), MATCH(\"B\",INDIRECT(\"A1:A3\"),0))";
            cells["C2"].Formula = "=INDEX(MyFunction(\"A1:A3\"), 2)";
            cells["C3"].Formula = "=MATCH(\"B\",MyFunction(\"A1:A3\"),0)";
            cells["C4"].Formula = "=INDEX(INDIRECT(\"A1:A3\"), MATCH(\"B\",INDIRECT(\"A1:A3\"),0))";
            cells["C5"].Formula = "=MATCH(\"B\",INDIRECT(\"A1:A3\"),0)";
            cells["C6"].Formula = "=INDEX(INDIRECT(\"A1:A3\"), MATCH(\"B\",MyFunction(\"A1:A3\"),0))";
            CalculationOptions opt = new CalculationOptions();
            opt.Recursive = false;
            opt.CustomEngine = new EngineJava44185(cells);
            wb.CalculateFormula(opt);
            for (int i = 0; i < 6; i++)
            {
                if (i == 2 || i == 4)
                {
                    Assert.AreEqual(2, cells[i, 2].IntValue);
                }
                else
                {
                    Assert.AreEqual("B", cells[i, 2].StringValue);
                }
            }
        }
```

### See Also

* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


