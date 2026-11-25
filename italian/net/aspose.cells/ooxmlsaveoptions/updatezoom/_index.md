---
title: "OoxmlSaveOptions.UpdateZoom"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà OoxmlSaveOptions. Indica se aggiornare il fattore di scala prima di salvare il file quando le proprietà PageSetup.FitToPagesWide e PageSetup.FitToPagesTall controllano come il foglio di lavoro viene scalato"
type: docs
url: /it/net/aspose.cells/ooxmlsaveoptions/updatezoom/
---
## OoxmlSaveOptions.UpdateZoom property

Indica se aggiornare il fattore di scala prima di salvare il file se le proprietà PageSetup.FitToPagesWide e PageSetup.FitToPagesTall controllano come il foglio di lavoro viene scalato.

```csharp
public bool UpdateZoom { get; set; }
```

### Osservazioni

Il valore predefinito è false per motivi di prestazioni.

### Esempi

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
            // Crea una cartella di lavoro di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta il livello di zoom iniziale
            worksheet.PageSetup.Zoom = 100;

            // Crea le opzioni di salvataggio con UpdateZoom abilitato
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions(SaveFormat.Xlsx);
            saveOptions.UpdateZoom = true;

            // Salva su stream di memoria
            using (MemoryStream stream = new MemoryStream())
            {
                workbook.Save(stream, saveOptions);
                
                // Ricarica la cartella di lavoro per verificare che lo zoom sia stato aggiornato
                stream.Position = 0;
                Workbook reloadedWorkbook = new Workbook(stream);
                Console.WriteLine("Worksheet zoom level: " + reloadedWorkbook.Worksheets[0].PageSetup.Zoom);
            }
        }
    }
}
```

### Vedi anche

* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


