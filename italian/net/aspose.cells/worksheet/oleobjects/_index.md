---
title: "Worksheet.OleObjects"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Worksheet. Rappresenta una raccolta di OleObject in un foglio di lavoro"
type: docs
url: /it/net/aspose.cells/worksheet/oleobjects/
---
## Worksheet.OleObjects property

Rappresenta una raccolta di [`OleObject`](../../../aspose.cells.drawing/oleobject/) in un foglio di lavoro.

```csharp
public OleObjectCollection OleObjects { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyOleObjectsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un OleObject al foglio di lavoro
            int oleObjectIndex = worksheet.OleObjects.Add(10, 10, 200, 200, File.ReadAllBytes(@"C:\temp\example.xlsx"));
            OleObject ole = worksheet.OleObjects[oleObjectIndex];
            
            // Modifica le proprietà di OleObject
            ole.ObjectSourceFullName = @"C:\temp\modified.xlsx";
            ole.FileFormatType = FileFormatType.Xlsx;

            // Salva la cartella di lavoro
            workbook.Save(@"C:\temp\output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [OleObjectCollection](../../../aspose.cells.drawing/oleobjectcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


