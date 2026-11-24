---
title: "WarningInfo.CorrectedObject"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WarningInfo-Eigenschaft. Ruft das korrigierte Objekt ab und legt es fest"
type: docs
url: /de/net/aspose.cells/warninginfo/correctedobject/
---
## WarningInfo.CorrectedObject property

Liest und setzt das korrigierte Objekt.

```csharp
public object CorrectedObject { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WarningInfoPropertyCorrectedObjectDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe und lösen Sie eine Warnung aus
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Setzen Sie einen Namen, der normalerweise eine Warnung auslösen würde
            string originalName = "MyRange";
            worksheet.Cells.CreateRange(originalName);
            
            // Warnungs-Callback verarbeiten
            workbook.Settings.WarningCallback = new WarningHandler();
            
            // Dieser Vorgang würde den Warnungs-Callback auslösen
            worksheet.Cells.CreateRange(originalName); // Duplicate range name
        }
    }

    public class WarningHandler : IWarningCallback
    {
        public void Warning(WarningInfo warningInfo)
        {
            if (warningInfo.WarningType == WarningType.DuplicateDefinedName)
            {
                // Demonstrieren Sie die Verwendung von CorrectedObject
                warningInfo.CorrectedObject = "_" + warningInfo.ErrorObject;
                Console.WriteLine($"Warning handled. Original: {warningInfo.ErrorObject}, Corrected: {warningInfo.CorrectedObject}");
            }
        }
    }
}
```

### Siehe auch

* class [WarningInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


