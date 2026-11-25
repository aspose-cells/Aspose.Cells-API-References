---
title: "HtmlSaveOptions.ExportObjectListener"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà HtmlSaveOptions. Ottiene o imposta l'ExportObjectListener per l'esportazione di oggetti"
type: docs
url: /it/net/aspose.cells/htmlsaveoptions/exportobjectlistener/
---
## HtmlSaveOptions.ExportObjectListener property

Ottiene o imposta l'ExportObjectListener per l'esportazione di oggetti.

```csharp
[Obsolete("Use HtmlSaveOptions.IStreamProvider property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public IExportObjectListener ExportObjectListener { get; set; }
```

### Osservazioni

NOTA: Questa proprietà è ora obsoleta. Invece, utilizza la proprietà HtmlSaveOptions.IStreamProvider. Questa proprietà sarà rimossa 12 mesi dopo, a partire da agosto 2015. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

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
            // Crea un listener di esportazione oggetti personalizzato
            var listener = new CustomExportObjectListener();
            
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Export Object Listener");
            
            // Crea le opzioni di salvataggio HTML con il listener
            HtmlSaveOptions saveOptions = new HtmlSaveOptions
            {
                ExportObjectListener = listener
            };

            // Salva in un file HTML
            workbook.Save("output.html", saveOptions);
        }
    }

    // Implementazione personalizzata di IExportObjectListener
    public class CustomExportObjectListener : IExportObjectListener
    {
        public object ExportObject(ExportObjectEvent e)
        {
            // Esempio: Elabora l'oggetto esportato
            Console.WriteLine($"Exporting object: {e.GetType()}");
            // Restituisci l'oggetto originale (può essere modificato se necessario)
            return e;
        }
    }
}
```

### Vedi anche

* interface [IExportObjectListener](../../iexportobjectlistener/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


