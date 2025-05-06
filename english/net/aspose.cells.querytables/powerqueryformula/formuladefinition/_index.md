---
title: PowerQueryFormula.FormulaDefinition
second_title: Aspose.Cells for .NET API Reference
description: PowerQueryFormula property. Gets the definition of the power query formula
type: docs
url: /net/aspose.cells.querytables/powerqueryformula/formuladefinition/
---
## PowerQueryFormula.FormulaDefinition property

Gets the definition of the power query formula.

```csharp
public virtual string FormulaDefinition { get; }
```

### Examples

```csharp
// Called: Assert.IsFalse(string.IsNullOrEmpty(powerQueryFormula.FormulaDefinition));
[Test]
        public void Property_FormulaDefinition()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet47552.xlsx&quot;);
            Aspose.Cells.QueryTables.DataMashup mashupData = workbook.DataMashup;
            foreach (PowerQueryFormula powerQueryFormula in mashupData.PowerQueryFormulas)
            {
                Console.WriteLine(&quot;__________________________________&quot;);
                Console.WriteLine(powerQueryFormula.FormulaDefinition);
                Assert.IsFalse(string.IsNullOrEmpty(powerQueryFormula.FormulaDefinition));
                var contents = powerQueryFormula.FormulaDefinition.Replace(&quot;\r\n&quot;, &quot;\n&quot;);
            }
            workbook.Save(Constants.destPath + &quot;CellsNet47552.xlsx&quot;);

        }
```

### See Also

* class [PowerQueryFormula](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


