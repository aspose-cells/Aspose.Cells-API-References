---
title: "FontConfigs.IsFontAvailable"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FontConfigs-Methode. Gibt an, ob die Schrift verfügbar ist"
type: docs
url: /de/net/aspose.cells/fontconfigs/isfontavailable/
---
## FontConfigs.IsFontAvailable method

Gibt an, ob die Schriftart verfügbar ist.

```csharp
public static bool IsFontAvailable(string fontName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fontName | String | Schriftname |

### Rückgabewert

true, wenn die Schrift verfügbar ist, andernfalls false.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontConfigsMethodIsFontAvailableWithStringDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Testen Sie Schriftartnamen, um die Verfügbarkeit zu prüfen
            string[] testFonts = { "Arial", "Times New Roman", "NonExistentFont" };

            try
            {
                foreach (string fontName in testFonts)
                {
                    // Rufen Sie die Methode IsFontAvailable mit dem Schriftartnamen auf
                    bool isAvailable = FontConfigs.IsFontAvailable(fontName);

                    // Ergebnis anzeigen
                    Console.WriteLine($"Font '{fontName}' is available: {isAvailable}");

                    // Schreiben Sie das Ergebnis in das Arbeitsblatt
                    int row = worksheet.Cells.MaxDataRow + 1;
                    worksheet.Cells[row, 0].PutValue($"Font '{fontName}' available:");
                    worksheet.Cells[row, 1].PutValue(isAvailable);
                }

                Console.WriteLine("Method executed successfully with parameters (String)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing IsFontAvailable method: {ex.Message}");
            }

            // Ergebnis speichern
            workbook.Save("FontConfigsMethodIsFontAvailableWithStringDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


