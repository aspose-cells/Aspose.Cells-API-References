---
title: "Enum EmfRenderSetting"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.EmfRenderSetting-enum. Inställning för rendering av Emf-metafil"
type: docs
url: /sv/net/aspose.cells/emfrendersetting/
---
## EmfRenderSetting enumeration

Inställning för rendering av EMF-metafil.

```csharp
public enum EmfRenderSetting
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| EmfOnly | `0` | Endast renderar Emf-poster. |
| EmfPlusPrefer | `1` | Föredrar rendera EmfPlus-poster. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class CellsClassEmfRenderSettingDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("EMF Render Setting Demo");
            worksheet.Cells["A2"].PutValue("Using EmfOnly setting");

            // Skapa bildalternativ med EMF-renderingsinställning
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                EmfRenderSetting = EmfRenderSetting.EmfOnly
            };

            // Skapa en bladrendering med alternativen
            SheetRender render = new SheetRender(worksheet, options);

            // Spara den första sidan som EMF-bild
            render.ToImage(0, "EmfRenderSettingDemo.emf");

            Console.WriteLine("EMF file created successfully with EmfOnly setting.");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


