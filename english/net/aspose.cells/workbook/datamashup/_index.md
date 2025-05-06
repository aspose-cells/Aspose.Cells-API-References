---
title: Workbook.DataMashup
second_title: Aspose.Cells for .NET API Reference
description: Workbook property. Gets mashup data
type: docs
url: /net/aspose.cells/workbook/datamashup/
---
## Workbook.DataMashup property

Gets mashup data.

```csharp
public DataMashup DataMashup { get; }
```

### Examples

```csharp
// Called: DataMashup dataMashup = workbook.DataMashup;
public static void Property_DataMashup()
        {
            // Create a new workbook
            Workbook workbook = new Workbook(&quot;PowerQueryFormulaDemo_original.xlsx&quot;);

            // Create a DataMashup object
            DataMashup dataMashup = workbook.DataMashup;

            // Access PowerQueryFormulas collection
            PowerQueryFormulaCollection powerQueryFormulas = dataMashup.PowerQueryFormulas;

            // Display the count of Power Query formulas
            Console.WriteLine($&quot;Number of Power Query Formulas: {powerQueryFormulas.Count}&quot;);

            // Example of accessing a specific Power Query formula (if any exist)
            if (powerQueryFormulas.Count &gt; 0)
            {
                PowerQueryFormula firstFormula = powerQueryFormulas[0];
                Console.WriteLine($&quot;First Power Query Formula: {firstFormula}&quot;);
            }

            // Save the workbook
            workbook.Save(&quot;PowerQueryFormulaDemo.xlsx&quot;);
        }
```

### See Also

* class [DataMashup](../../../aspose.cells.querytables/datamashup/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


