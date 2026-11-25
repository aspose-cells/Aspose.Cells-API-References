---
title: "WorkbookSettings.DefaultImageResolution"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorkbookSettings. Ottiene e imposta la risoluzione predefinita dell'immagine"
type: docs
url: /it/net/aspose.cells/workbooksettings/defaultimageresolution/
---
## WorkbookSettings.DefaultImageResolution property

Ottiene e imposta la risoluzione predefinita dell'immagine.

```csharp
public int DefaultImageResolution { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyDefaultImageResolutionDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Imposta la risoluzione predefinita dell'immagine
            workbook.Settings.DefaultImageResolution = 300;
            
            // Aggiungi un foglio di lavoro e inserisci un'immagine
            Worksheet worksheet = workbook.Worksheets[0];
            int imgIndex = worksheet.Pictures.Add(0, 0, "example.jpg");
            Picture picture = worksheet.Pictures[imgIndex];
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
            
            // Verifica la risoluzione predefinita dell'immagine
            Console.WriteLine("Default Image Resolution: " + workbook.Settings.DefaultImageResolution);
        }
    }
}
```

### Vedi anche

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


