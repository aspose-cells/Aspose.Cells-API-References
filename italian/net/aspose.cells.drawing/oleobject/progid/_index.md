---
title: "OleObject.ProgID"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà OleObject. Ottiene o imposta il ProgID dell'oggetto OLE"
type: docs
url: /it/net/aspose.cells.drawing/oleobject/progid/
---
## OleObject.ProgID property

Ottiene o imposta il ProgID dell'oggetto OLE.

```csharp
public string ProgID { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyProgIDDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un oggetto OLE al foglio di lavoro
            int oleIndex = worksheet.OleObjects.Add(10, 10, 200, 200, new byte[0], "test.pdf");
            OleObject ole = worksheet.OleObjects[oleIndex];
            
            // Imposta il ProgID per l'oggetto OLE
            ole.ProgID = "AcroExch.Document.DC";
            
            // Visualizza il ProgID
            Console.WriteLine("OLE Object ProgID: " + ole.ProgID);

            // Salva la cartella di lavoro
            workbook.Save("OleObjectProgIDDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


