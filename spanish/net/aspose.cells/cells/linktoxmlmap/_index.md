---
title: "Cells.LinkToXmlMap"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Enlazar a un mapa XML"
type: docs
url: /es/net/aspose.cells/cells/linktoxmlmap/
---
## Cells.LinkToXmlMap method

Enlace a un mapa XML.

```csharp
public void LinkToXmlMap(string mapName, int row, int column, string path)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| mapName | String | nombre del mapa XML |
| fila | Int32 | fila de la celda de destino |
| columna | Int32 | columna de la celda de destino |
| ruta | String | ruta del elemento xml en el mapa xml |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodLinkToXmlMapWithStringInt32Int32StringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook wb = new Workbook();
            
            // Agregar un mapa XML de ejemplo
            int mapIndex = wb.Worksheets.XmlMaps.Add("<Transmittals><Issued_Document>Test</Issued_Document></Transmittals>");
            XmlMap xmlMap = wb.Worksheets.XmlMaps[mapIndex];
            xmlMap.Name = "Transmittals_Map";
            
            // Obtener la primera hoja de cálculo
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // Vincular celda al mapa XML
            cells.LinkToXmlMap("Transmittals_Map", 0, 0, "/Transmittals/Issued_Document");
            
            // Guarda el libro de trabajo
            wb.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


