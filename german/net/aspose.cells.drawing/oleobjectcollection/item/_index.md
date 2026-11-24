---
title: "OleObjectCollection.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "OleObjectCollection-Eigenschaft. Gibt das OleObject-Element am angegebenen Index zurück"
type: docs
url: /de/net/aspose.cells.drawing/oleobjectcollection/item/
---
## OleObjectCollection indexer

Gibt das [`OleObject`](../../oleobject/) Element am angegebenen Index zurück.

```csharp
public OleObject this[int index] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| Index | Der nullbasierte Index des Elements. |

### Rückgabewert

Das Element am angegebenen Index.

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Beispielbilddaten hinzufügen
            byte[] binaryImg = File.ReadAllBytes("image1.png");
            
            // OLE-Objekt zum ersten Arbeitsblatt hinzufügen
            int idxOle = workbook.Worksheets[0].OleObjects.Add(0, 0, 60, 60, binaryImg);
            
            // Auf das OLE-Objekt über die Item-Eigenschaft zugreifen
            OleObject objOle = workbook.Worksheets[0].OleObjects[idxOle];
            
            // Eingebettete Objekt‑Eigenschaften festlegen
            byte[] binaryXlsx = File.ReadAllBytes("example.xlsx");
            objOle.SetEmbeddedObject(false, binaryXlsx, "SampleFile.xlsx", true, "Excel.Sheet", false);
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
            
            // Überprüfen Sie die gespeicherte Datei
            Workbook savedWorkbook = new Workbook("output.xlsx");
            Console.WriteLine("OLE Object Source: " + savedWorkbook.Worksheets[0].OleObjects[0].ObjectSourceFullName);
        }
    }
}
```

### Siehe auch

* class [OleObject](../../oleobject/)
* class [OleObjectCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


