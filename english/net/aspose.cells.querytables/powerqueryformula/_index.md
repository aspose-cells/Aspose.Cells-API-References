---
title: Class PowerQueryFormula
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.QueryTables.PowerQueryFormula class. Represents the definition of power query formula
type: docs
url: /net/aspose.cells.querytables/powerqueryformula/
---
## PowerQueryFormula class

Represents the definition of power query formula.

```csharp
public class PowerQueryFormula
```

## Properties

| Name | Description |
| --- | --- |
| [Description](../../aspose.cells.querytables/powerqueryformula/description/) { get; set; } | Gets and sets the description of the power query formula. |
| virtual [FormulaDefinition](../../aspose.cells.querytables/powerqueryformula/formuladefinition/) { get; } | Gets the definition of the power query formula. |
| [GroupName](../../aspose.cells.querytables/powerqueryformula/groupname/) { get; } | Gets the name of group which contains this power query formula. |
| [Name](../../aspose.cells.querytables/powerqueryformula/name/) { get; set; } | Gets and sets the name of the power query formula. |
| [PowerQueryFormulaItems](../../aspose.cells.querytables/powerqueryformula/powerqueryformulaitems/) { get; } | Gets all items of power query formula. |
| virtual [Type](../../aspose.cells.querytables/powerqueryformula/type/) { get; } | Gets the type of this power query formula. |

### Examples

```csharp
// Called: PowerQueryFormula firstFormula = powerQueryFormulas[0];
public static void QueryTables_Type_PowerQueryFormula()
        {
            // Create a new workbook
            Workbook workbook = new Workbook("PowerQueryFormulaDemo_original.xlsx");

            // Create a DataMashup object
            DataMashup dataMashup = workbook.DataMashup;

            // Access PowerQueryFormulas collection
            PowerQueryFormulaCollection powerQueryFormulas = dataMashup.PowerQueryFormulas;

            // Display the count of Power Query formulas
            Console.WriteLine($"Number of Power Query Formulas: {powerQueryFormulas.Count}");

            // Example of accessing a specific Power Query formula (if any exist)
            if (powerQueryFormulas.Count > 0)
            {
                PowerQueryFormula firstFormula = powerQueryFormulas[0];
                Console.WriteLine($"First Power Query Formula: {firstFormula}");
            }

            // Save the workbook
            workbook.Save("PowerQueryFormulaDemo.xlsx");
        }
```

### See Also

* namespace [Aspose.Cells.QueryTables](../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../)


