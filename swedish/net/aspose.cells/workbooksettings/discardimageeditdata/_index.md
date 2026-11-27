---
title: "WorkbookSettings.DiscardImageEditData"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookSettings property. Anger om redigeringsdata för bilder ska kasseras"
type: docs
url: /sv/net/aspose.cells/workbooksettings/discardimageeditdata/
---
## WorkbookSettings.DiscardImageEditData property

Anger om redigeringsbilddata ska kastas.

```csharp
public bool DiscardImageEditData { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyDiscardImageEditDataDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till en bild i kalkylbladet
            int index = worksheet.Pictures.Add(0, 0, "example.jpg");
            Picture picture = worksheet.Pictures[index];
            
            // Sätt DiscardImageEditData till true (standard är false)
            workbook.Settings.DiscardImageEditData = true;
            
            // Spara arbetsboken
            workbook.Save("output_with_discarded_image_data.xlsx", SaveFormat.Xlsx);
            
            // Verifiera att inställningen har tillämpats
            Console.WriteLine("DiscardImageEditData is set to: " + workbook.Settings.DiscardImageEditData);
        }
    }
}
```

### Se även

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


