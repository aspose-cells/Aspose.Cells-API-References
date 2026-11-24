---
title: "Aufzählung EmfRenderSetting"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.EmfRenderSetting Aufzählung. Einstellung für das Rendern von Emf-Metadatei"
type: docs
url: /de/net/aspose.cells/emfrendersetting/
---
## EmfRenderSetting enumeration

Einstellung für die Darstellung von EMF‑Metadateien.

```csharp
public enum EmfRenderSetting
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| EmfOnly | `0` | Nur Emf-Datensätze rendern. |
| EmfPlusPrefer | `1` | Bevorzugt das Rendern von EmfPlus-Datensätzen. |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("EMF Render Setting Demo");
            worksheet.Cells["A2"].PutValue("Using EmfOnly setting");

            // Erstelle Bildoptionen mit EMF-Render-Einstellung
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                EmfRenderSetting = EmfRenderSetting.EmfOnly
            };

            // Erstelle ein Blatt-Rendering mit den Optionen
            SheetRender render = new SheetRender(worksheet, options);

            // Speichere die erste Seite als EMF-Bild
            render.ToImage(0, "EmfRenderSettingDemo.emf");

            Console.WriteLine("EMF file created successfully with EmfOnly setting.");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


