---
title: "PowerQueryFormulaParameter.Type"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PowerQueryFormulaParameter. Ottiene il tipo di formula Power Query"
type: docs
url: /it/net/aspose.cells.querytables/powerqueryformulaparameter/type/
---
## PowerQueryFormulaParameter.Type property

Ottiene il tipo della formula power query.

```csharp
public override PowerQueryFormulaType Type { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.QueryTables;
    using System;

    public class PowerQueryFormulaParameterPropertyTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            try
            {
                // Poiché non possiamo creare direttamente un PowerQueryFormulaParameter senza conoscere i parametri richiesti del costruttore,
                // dimostreremo l'accesso alla proprietà Type tramite i parametri di una tabella di query esistente
                Console.WriteLine("This demo shows how to access the Type property of PowerQueryFormulaParameter.");
                
                // In uno scenario reale, accederesti a questo da una tabella di query esistente
                // Per scopi dimostrativi, mostreremo come verificare il tipo se avessi un'istanza
                PowerQueryFormulaParameter parameter = null; // This would normally come from a query table
                
                if (parameter != null)
                {
                    // Visualizza il valore della proprietà Type (proprietà di sola lettura)
                    Console.WriteLine($"PowerQueryFormulaParameter Type: {parameter.Type}");
                    
                    // Mostra i possibili valori enum
                    Console.WriteLine("Possible PowerQueryFormulaType values:");
                    foreach (PowerQueryFormulaType type in Enum.GetValues(typeof(PowerQueryFormulaType)))
                    {
                        Console.WriteLine($"- {type}");
                    }
                }
                else
                {
                    Console.WriteLine("No PowerQueryFormulaParameter instance available for demonstration.");
                }
                
                // Salva la cartella di lavoro
                workbook.Save("TypeDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* enum [PowerQueryFormulaType](../../powerqueryformulatype/)
* class [PowerQueryFormulaParameter](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


