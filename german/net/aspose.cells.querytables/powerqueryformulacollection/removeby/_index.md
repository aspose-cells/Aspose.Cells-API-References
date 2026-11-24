---
title: "PowerQueryFormulaCollection.RemoveBy"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PowerQueryFormulaCollection‑Methode. Entfernt Power‑Query‑Formel nach Namen"
type: docs
url: /de/net/aspose.cells.querytables/powerqueryformulacollection/removeby/
---
## PowerQueryFormulaCollection.RemoveBy method

Entfernt Power Query-Formel nach Namen.

```csharp
public void RemoveBy(string name)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | String | Der Name der Power‑Query‑Formel. |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            try
            {
                // Greifen Sie auf die PowerQueryFormulaCollection zu (vorausgesetzt, sie existiert in der Arbeitsmappe)
                PowerQueryFormulaCollection powerQueryFormulas = workbook.DataMashup.PowerQueryFormulas;
                
                // Fügen Sie eine Beispiel‑Formel zum Entfernen hinzu (dies würde normalerweise aus vorhandenen Daten stammen)
                string formulaName = "SampleFormula";
                
                // Rufen Sie RemoveBy mit dem Formelnamen auf
                powerQueryFormulas.RemoveBy(formulaName);
                
                Console.WriteLine($"Formula '{formulaName}' removed successfully");
                
                // Speichere die Arbeitsmappe
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

### Siehe auch

* class [PowerQueryFormulaCollection](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


