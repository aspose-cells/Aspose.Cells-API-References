---
title: "WorkbookSettings.DiscardImageEditData"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorkbookSettings. Indica se scartare i dati di modifica dell'immagine"
type: docs
url: /it/net/aspose.cells/workbooksettings/discardimageeditdata/
---
## WorkbookSettings.DiscardImageEditData property

Indica se scartare i dati di immagine in fase di modifica.

```csharp
public bool DiscardImageEditData { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyDiscardImageEditDataDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi un'immagine al foglio di lavoro
            int index = worksheet.Pictures.Add(0, 0, "example.jpg");
            Picture picture = worksheet.Pictures[index];
            
            // Imposta DiscardImageEditData su true (il valore predefinito è false)
            workbook.Settings.DiscardImageEditData = true;
            
            // Salva la cartella di lavoro
            workbook.Save("output_with_discarded_image_data.xlsx", SaveFormat.Xlsx);
            
            // Verifica che l'impostazione sia stata applicata
            Console.WriteLine("DiscardImageEditData is set to: " + workbook.Settings.DiscardImageEditData);
        }
    }
}
```

### Vedi anche

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


