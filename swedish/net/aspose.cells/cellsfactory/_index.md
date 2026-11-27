---
title: "Klass CellsFactory"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.CellsFactory‑klass. Verktyg för att instansiera klasser i Cells‑modellen"
type: docs
url: /sv/net/aspose.cells/cellsfactory/
---
## CellsFactory class

Verktyg för att instansiera klasser i Cells-modellen.

```csharp
public class CellsFactory
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [CellsFactory](cellsfactory/)() | Standardkonstruktorn. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [CreateStyle](../../aspose.cells/cellsfactory/createstyle/)() | Skapar en ny stil. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsFactoryDemo
    {
        public static void CellsFactoryExample()
        {
            // Skapa en ny instans av CellsFactory
            CellsFactory factory = new CellsFactory();

            // Använd fabriken för att skapa en ny Stil
            Style style = factory.CreateStyle();

            // Anpassa stilen
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.LightBlue;
            style.Pattern = BackgroundType.Solid;

            // Skapa en ny arbetsbok och ett kalkylblad
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Applicera stilen på en specifik cell
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Styled Cell");
            cell.SetStyle(style);

            // Spara arbetsboken till en fil
            workbook.Save("CellsFactoryExample.xlsx");
            workbook.Save("CellsFactoryExample.pdf");
            return;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


