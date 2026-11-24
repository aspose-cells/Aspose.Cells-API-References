---
title: "OleObject.IsAutoSize"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "OleObject-Eigenschaft. True zeigt an, dass die Größe des Ole-Objekts automatisch geändert wird, entsprechend der Größe des Schnappschusses des eingebetteten Inhalts, wenn das Ole-Objekt aktiviert wird."
type: docs
url: /de/net/aspose.cells.drawing/oleobject/isautosize/
---
## OleObject.IsAutoSize property

True zeigt an, dass die Größe des OLE-Objekts automatisch geändert wird, entsprechend der Größe des Schnappschusses des eingebetteten Inhalts, wenn das OLE-Objekt aktiviert wird.

```csharp
public bool IsAutoSize { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyIsAutoSizeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // OLE-Objekt hinzufügen (Dateidaten als Byte-Array verwenden)
            byte[] oleData = System.IO.File.ReadAllBytes(@"C:\example\test.docx");
            int oleIndex = worksheet.OleObjects.Add(10, 10, 200, 200, oleData);
            Aspose.Cells.Drawing.OleObject oleObject = worksheet.OleObjects[oleIndex];

            // IsAutoSize-Eigenschaft setzen und demonstrieren
            oleObject.IsAutoSize = true;
            Console.WriteLine("OLE Object AutoSize initially: " + oleObject.IsAutoSize);

            // Ändern Sie die Eigenschaft
            oleObject.IsAutoSize = false;
            Console.WriteLine("OLE Object AutoSize after change: " + oleObject.IsAutoSize);

            // Speichere die Arbeitsmappe
            workbook.Save("OleObjectIsAutoSizeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


