---
title: "PaginatedSaveOptions.EmfRenderSetting"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PaginatedSaveOptions-Eigenschaft. Einstellung für das Rendern von EMF-Metadateien"
type: docs
url: /de/net/aspose.cells/paginatedsaveoptions/emfrendersetting/
---
## PaginatedSaveOptions.EmfRenderSetting property

Einstellung für die Darstellung von EMF‑Metadateien.

```csharp
public EmfRenderSetting EmfRenderSetting { get; set; }
```

### Hinweise

EMF-Metadateien, die als "EMF+ Dual" identifiziert werden, können sowohl EMF+-Datensätze als auch EMF-Datensätze enthalten. Jeder Datentyp kann zum Rendern des Bildes verwendet werden, nur EMF+-Datensätze oder nur EMF-Datensätze. Wenn EmfPlusPrefer gesetzt ist, werden EMF+-Datensätze beim Rendern der Seite geparst, andernfalls werden nur EMF-Datensätze geparst. Der Standardwert ist EmfOnly.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyEmfRenderSettingDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("EMF Render Setting Demo");
            worksheet.Cells["A2"].PutValue(DateTime.Now.ToString());

            // Erstelle ein Bild für die EMF-Demonstration
            worksheet.Pictures.Add(10, 10, "example.png");

            // Konfiguriere Speicheroptionen mit EMF-Einstellungen mittels PdfSaveOptions
            PdfSaveOptions options = new PdfSaveOptions()
            {
                EmfRenderSetting = EmfRenderSetting.EmfPlusPrefer
            };

            // Speichere die Arbeitsmappe mit EMF-Einstellungen
            workbook.Save("EmfRenderSettingDemo.pdf", options);
        }
    }
}
```

### Siehe auch

* enum [EmfRenderSetting](../../emfrendersetting/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


