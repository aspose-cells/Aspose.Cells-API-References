---
title: "HtmlSaveOptions.ExportObjectListener"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlSaveOptions‑egenskap. Hämtar eller anger ExportObjectListener för att exportera objekt"
type: docs
url: /sv/net/aspose.cells/htmlsaveoptions/exportobjectlistener/
---
## HtmlSaveOptions.ExportObjectListener property

Hämtar eller anger ExportObjectListener för att exportera objekt.

```csharp
[Obsolete("Use HtmlSaveOptions.IStreamProvider property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public IExportObjectListener ExportObjectListener { get; set; }
```

### Anmärkningar

OBS: Denna egenskap är nu föråldrad. Använd i stället HtmlSaveOptions.IStreamProvider‑egenskapen. Denna egenskap kommer att tas bort 12 månader senare, sedan augusti 2015. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportObjectListenerDemo
    {
        public static void Run()
        {
            // Skapa en anpassad export‑objekt‑lyssnare
            var listener = new CustomExportObjectListener();
            
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Export Object Listener");
            
            // Skapa HTML‑sparalternativ med lyssnaren
            HtmlSaveOptions saveOptions = new HtmlSaveOptions
            {
                ExportObjectListener = listener
            };

            // Spara till HTML‑fil
            workbook.Save("output.html", saveOptions);
        }
    }

    // Anpassad implementation av IExportObjectListener
    public class CustomExportObjectListener : IExportObjectListener
    {
        public object ExportObject(ExportObjectEvent e)
        {
            // Exempel: Bearbeta det exporterade objektet
            Console.WriteLine($"Exporting object: {e.GetType()}");
            // Returnera det ursprungliga objektet (kan modifieras om så behövs)
            return e;
        }
    }
}
```

### Se även

* interface [IExportObjectListener](../../iexportobjectlistener/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


