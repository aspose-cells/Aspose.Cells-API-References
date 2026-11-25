---
title: "PaginatedSaveOptions.EmfRenderSetting"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PaginatedSaveOptions. Impostazione per il rendering del metafile Emf"
type: docs
url: /it/net/aspose.cells/paginatedsaveoptions/emfrendersetting/
---
## PaginatedSaveOptions.EmfRenderSetting property

Impostazione per il rendering del metafile Emf.

```csharp
public EmfRenderSetting EmfRenderSetting { get; set; }
```

### Osservazioni

I metafili EMF identificati come "EMF+ Dual" possono contenere sia record EMF+ sia record EMF. Entrambi i tipi di record possono essere usati per renderizzare l'immagine, solo record EMF+, o solo record EMF. Quando EmfPlusPrefer è impostato, i record EMF+ verranno analizzati durante il rendering della pagina, altrimenti verranno analizzati solo i record EMF. Il valore predefinito è EmfOnly.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyEmfRenderSettingDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("EMF Render Setting Demo");
            worksheet.Cells["A2"].PutValue(DateTime.Now.ToString());

            // Crea immagine per la dimostrazione EMF
            worksheet.Pictures.Add(10, 10, "example.png");

            // Configura le opzioni di salvataggio con le impostazioni EMF usando PdfSaveOptions
            PdfSaveOptions options = new PdfSaveOptions()
            {
                EmfRenderSetting = EmfRenderSetting.EmfPlusPrefer
            };

            // Salva la cartella di lavoro con le impostazioni EMF
            workbook.Save("EmfRenderSettingDemo.pdf", options);
        }
    }
}
```

### Vedi anche

* enum [EmfRenderSetting](../../emfrendersetting/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


