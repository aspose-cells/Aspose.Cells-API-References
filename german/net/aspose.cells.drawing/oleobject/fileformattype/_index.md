---
title: "OleObject.FileFormatType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "OleObject-Eigenschaft. Gibt den Dateityp der eingebetteten Ole-Objektdaten zurück und legt ihn fest"
type: docs
url: /de/net/aspose.cells.drawing/oleobject/fileformattype/
---
## OleObject.FileFormatType property

Liest und setzt den Dateityp der eingebetteten OleObject-Daten

```csharp
public FileFormatType FileFormatType { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyFileFormatTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie ein OLE-Objekt zum Arbeitsblatt hinzu (ohne Dateidaten)
            int oleIndex = worksheet.OleObjects.Add(10, 10, 200, 200, null);
            
            // Rufen Sie das hinzugefügte OLE-Objekt ab
            OleObject oleObject = worksheet.OleObjects[oleIndex];
            
            // Setzen und Anzeigen des Dateiformattyps
            oleObject.FileFormatType = FileFormatType.Docm;
            Console.WriteLine("OLE Object File Format Type: " + oleObject.FileFormatType);
            
            // Speichere die Arbeitsmappe
            workbook.Save("OleObjectFileFormatTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [FileFormatType](../../../aspose.cells/fileformattype/)
* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


