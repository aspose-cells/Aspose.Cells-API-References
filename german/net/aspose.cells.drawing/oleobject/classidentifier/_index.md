---
title: "OleObject.ClassIdentifier"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "OleObject-Eigenschaft. Liest und setzt den Klassenbezeichner des eingebetteten Objekts. Es gibt an, welche Anwendung die eingebettete Datei öffnet"
type: docs
url: /de/net/aspose.cells.drawing/oleobject/classidentifier/
---
## OleObject.ClassIdentifier property

Liest und setzt die Klassenkennung des eingebetteten Objekts. Sie gibt an, welche Anwendung die eingebettete Datei öffnet.

```csharp
public byte[] ClassIdentifier { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyClassIdentifierDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Beispiel-Byte-Array für ClassIdentifier (normalerweise wäre dies eine echte Klassen-ID)
            byte[] classId = new byte[] { 0x01, 0x02, 0x03, 0x04, 0x05, 0x06, 0x07, 0x08, 
                                         0x09, 0x0A, 0x0B, 0x0C, 0x0D, 0x0E, 0x0F, 0x10 };

            // OLE-Objekt mit Beispieldaten hinzufügen
            int oleIndex = sheet.OleObjects.Add(10, 10, 200, 100, new byte[100]);
            OleObject oleObject = sheet.OleObjects[oleIndex];
            
            // ClassIdentifier-Eigenschaft festlegen
            oleObject.ClassIdentifier = classId;
            oleObject.ProgID = "Excel.Sheet.12";
            oleObject.DisplayAsIcon = true;

            // Speichere die Arbeitsmappe
            workbook.Save("OleObjectDemo.xlsx");

            // Gespeichertes Arbeitsbuch laden, um den ClassIdentifier zu überprüfen
            Workbook loadedWorkbook = new Workbook("OleObjectDemo.xlsx");
            OleObject loadedOle = loadedWorkbook.Worksheets[0].OleObjects[0];
            
            // Überprüfen Sie, ob der ClassIdentifier erhalten wurde
            Console.WriteLine("ClassIdentifier length: " + loadedOle.ClassIdentifier.Length);
        }
    }
}
```

### Siehe auch

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


