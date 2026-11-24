---
title: "OoxmlSaveOptions.UpdateZoom"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "OoxmlSaveOptions‑Eigenschaft. Gibt an, ob der Skalierungsfaktor vor dem Speichern der Datei aktualisiert wird, wenn die Eigenschaften PageSetup.FitToPagesWide und PageSetup.FitToPagesTall steuern, wie das Arbeitsblatt skaliert wird"
type: docs
url: /de/net/aspose.cells/ooxmlsaveoptions/updatezoom/
---
## OoxmlSaveOptions.UpdateZoom property

Gibt an, ob der Skalierungsfaktor vor dem Speichern der Datei aktualisiert wird, wenn die Eigenschaften PageSetup.FitToPagesWide und PageSetup.FitToPagesTall steuern, wie das Arbeitsblatt skaliert wird.

```csharp
public bool UpdateZoom { get; set; }
```

### Hinweise

Der Standardwert ist aus Leistungsgründen false.

### Beispiele

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
            // Erstelle ein Beispielarbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Setze den anfänglichen Zoom‑Level
            worksheet.PageSetup.Zoom = 100;

            // Erstelle Speicheroptionen mit aktiviertem UpdateZoom
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions(SaveFormat.Xlsx);
            saveOptions.UpdateZoom = true;

            // In den Speicherstream speichern
            using (MemoryStream stream = new MemoryStream())
            {
                workbook.Save(stream, saveOptions);
                
                // Lade die Arbeitsmappe neu, um zu überprüfen, ob der Zoom aktualisiert wurde
                stream.Position = 0;
                Workbook reloadedWorkbook = new Workbook(stream);
                Console.WriteLine("Worksheet zoom level: " + reloadedWorkbook.Worksheets[0].PageSetup.Zoom);
            }
        }
    }
}
```

### Siehe auch

* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


