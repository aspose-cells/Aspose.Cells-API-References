---
title: "WorkbookSettings.AutoCompressPictures"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorkbookSettings. Specifica un valore booleano che indica se l'applicazione comprime automaticamente le immagini nella cartella di lavoro"
type: docs
url: /it/net/aspose.cells/workbooksettings/autocompresspictures/
---
## WorkbookSettings.AutoCompressPictures property

Specifica un valore booleano che indica che l'applicazione comprime automaticamente le immagini nella cartella di lavoro.

```csharp
public bool AutoCompressPictures { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyAutoCompressPicturesDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Abilita AutoCompressPictures
            workbook.Settings.AutoCompressPictures = true;
            
            // Aggiungi un'immagine di esempio per dimostrare la compressione
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Pictures.Add(0, 0, "example.jpg");
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
            
            // Carica la cartella di lavoro salvata per verificare l'impostazione
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Console.WriteLine("AutoCompressPictures: " + loadedWorkbook.Settings.AutoCompressPictures);
        }
    }
}
```

### Vedi anche

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


