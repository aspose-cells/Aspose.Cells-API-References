---
title: "OleObject.FullObjectBin"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "OleObject Eigenschaft. Gibt die vollständigen eingebetteten OLE-Objektdaten im Binärformat in der Vorlagendatei zurück"
type: docs
url: /de/net/aspose.cells.drawing/oleobject/fullobjectbin/
---
## OleObject.FullObjectBin property

Liest die vollständigen binären Daten des eingebetteten OleObject in der Vorlagendatei.

```csharp
public byte[] FullObjectBin { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class OleObjectPropertyFullObjectBinDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ein OLE-Objekt zum Arbeitsblatt hinzufügen
            byte[] objectData = File.ReadAllBytes("example.docx");
            int oleObjectIndex = worksheet.OleObjects.Add(10, 10, 200, 200, objectData, "docx");
            OleObject oleObject = worksheet.OleObjects[oleObjectIndex];

            // Einige Eigenschaften für das OLE-Objekt festlegen
            oleObject.FileFormatType = FileFormatType.Docx;
            oleObject.ObjectData = objectData;
            oleObject.IsAutoSize = true;

            // FullObjectBin-Daten abrufen (schreibgeschützte Eigenschaft)
            byte[] fullObjectBinData = oleObject.FullObjectBin;
            Console.WriteLine("FullObjectBin data length: " + (fullObjectBinData != null ? fullObjectBinData.Length.ToString() : "null"));

            // Verwendung von FullObjectBin demonstrieren, indem es in einer Datei gespeichert wird
            if (fullObjectBinData != null && fullObjectBinData.Length > 0)
            {
                File.WriteAllBytes("FullObjectBinData.bin", fullObjectBinData);
                Console.WriteLine("Saved FullObjectBin data to file.");
            }

            // Ein weiteres Arbeitsbuch erstellen, um das Lesen des OLE-Objekts zu demonstrieren
            Workbook workbook2 = new Workbook();
            Worksheet worksheet2 = workbook2.Worksheets[0];

            // OLE-Objekt aus den FullObjectBin-Daten hinzufügen
            if (fullObjectBinData != null)
            {
                int newOleObjectIndex = worksheet2.OleObjects.Add(10, 10, 200, 200, fullObjectBinData, "docx");
                Console.WriteLine("Added new OLE object using FullObjectBin data.");
            }

            // Arbeitsmappen speichern
            workbook.Save("OleObjectWithFullObjectBin.xlsx");
            workbook2.Save("OleObjectFromFullObjectBin.xlsx");
        }
    }
}
```

### Siehe auch

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


