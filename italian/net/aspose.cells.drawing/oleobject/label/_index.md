---
title: "OleObject.Label"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà OleObject. Ottiene e imposta l'etichetta di visualizzazione dell'oggetto ole collegato"
type: docs
url: /it/net/aspose.cells.drawing/oleobject/label/
---
## OleObject.Label property

Ottiene e imposta l'etichetta di visualizzazione dell'oggetto ole collegato.

```csharp
public string Label { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyLabelDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un oggetto OLE con un'etichetta
            int oleIndex = worksheet.OleObjects.Add(10, 10, 200, 200, new byte[0]);
            OleObject oleObject = worksheet.OleObjects[oleIndex];
            oleObject.Label = "label_nameです";

            // Salva e ricarica il workbook
            string outputPath = "output.xlsx";
            workbook.Save(outputPath);
            
            // Verifica la proprietà label
            Workbook loadedWorkbook = new Workbook(outputPath);
            OleObject loadedOleObject = loadedWorkbook.Worksheets[0].OleObjects[0];
            Console.WriteLine("OLE Object Label: " + loadedOleObject.Label);
        }
    }
}
```

### Vedi anche

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


