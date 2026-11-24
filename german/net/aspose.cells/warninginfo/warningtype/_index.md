---
title: "WarningInfo.WarningType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WarningInfo-Eigenschaft. Warnungstyp abrufen"
type: docs
url: /de/net/aspose.cells/warninginfo/warningtype/
---
## WarningInfo.WarningType property

Warnungstyp abrufen.

```csharp
[Obsolete("Use WarningInfo.Type property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public WarningType WarningType { get; }
```

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Bitte verwenden Sie stattdessen die WarningInfo.Type‑Eigenschaft. Diese Eigenschaft wird 12 Monate später, seit Dezember 2024, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erfahren haben.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WarningInfoPropertyWarningTypeDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe und lösen Sie eine Warnung aus
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Dies löst eine Warnung aus, wenn Sie mit nicht unterstützten Funktionen speichern
            workbook.Settings.WarningCallback = new WarningCallback();
            
            // Speichern Sie mit einem Format, das Warnungen verursachen könnte
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }

    internal class WarningCallback : IWarningCallback
    {
        public void Warning(WarningInfo warningInfo)
        {
            // Demonstrieren Sie die Verwendung der WarningType‑Eigenschaft
            Console.WriteLine("Warning: " + warningInfo.WarningType + " - " + warningInfo.Description);
            
            // Verarbeiten Sie spezifische Warnungsarten
            if (warningInfo.WarningType == WarningType.UnsupportedFileFormat)
            {
                Console.WriteLine("Unsupported format warning detected!");
            }
        }
    }
}
```

### Siehe auch

* enum [WarningType](../../warningtype/)
* class [WarningInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


