---
title: "OleObject.ObjectSourceFullName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "OleObject-Eigenschaft. Gibt den vollständigen Namen der Quelldatei für das verknüpfte OLE-Objekt zurück"
type: docs
url: /de/net/aspose.cells.drawing/oleobject/objectsourcefullname/
---
## OleObject.ObjectSourceFullName property

Gibt den vollständigen Namen der Quelldatei für das verknüpfte OLE-Objekt zurück.

```csharp
public string ObjectSourceFullName { get; set; }
```

### Hinweise

Unterstützt das Festlegen des vollständigen Quellnamens nur, wenn der Dateityp OleFileType.Unknown ist. Zum Beispiel wav-Datei, avi-Datei usw.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyObjectSourceFullNameDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // OLE-Objekt hinzufügen (Dateidaten als Byte-Array verwenden)
            byte[] fileData = System.IO.File.ReadAllBytes("test.docx");
            int oleObjectIndex = worksheet.OleObjects.Add(10, 10, 200, 200, fileData);
            Aspose.Cells.Drawing.OleObject oleObject = worksheet.OleObjects[oleObjectIndex];

            // ObjectSourceFullName setzen und abrufen
            oleObject.ObjectSourceFullName = "C:\\Temp\\source.docx";
            Console.WriteLine("OLE Object Source Full Name: " + oleObject.ObjectSourceFullName);

            // Speichere die Arbeitsmappe
            workbook.Save("OleObjectDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


