---
title: "OleObject.AutoLoad"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà OleObject. Specifica se l'applicazione host per l'oggetto incorporato deve essere chiamata per caricare automaticamente i dati dell'oggetto quando la cartella di lavoro principale viene aperta"
type: docs
url: /it/net/aspose.cells.drawing/oleobject/autoload/
---
## OleObject.AutoLoad property

Specifica se l'applicazione host per l'oggetto incorporato deve essere chiamata per caricare i dati dell'oggetto automaticamente quando la cartella di lavoro principale viene aperta.

```csharp
public bool AutoLoad { get; set; }
```

### Esempi

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyAutoLoadDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi un OleObject al foglio di lavoro
            int oleNumber = sheet.OleObjects.Add(10, 10, 200, 200, new byte[0]);
            
            // Imposta le proprietà di OleObject
            OleObject ole = sheet.OleObjects[oleNumber];
            ole.ProgID = "Excel.Sheet";
            ole.ObjectData = new byte[0];
            
            // Dimostra la proprietà AutoLoad
            ole.AutoLoad = true; // Automatically load the OleObject when the workbook opens
            
            // Salva la cartella di lavoro
            workbook.Save("OleObjectAutoLoadDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


