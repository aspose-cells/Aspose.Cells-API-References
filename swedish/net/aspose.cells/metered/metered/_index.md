---
title: "Metered.Metered"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Metered-konstruktor. Initierar en ny instans av denna klass"
type: docs
url: /sv/net/aspose.cells/metered/metered/
---
## Metered constructor

Initierar en ny instans av denna klass.

```csharp
public Metered()
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MeteredMethodCtorDemo
    {
        public static void Run()
        {
            // Skapa en instans med hjälp av konstruktorn
            Metered metered = new Metered();

            // Ställ in Metered-licens
            metered.SetMeteredKey("YourPublicKey", "YourPrivateKey");

            // Skapa en enkel arbetsbok för att demonstrera funktionaliteten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Metered License Demo");
            
            // Spara arbetsboken
            workbook.Save("MeteredDemoOutput.xlsx");
            
            Console.WriteLine("Demo completed successfully.");
        }
    }
}
```

### Se även

* class [Metered](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


