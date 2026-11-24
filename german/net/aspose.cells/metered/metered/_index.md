---
title: "Metered.Metered"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Metered‑Konstruktor. Initialisiert eine neue Instanz dieser Klasse"
type: docs
url: /de/net/aspose.cells/metered/metered/
---
## Metered constructor

Initialisiert eine neue Instanz dieser Klasse.

```csharp
public Metered()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MeteredMethodCtorDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Instanz mit dem Konstruktor
            Metered metered = new Metered();

            // Metered‑Lizenz festlegen
            metered.SetMeteredKey("YourPublicKey", "YourPrivateKey");

            // Erstellen Sie eine einfache Arbeitsmappe, um die Funktionalität zu demonstrieren
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Metered License Demo");
            
            // Speichere die Arbeitsmappe
            workbook.Save("MeteredDemoOutput.xlsx");
            
            Console.WriteLine("Demo completed successfully.");
        }
    }
}
```

### Siehe auch

* class [Metered](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


