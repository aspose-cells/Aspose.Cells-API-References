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
// Called: Console.WriteLine(powerQueryFormula.FormulaDefinition);
public void PowerQueryFormula_Property_FormulaDefinition()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    Aspose.Cells.QueryTables.DataMashup mashupData = workbook.DataMashup;
    foreach (PowerQueryFormula powerQueryFormula in mashupData.PowerQueryFormulas)
    {
        Console.WriteLine("__________________________________");
        Console.WriteLine(powerQueryFormula.FormulaDefinition);
        Assert.IsFalse(string.IsNullOrEmpty(powerQueryFormula.FormulaDefinition));
        var contents = powerQueryFormula.FormulaDefinition.Replace("\r\n", "\n");
    }
    workbook.Save(Constants.destPath + "example.xlsx");

}
```

### See Also

* class [PowerQueryFormula](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


