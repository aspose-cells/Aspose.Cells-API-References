---
title: "Metered.Metered"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Costruttore Metered. Inizializza una nuova istanza di questa classe"
type: docs
url: /it/net/aspose.cells/metered/metered/
---
## Metered constructor

Inizializza una nuova istanza di questa classe.

```csharp
public Metered()
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MeteredMethodCtorDemo
    {
        public static void Run()
        {
            // Crea un'istanza usando il costruttore
            Metered metered = new Metered();

            // Imposta la licenza metered
            metered.SetMeteredKey("YourPublicKey", "YourPrivateKey");

            // Crea una cartella di lavoro semplice per dimostrare la funzionalità
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Metered License Demo");
            
            // Salva la cartella di lavoro
            workbook.Save("MeteredDemoOutput.xlsx");
            
            Console.WriteLine("Demo completed successfully.");
        }
    }
}
```

### Vedi anche

* class [Metered](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


