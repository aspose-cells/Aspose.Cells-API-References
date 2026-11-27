---
title: "OoxmlSaveOptions.UpdateZoom"
second_title: "Aspose.Cells för .NET API‑referens"
description: "OoxmlSaveOptions egenskap. Anger om skalningsfaktorn ska uppdateras innan filen sparas när egenskaperna PageSetup.FitToPagesWide och PageSetup.FitToPagesTall styr hur arbetsbladet skalas"
type: docs
url: /sv/net/aspose.cells/ooxmlsaveoptions/updatezoom/
---
## OoxmlSaveOptions.UpdateZoom property

Anger om skalningsfaktorn ska uppdateras innan filen sparas om egenskaperna PageSetup.FitToPagesWide och PageSetup.FitToPagesTall styr hur kalkylbladet skalas.

```csharp
public bool UpdateZoom { get; set; }
```

### Anmärkningar

Standardvärdet är falskt för prestanda.

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OoxmlSaveOptionsPropertyUpdateZoomDemo
    {
        public static void Run()
        {
            // Skapa en exempelarbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ställ in initial zoomnivå
            worksheet.PageSetup.Zoom = 100;

            // Skapa sparalternativ med UpdateZoom aktiverat
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions(SaveFormat.Xlsx);
            saveOptions.UpdateZoom = true;

            // Spara till minnesström
            using (MemoryStream stream = new MemoryStream())
            {
                workbook.Save(stream, saveOptions);
                
                // Läs in arbetsboken igen för att verifiera att zoom har uppdaterats
                stream.Position = 0;
                Workbook reloadedWorkbook = new Workbook(stream);
                Console.WriteLine("Worksheet zoom level: " + reloadedWorkbook.Worksheets[0].PageSetup.Zoom);
            }
        }
    }
}
```

### Se även

* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


