---
title: "PaginatedSaveOptions.EmfRenderSetting"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PaginatedSaveOptions‑egenskap. Inställning för rendering av Emf‑metafil"
type: docs
url: /sv/net/aspose.cells/paginatedsaveoptions/emfrendersetting/
---
## PaginatedSaveOptions.EmfRenderSetting property

Inställning för rendering av EMF-metafil.

```csharp
public EmfRenderSetting EmfRenderSetting { get; set; }
```

### Anmärkningar

EMF‑metafiler identifierade som "EMF+ Dual" kan innehålla både EMF+‑poster och EMF‑poster. Antingen kan någon av posterna användas för att rendera bilden, endast EMF+‑poster, eller endast EMF‑poster. När EmfPlusPrefer är satt, kommer EMF+‑poster att parsas vid rendering till sidan, annars parsas endast EMF‑poster. Standardvärdet är EmfOnly.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyEmfRenderSettingDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("EMF Render Setting Demo");
            worksheet.Cells["A2"].PutValue(DateTime.Now.ToString());

            // Skapa bild för EMF‑demonstration
            worksheet.Pictures.Add(10, 10, "example.png");

            // Konfigurera sparalternativ med EMF‑inställningar med PdfSaveOptions
            PdfSaveOptions options = new PdfSaveOptions()
            {
                EmfRenderSetting = EmfRenderSetting.EmfPlusPrefer
            };

            // Spara arbetsboken med EMF‑inställningar
            workbook.Save("EmfRenderSettingDemo.pdf", options);
        }
    }
}
```

### Se även

* enum [EmfRenderSetting](../../emfrendersetting/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


