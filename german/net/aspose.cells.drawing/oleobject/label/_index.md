---
title: "OleObject.Label"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "OleObject-Eigenschaft. Gibt das Anzeigetext-Label des verknüpften Ole-Objekts zurück und legt es fest"
type: docs
url: /de/net/aspose.cells.drawing/oleobject/label/
---
## OleObject.Label property

Liest und setzt die Anzeigebezeichnung des verknüpften OleObject.

```csharp
public string Label { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie ein OLE-Objekt mit einem Label hinzu
            int oleIndex = worksheet.OleObjects.Add(10, 10, 200, 200, new byte[0]);
            OleObject oleObject = worksheet.OleObjects[oleIndex];
            oleObject.Label = "label_nameです";

            // Speichere das Workbook und lade es erneut
            string outputPath = "output.xlsx";
            workbook.Save(outputPath);
            
            // Überprüfen Sie die Label-Eigenschaft
            Workbook loadedWorkbook = new Workbook(outputPath);
            OleObject loadedOleObject = loadedWorkbook.Worksheets[0].OleObjects[0];
            Console.WriteLine("OLE Object Label: " + loadedOleObject.Label);
        }
    }
}
```

### Siehe auch

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


