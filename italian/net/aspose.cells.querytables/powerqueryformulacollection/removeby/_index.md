---
title: "PowerQueryFormulaCollection.RemoveBy"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PowerQueryFormulaCollection. Rimuovi la formula Power Query per nome"
type: docs
url: /it/net/aspose.cells.querytables/powerqueryformulacollection/removeby/
---
## PowerQueryFormulaCollection.RemoveBy method

Rimuove la formula Power Query per nome.

```csharp
public void RemoveBy(string name)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | String | Il nome della formula Power Query. |

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            try
            {
                // Accedi a PowerQueryFormulaCollection (supponendo che esista nella cartella di lavoro)
                PowerQueryFormulaCollection powerQueryFormulas = workbook.DataMashup.PowerQueryFormulas;
                
                // Aggiungi una formula di esempio da rimuovere (di solito proviene da dati esistenti)
                string formulaName = "SampleFormula";
                
                // Chiama RemoveBy con il nome della formula
                powerQueryFormulas.RemoveBy(formulaName);
                
                Console.WriteLine($"Formula '{formulaName}' removed successfully");
                
                // Salva la cartella di lavoro
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

### Vedi anche

* class [PowerQueryFormulaCollection](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


