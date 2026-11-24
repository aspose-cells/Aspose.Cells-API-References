---
title: "Cells.LinkToXmlMap"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Verknüpfung zu einer XML-Map"
type: docs
url: /de/net/aspose.cells/cells/linktoxmlmap/
---
## Cells.LinkToXmlMap method

Link zu einer XML-Map.

```csharp
public void LinkToXmlMap(string mapName, int row, int column, string path)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| mapName | String | Name der XML-Map |
| row | Int32 | Zeile der Zielzelle |
| column | Int32 | Spalte der Zielzelle |
| Pfad | String | Pfad des XML-Elements in der XML-Map |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodLinkToXmlMapWithStringInt32Int32StringDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook wb = new Workbook();
            
            // Füge eine Beispiel-XML-Map hinzu
            int mapIndex = wb.Worksheets.XmlMaps.Add("<Transmittals><Issued_Document>Test</Issued_Document></Transmittals>");
            XmlMap xmlMap = wb.Worksheets.XmlMaps[mapIndex];
            xmlMap.Name = "Transmittals_Map";
            
            // Hole das erste Arbeitsblatt
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // Zelle mit XML-Map verknüpfen
            cells.LinkToXmlMap("Transmittals_Map", 0, 0, "/Transmittals/Issued_Document");
            
            // Speichere die Arbeitsmappe
            wb.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


