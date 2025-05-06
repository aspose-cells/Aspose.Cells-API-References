---
title: FormulaSettings.MaxIteration
second_title: Aspose.Cells for .NET API Reference
description: FormulaSettings property. The maximum iterations to resolve a circular reference
type: docs
url: /net/aspose.cells/formulasettings/maxiteration/
---
## FormulaSettings.MaxIteration property

The maximum iterations to resolve a circular reference.

```csharp
public int MaxIteration { get; set; }
```

### Examples

```csharp
// Called: settings.MaxIteration = 1;
[Test]
        public void Property_MaxIteration()
        {
            Workbook wb = new Workbook(Constants.sourcePath + &quot;Formula/calculate/CELLSNET-43641.xlsx&quot;);
            FormulaSettings settings = wb.Settings.FormulaSettings;
            settings.EnableCalculationChain = true;
            settings.EnableIterativeCalculation = true;
            settings.MaxIteration = 1;
            settings.MaxChange = 1;
            Worksheet worksheet = wb.Worksheets[&quot;Sheet1&quot;];
            Cell cell = worksheet.Cells[&quot;C2&quot;];
            int init = cell.IntValue;
            wb.CalculateFormula();
            int count = 1;
            while (cell.IntValue != init)
            {
                init = cell.IntValue;
                //Console.WriteLine(&quot;Current Value in C2 is : {0}, {1}&quot;, init, count);
                wb.CalculateFormula();
                count++;
                if (count &gt; 851)
                {
                    Assert.Fail(&quot;Calculation count for circular formula exceeds 851&quot;);
                }
            }
            Assert.AreEqual(851, count, &quot;Calculation count for circular formula&quot;);
        }
```

### See Also

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


