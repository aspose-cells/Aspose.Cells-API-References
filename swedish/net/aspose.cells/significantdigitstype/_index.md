---
title: "Enum SignificantDigitsType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.SignificantDigitsType enum. Representerar typen av signifikanta siffror för utskrift av numeriska värden"
type: docs
url: /sv/net/aspose.cells/significantdigitstype/
---
## SignificantDigitsType enumeration

Representerar typen av signifikanta siffror för utskrift av numeriska värden.

```csharp
public enum SignificantDigitsType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Digits15 | `0` | 15 siffror |
| G17 | `1` | 17 siffror genom att formatera värdet med \"G17\". |
| Rounding17 | `2` | 17 siffror genom att avrunda värdet. |

### Exempel

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
                // Skapa en ny arbetsbok för demonstration
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Demonstrera användning av varje SignificantDigitsType enum‑värde
                SignificantDigitsType[] types = {
                    SignificantDigitsType.Digits15,
                    SignificantDigitsType.G17,
                    SignificantDigitsType.Rounding17
                };

                foreach (SignificantDigitsType type in types)
                {
                    // Ställ in typen av signifikanta siffror för arbetsboken
                    workbook.Settings.SignificantDigitsType = type;

                    // Visa den aktuella inställningen
                    Console.WriteLine($"Current SignificantDigitsType: {type} (Value: {(int)type})");

                    // Lägg till ett exempelvärde för att demonstrera inställningen
                    worksheet.Cells["A1"].PutValue(123.4567890123456789);

                    // Spara arbetsboken med den aktuella inställningen
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

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


