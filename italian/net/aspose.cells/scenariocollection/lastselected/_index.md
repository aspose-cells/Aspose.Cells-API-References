---
title: "ScenarioCollection.LastSelected"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ScenarioCollection. Indica quale scenario è stato selezionato per ultimo dall'utente per essere eseguito/visualizzato"
type: docs
url: /it/net/aspose.cells/scenariocollection/lastselected/
---
## ScenarioCollection.LastSelected property

Indica quale scenario è stato selezionato per ultimo dall'utente per essere eseguito/visualizzato.

```csharp
public int LastSelected { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ScenarioCollectionPropertyLastSelectedDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi scenari
            ScenarioCollection scenarios = worksheet.Scenarios;
            scenarios.Add("Scenario1");
            scenarios.Add("Scenario2");

            // Imposta lo scenario attivo e l'indice dell'ultimo selezionato
            scenarios.ActiveIndex = 1;
            scenarios.LastSelected = 1;

            // Verifica e dimostra la proprietà LastSelected
            Console.WriteLine("Total scenarios: " + scenarios.Count);
            Console.WriteLine("Active scenario index: " + scenarios.ActiveIndex);
            Console.WriteLine("Last selected scenario index: " + scenarios.LastSelected);

            // Modifica l'indice dell'ultimo selezionato
            scenarios.LastSelected = 0;
            Console.WriteLine("Updated last selected scenario index: " + scenarios.LastSelected);
        }
    }
}
```

### Vedi anche

* class [ScenarioCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


