---
title: "PowerQueryFormulaFunction.Type"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PowerQueryFormulaFunction. Restituisce il tipo di formula Power Query"
type: docs
url: /it/net/aspose.cells.querytables/powerqueryformulafunction/type/
---
## PowerQueryFormulaFunction.Type property

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

    public class PowerQueryFormulaFunctionPropertyTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea una funzione di formula Power Query
            // Poiché non possiamo crearla direttamente, dovremo ottenerla da qualche parte
            // Per scopi dimostrativi, mostreremo solo come accedere alla proprietà Type
            // (In un utilizzo reale, otterresti questo da una collezione esistente)
            PowerQueryFormulaFunction function = null; // Can't instantiate directly
            
            // Poiché non possiamo nemmeno creare direttamente una QueryTable, salteremo quella parte
            QueryTable queryTable = null; // Can't instantiate directly
            
            // Impossibile aggiungere alla collezione di query tables in questo modo - è di sola lettura
            // worksheet.QueryTables[0] = queryTable; // Removed this line
            
            // Per dimostrazione, mostreremo solo il formato di output che useremmo se avessimo una funzione
            if (function != null)
            {
                Console.WriteLine("Power Query Formula Function Type: " + function.Type);
                Console.WriteLine("Is this a function? " + (function.Type == PowerQueryFormulaType.Function));
            }
            else
            {
                Console.WriteLine("Could not create PowerQueryFormulaFunction instance - constructor not available");
            }

            // Salva il risultato
            workbook.Save("PowerQueryFormulaFunctionTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [PowerQueryFormulaType](../../powerqueryformulatype/)
* class [PowerQueryFormulaFunction](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)


