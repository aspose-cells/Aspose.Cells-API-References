---
title: "Cells.LinkToXmlMap"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Länk till en XML-karta"
type: docs
url: /sv/net/aspose.cells/cells/linktoxmlmap/
---
## Cells.LinkToXmlMap method

Länk till en XML-karta.

```csharp
public void LinkToXmlMap(string mapName, int row, int column, string path)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| mapName | String | namn på XML-karta |
| row | Int32 | rad för destinationscellen |
| column | Int32 | kolumn för destinationscellen |
| sökväg | String | sökväg för XML-element i XML-karta |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodLinkToXmlMapWithStringInt32Int32StringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook wb = new Workbook();
            
            // Lägg till ett exempel på XML-karta
            int mapIndex = wb.Worksheets.XmlMaps.Add("<Transmittals><Issued_Document>Test</Issued_Document></Transmittals>");
            XmlMap xmlMap = wb.Worksheets.XmlMaps[mapIndex];
            xmlMap.Name = "Transmittals_Map";
            
            // Hämta det första kalkylbladet
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // Länka cell till XML-karta
            cells.LinkToXmlMap("Transmittals_Map", 0, 0, "/Transmittals/Issued_Document");
            
            // Spara arbetsboken
            wb.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


