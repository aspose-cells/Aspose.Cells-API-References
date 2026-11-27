---
title: "PowerQueryFormulaCollection.RemoveBy"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PowerQueryFormulaCollection-metod. Ta bort power query-formel efter namn"
type: docs
url: /sv/net/aspose.cells.querytables/powerqueryformulacollection/removeby/
---
## PowerQueryFormulaCollection.RemoveBy method

Ta bort Power Query‑formel efter namn.

```csharp
public void RemoveBy(string name)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| namn | String | Namnet på power query-formeln. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.QueryTables;
    using System;

    public class PowerQueryFormulaCollectionMethodRemoveByWithStringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            try
            {
                // Åtkomst till PowerQueryFormulaCollection (förutsatt att den finns i arbetsboken)
                PowerQueryFormulaCollection powerQueryFormulas = workbook.DataMashup.PowerQueryFormulas;
                
                // Lägg till en exempelformel som ska tas bort (denna skulle normalt komma från befintliga data)
                string formulaName = "SampleFormula";
                
                // Anropa RemoveBy med formelnamnet
                powerQueryFormulas.RemoveBy(formulaName);
                
                Console.WriteLine($"Formula '{formulaName}' removed successfully");
                
                // Spara arbetsboken
                workbook.Save("RemoveByWithStringDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in RemoveBy demonstration: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [PowerQueryFormulaCollection](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


