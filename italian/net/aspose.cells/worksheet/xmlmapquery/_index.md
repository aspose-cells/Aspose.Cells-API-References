---
title: "Worksheet.XmlMapQuery"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Worksheet. Interroga le aree di celle che sono state mappate/collegate al percorso specifico della mappa xml"
type: docs
url: /it/net/aspose.cells/worksheet/xmlmapquery/
---
## Worksheet.XmlMapQuery method

Interroga le aree di celle mappate/collegate al percorso specifico della mappa XML.

```csharp
[Obsolete("Use Worksheet.GetAreasOfXmlMapQuery() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList XmlMapQuery(string path, XmlMap xmlMap)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| percorso | String | percorso dell'elemento xml |
| xmlMap | XmlMap | Specifica una mappa xml se desideri interrogare il percorso specifico all'interno di una mappa specifica |

### Valore di ritorno

[`CellArea`](../../cellarea/) list that mapped/linked to the specific path of xml map, an empty list is returned if nothing is mapped/linked.

### Osservazioni

NOTA: Questo metodo è ora obsoleto. Invece, utilizza il metodo Worksheet.GetAreasOfXmlMapQuery(). Questa proprietà sarà rimossa 12 mesi dopo, a partire da agosto 2026. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

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
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            
            // Aggiungi un foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea una mappa XML di esempio
            string xml = @"<?xml version='1.0' encoding='UTF-8'?>
                <ns1:Root xmlns:ns1='http://example.com'>
                    <ns1:Data>
                        <ns1:Item>Value1</ns1:Item>
                    </ns1:Data>
                </ns1:Root>";
            
            // Importa XML per creare la mappa
            workbook.ImportXml(xml, "Sheet1", 0, 0);
            
            // Ottieni la mappa XML
            XmlMap xmlMap = workbook.Worksheets.XmlMaps[0];
            
            // Interroga la mappa XML
            ArrayList cellAreas = worksheet.XmlMapQuery("/ns1:Root/ns1:Data/ns1:Item", xmlMap);
            
            // Restituisci i risultati
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

### Vedi anche

* class [XmlMap](../../xmlmap/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


