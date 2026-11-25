---
title: "WarningInfo.Description"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WarningInfo. Ottieni la descrizione delle informazioni di avviso"
type: docs
url: /it/net/aspose.cells/warninginfo/description/
---
## WarningInfo.Description property

Ottieni la descrizione delle informazioni di avviso.

```csharp
public string Description { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WarningInfoPropertyDescriptionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea un nome definito duplicato per generare un avviso
            worksheet.Cells.CreateRange(0, 0, 10, 10).Name = "_XLNM.PRINT_AREA";
            worksheet.Cells.CreateRange(0, 0, 10, 10).Name = "_XLNM.PRINT_AREA"; // Different name to actually trigger warning

            // Ottieni il callback di avviso
            WarningCallback callback = new WarningCallback();
            workbook.Settings.WarningCallback = callback; // Correct property path

            // Salva per generare un avviso
            workbook.Save("output.xlsx");

            // Dimostra l'uso della proprietà Description
            if (callback.LastWarning != null)
            {
                Console.WriteLine("Warning Description: " + callback.LastWarning.Description);
                Console.WriteLine("Warning Type: " + callback.LastWarning.Type);
            }
        }
    }

    public class WarningCallback : IWarningCallback
    {
        public WarningInfo LastWarning { get; private set; }

        public void Warning(WarningInfo warningInfo)
        {
            LastWarning = warningInfo;
        }
    }
}
```

### Vedi anche

* class [WarningInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


