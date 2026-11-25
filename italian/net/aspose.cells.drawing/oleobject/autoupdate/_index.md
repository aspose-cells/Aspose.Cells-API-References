---
title: "OleObject.AutoUpdate"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà OleObject. Specifica se il collegamento a OleObject viene aggiornato automaticamente o meno"
type: docs
url: /it/net/aspose.cells.drawing/oleobject/autoupdate/
---
## OleObject.AutoUpdate property

Specifica se il collegamento all'OleObject viene aggiornato automaticamente o meno.

```csharp
public bool AutoUpdate { get; set; }
```

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyAutoUpdateDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Crea file di esempio per la dimostrazione
            string imagePath = "OleObjectExample.jpg";
            string excelPath = "OleObjectExample.xls";
            
            // Crea un file immagine di esempio se non esiste
            if (!File.Exists(imagePath))
            {
                using (File.Create(imagePath)) { }
            }

            // Crea un file Excel di esempio se non esiste
            if (!File.Exists(excelPath))
            {
                new Workbook().Save(excelPath);
            }

            // Leggi i dati dell'immagine
            byte[] imageData = File.ReadAllBytes(imagePath);
            
            // Aggiungi OleObject al foglio di lavoro
            int oleIndex = sheet.OleObjects.Add(1, 1, 200, 200, imageData);
            Aspose.Cells.Drawing.OleObject oleObject = sheet.OleObjects[oleIndex];
            
            // Imposta le proprietà di OleObject
            oleObject.ObjectData = File.ReadAllBytes(excelPath);
            oleObject.ProgID = "Excel.Sheet.8";
            oleObject.DisplayAsIcon = true;
            
            // Dimostra la proprietà AutoUpdate
            oleObject.AutoUpdate = false; // When false, the object won't update automatically when source changes
            
            // Salva la cartella di lavoro
            workbook.Save("OleObjectAutoUpdateDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


