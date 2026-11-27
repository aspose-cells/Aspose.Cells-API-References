---
title: "Klass AbstractLowCodeLoadOptionsProvider"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.LowCode.AbstractLowCodeLoadOptionsProvider klass. Implementering för att tillhandahålla flera inläsningsalternativ för processer som använder flera indata såsom mallfiler"
type: docs
url: /sv/net/aspose.cells.lowcode/abstractlowcodeloadoptionsprovider/
---
## AbstractLowCodeLoadOptionsProvider class

Implementering för att tillhandahålla flera inläsningsalternativ för processer som använder flera indata (t.ex. mallfiler).

```csharp
public abstract class AbstractLowCodeLoadOptionsProvider
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| abstract [Current](../../aspose.cells.lowcode/abstractlowcodeloadoptionsprovider/current/) { get; } | Hämtar inläsningsalternativen från vilka data för den för närvarande bearbetade delen ska läsas in. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| virtual [Finish](../../aspose.cells.lowcode/abstractlowcodeloadoptionsprovider/finish/)(LowCodeLoadOptions) | Frigör resurser efter att ha bearbetat den aktuella delen av indata. |
| abstract [MoveNext](../../aspose.cells.lowcode/abstractlowcodeloadoptionsprovider/movenext/)() | Kontrollerar om det finns mer indata. |

### Anmärkningar

Till exempel kräver funktionen [`SpreadsheetMerger`](../spreadsheetmerger/) flera mallfiler för att slå ihop.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeClassAbstractLowCodeLoadOptionsProviderDemo
    {
        public static void Run()
        {
            // Skapa en anpassad implementering av AbstractLowCodeLoadOptionsProvider
            var provider = new CustomLoadOptionsProvider();

            // Bearbeta flera indata med hjälp av leverantören
            while (provider.MoveNext())
            {
                // Hämta aktuella inläsningsalternativ
                LowCodeLoadOptions currentOptions = provider.Current;
                Console.WriteLine($"Processing with load options: {currentOptions}");

                // Skapa arbetsbok med aktuella alternativ
                Workbook workbook = new Workbook(FileFormatType.Xlsx);
                Worksheet worksheet = workbook.Worksheets[0];

                // Demonstrera användning med arbetsbok
                worksheet.Cells["A1"].PutValue("Processed with custom provider");
                
                // Avsluta bearbetning av denna del
                provider.Finish(currentOptions);
            }
        }

        private class CustomLoadOptionsProvider : AbstractLowCodeLoadOptionsProvider
        {
            private int currentIndex = 0;
            private readonly LowCodeLoadOptions[] optionsList = new LowCodeLoadOptions[]
            {
                new LowCodeLoadOptions(),
                new LowCodeLoadOptions { InputFile = "protected.xlsx" }, // Password would be handled separately
                new LowCodeLoadOptions() // MemorySetting would be handled separately
            };

            public override LowCodeLoadOptions Current => optionsList[currentIndex];

            public override bool MoveNext()
            {
                if (currentIndex < optionsList.Length - 1)
                {
                    currentIndex++;
                    return true;
                }
                return false;
            }

            public override void Finish(LowCodeLoadOptions part)
            {
                // Rensnings- eller avslutningslogik för varje del
                Console.WriteLine($"Finished processing part {currentIndex}");
            }
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


