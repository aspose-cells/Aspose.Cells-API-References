---
title: "Enum SignificantDigitsType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.SignificantDigitsType enum. Stellt den Typ signifikanter Stellen für die Ausgabe numerischer Werte dar"
type: docs
url: /de/net/aspose.cells/significantdigitstype/
---
## SignificantDigitsType enumeration

Stellt den Typ der signifikanten Stellen für die Ausgabe numerischer Werte dar.

```csharp
public enum SignificantDigitsType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Digits15 | `0` | 15 Stellen |
| G17 | `1` | 17 Stellen durch Formatieren des Wertes mit "G17". |
| Rounding17 | `2` | 17 Stellen durch Runden des Wertes. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassSignificantDigitsTypeDemo
    {
        public static void Run()
        {
            try
            {
                // Erstellt ein neues Arbeitsbuch für die Demonstration
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Demonstrieren Sie die Verwendung jedes SignificantDigitsType-Enum-Werts
                SignificantDigitsType[] types = {
                    SignificantDigitsType.Digits15,
                    SignificantDigitsType.G17,
                    SignificantDigitsType.Rounding17
                };

                foreach (SignificantDigitsType type in types)
                {
                    // Setzen Sie den Typ signifikanter Stellen für die Arbeitsmappe
                    workbook.Settings.SignificantDigitsType = type;

                    // Anzeige der aktuellen Einstellung
                    Console.WriteLine($"Current SignificantDigitsType: {type} (Value: {(int)type})");

                    // Fügen Sie einen Beispielwert hinzu, um die Einstellung zu demonstrieren
                    worksheet.Cells["A1"].PutValue(123.4567890123456789);

                    // Speichern Sie die Arbeitsmappe mit der aktuellen Einstellung
                    string fileName = $"SignificantDigitsType_{type}.xlsx";
                    workbook.Save(fileName);
                    Console.WriteLine($"Workbook saved with {type} setting as {fileName}");
                }

                Console.WriteLine("All SignificantDigitsType demonstrations completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error demonstrating SignificantDigitsType: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


