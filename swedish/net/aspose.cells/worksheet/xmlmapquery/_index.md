---
title: "Worksheet.XmlMapQuery"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet metod. Fråga cellområden som är mappade/länkade till den specifika sökvägen för xml-kartan"
type: docs
url: /sv/net/aspose.cells/worksheet/xmlmapquery/
---
## Worksheet.XmlMapQuery method

Fråga cellområden som är mappade/länkade till den specifika sökvägen för xml-kartan.

```csharp
[Obsolete("Use Worksheet.GetAreasOfXmlMapQuery() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList XmlMapQuery(string path, XmlMap xmlMap)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sökväg | String | xml-element-sökväg |
| xmlMap | XmlMap | Ange en xml-karta om du vill fråga efter den specifika sökvägen inom en specifik karta |

### Returvärde

[`CellArea`](../../cellarea/) list that mapped/linked to the specific path of xml map, an empty list is returned if nothing is mapped/linked.

### Anmärkningar

OBS: Denna metod är nu föråldrad. Använd istället Worksheet.GetAreasOfXmlMapQuery() metod. Denna egenskap kommer att tas bort 12 månader senare från och med augusti 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodXmlMapQueryWithStringXmlMapDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till ett kalkylblad
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa ett exempel på XML-karta
            string xml = @"<?xml version='1.0' encoding='UTF-8'?>
                <ns1:Root xmlns:ns1='http://example.com'>
                    <ns1:Data>
                        <ns1:Item>Value1</ns1:Item>
                    </ns1:Data>
                </ns1:Root>";
            
            // Importera XML för att skapa kartan
            workbook.ImportXml(xml, "Sheet1", 0, 0);
            
            // Hämta XML-kartan
            XmlMap xmlMap = workbook.Worksheets.XmlMaps[0];
            
            // Fråga XML-kartan
            ArrayList cellAreas = worksheet.XmlMapQuery("/ns1:Root/ns1:Data/ns1:Item", xmlMap);
            
            // Skriv ut resultat
            if (cellAreas.Count > 0)
            {
                CellArea area = (CellArea)cellAreas[0];
                Console.WriteLine($"Found data at row {area.StartRow}, column {area.StartColumn}");
                Console.WriteLine($"Cell value: {worksheet.Cells[area.StartRow, area.StartColumn].StringValue}");
            }
        }
    }
}
```

### Se även

* class [XmlMap](../../xmlmap/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


