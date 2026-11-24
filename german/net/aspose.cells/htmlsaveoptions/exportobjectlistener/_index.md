---
title: "HtmlSaveOptions.ExportObjectListener"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HtmlSaveOptions-Eigenschaft. Ruft den ExportObjectListener ab oder legt ihn fest für das Exportieren von Objekten."
type: docs
url: /de/net/aspose.cells/htmlsaveoptions/exportobjectlistener/
---
## HtmlSaveOptions.ExportObjectListener property

Ruft den ExportObjectListener ab oder legt ihn fest für das Exportieren von Objekten.

```csharp
[Obsolete("Use HtmlSaveOptions.IStreamProvider property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public IExportObjectListener ExportObjectListener { get; set; }
```

### Hinweise

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die HtmlSaveOptions.IStreamProvider-Eigenschaft. Diese Eigenschaft wird 12 Monate später, seit August 2015, entfernt werden. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erlebt haben.

### Beispiele

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
            // Erstellen Sie einen benutzerdefinierten ExportObjectListener
            var listener = new CustomExportObjectListener();
            
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Export Object Listener");
            
            // Erstellen Sie HTML-Speicheroptionen mit dem Listener
            HtmlSaveOptions saveOptions = new HtmlSaveOptions
            {
                ExportObjectListener = listener
            };

            // In HTML-Datei speichern
            workbook.Save("output.html", saveOptions);
        }
    }

    // Benutzerdefinierte Implementierung von IExportObjectListener
    public class CustomExportObjectListener : IExportObjectListener
    {
        public object ExportObject(ExportObjectEvent e)
        {
            // Beispiel: Verarbeiten Sie das exportierte Objekt
            Console.WriteLine($"Exporting object: {e.GetType()}");
            // Geben Sie das ursprüngliche Objekt zurück (kann bei Bedarf modifiziert werden)
            return e;
        }
    }
}
```

### Siehe auch

* interface [IExportObjectListener](../../iexportobjectlistener/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


