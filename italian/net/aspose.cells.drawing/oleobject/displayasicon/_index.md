---
title: "OleObject.DisplayAsIcon"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà OleObject. True se l'oggetto specificato è visualizzato come icona e l'immagine non verrà modificata automaticamente"
type: docs
url: /it/net/aspose.cells.drawing/oleobject/displayasicon/
---
## OleObject.DisplayAsIcon property

True se l'oggetto specificato è visualizzato come icona e l'immagine non verrà modificata automaticamente.

```csharp
public bool DisplayAsIcon { get; set; }
```

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyDisplayAsIconDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un oggetto OLE (PDF) al foglio di lavoro
            byte[] pdfData = File.ReadAllBytes("example.pdf");
            int oleIndex = worksheet.OleObjects.Add(10, 10, 200, 200, pdfData);
            
            // Ottieni l'oggetto OLE
            Aspose.Cells.Drawing.OleObject oleObject = worksheet.OleObjects[oleIndex];
            oleObject.ProgID = "AcroExch.Document.DC";
            
            // Dimostra la proprietà DisplayAsIcon
            oleObject.DisplayAsIcon = true; // Show as icon
            // oleObject.DisplayAsIcon = false; // Mostra il contenuto se possibile
            
            // Salva la cartella di lavoro
            workbook.Save("OleObjectDisplayAsIconDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


