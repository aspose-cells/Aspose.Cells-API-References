---
title: "Worksheet.XmlMapQuery"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Methode. Abfrage von Zellbereichen, die dem spezifischen Pfad der XML-Karte zugeordnet/verknüpft sind."
type: docs
url: /de/net/aspose.cells/worksheet/xmlmapquery/
---
## Worksheet.XmlMapQuery method

Abfrage von Zellbereichen, die dem spezifischen Pfad einer XML-Zuordnung zugeordnet/verknüpft sind.

```csharp
[Obsolete("Use Worksheet.GetAreasOfXmlMapQuery() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList XmlMapQuery(string path, XmlMap xmlMap)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Pfad | String | XML-Elementpfad |
| xmlMap | XmlMap | Geben Sie eine XML-Karte an, wenn Sie den spezifischen Pfad innerhalb einer bestimmten Karte abfragen möchten |

### Rückgabewert

[`CellArea`](../../cellarea/) list that mapped/linked to the specific path of xml map, an empty list is returned if nothing is mapped/linked.

### Hinweise

HINWEIS: Diese Methode ist jetzt veraltet. Verwenden Sie stattdessen die Methode Worksheet.GetAreasOfXmlMapQuery(). Diese Eigenschaft wird 12 Monate später, seit August 2026, entfernt werden. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

### Beispiele

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
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            
            // Arbeitsblatt hinzufügen
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Erstelle eine Beispiel-XML-Karte
            string xml = @"<?xml version='1.0' encoding='UTF-8'?>
                <ns1:Root xmlns:ns1='http://example.com'>
                    <ns1:Data>
                        <ns1:Item>Value1</ns1:Item>
                    </ns1:Data>
                </ns1:Root>";
            
            // Importiere XML, um die Karte zu erstellen
            workbook.ImportXml(xml, "Sheet1", 0, 0);
            
            // Rufe die XML-Karte ab
            XmlMap xmlMap = workbook.Worksheets.XmlMaps[0];
            
            // Abfrage der XML-Karte
            ArrayList cellAreas = worksheet.XmlMapQuery("/ns1:Root/ns1:Data/ns1:Item", xmlMap);
            
            // Ergebnisse ausgeben
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

### Siehe auch

* class [XmlMap](../../xmlmap/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


