---
title: "Cells.LinkToXmlMap"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cells. Collegamento a una mappa XML"
type: docs
url: /it/net/aspose.cells/cells/linktoxmlmap/
---
## Cells.LinkToXmlMap method

Collegamento a una mappa XML.

```csharp
public void LinkToXmlMap(string mapName, int row, int column, string path)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| mapName | String | nome della mappa XML |
| riga | Int32 | riga della cella di destinazione |
| colonna | Int32 | colonna della cella di destinazione |
| percorso | String | percorso dell'elemento xml nella mappa xml |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodLinkToXmlMapWithStringInt32Int32StringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook wb = new Workbook();
            
            // Aggiungi una mappa XML di esempio
            int mapIndex = wb.Worksheets.XmlMaps.Add("<Transmittals><Issued_Document>Test</Issued_Document></Transmittals>");
            XmlMap xmlMap = wb.Worksheets.XmlMaps[mapIndex];
            xmlMap.Name = "Transmittals_Map";
            
            // Ottieni il primo foglio di lavoro
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // Collega la cella alla mappa XML
            cells.LinkToXmlMap("Transmittals_Map", 0, 0, "/Transmittals/Issued_Document");
            
            // Salva la cartella di lavoro
            wb.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


