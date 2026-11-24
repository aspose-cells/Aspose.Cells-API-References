---
title: "Metered.IsMeteredLicensed"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Metered‑Methode. Prüft, ob Metered lizenziert ist"
type: docs
url: /de/net/aspose.cells/metered/ismeteredlicensed/
---
## Metered.IsMeteredLicensed method

Prüfen, ob metered lizenziert ist

```csharp
public static bool IsMeteredLicensed()
```

### Rückgabewert

Wahr oder falsch

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MeteredMethodIsMeteredLicensedDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstellen Sie eine Metered‑Instanz
            Metered metered = new Metered();

            try
            {
                // Prüfen, ob die nutzungsbasierte Lizenz angewendet wurde
                bool isLicensed = Metered.IsMeteredLicensed();

                // Ergebnis anzeigen
                Console.WriteLine($"Is Metered Licensed: {isLicensed}");

                // Füge das Ergebnis dem Arbeitsblatt hinzu
                worksheet.Cells["A1"].PutValue("Is Metered Licensed:");
                worksheet.Cells["B1"].PutValue(isLicensed);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing IsMeteredLicensed method: {ex.Message}");
            }

            // Ergebnis speichern
            workbook.Save("MethodIsMeteredLicensedDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Metered](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


