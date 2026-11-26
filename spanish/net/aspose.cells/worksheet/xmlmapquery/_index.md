---
title: "Worksheet.XmlMapQuery"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Worksheet. Consultar áreas de celdas que están mapeadas/vinculadas a la ruta específica del mapa xml"
type: docs
url: /es/net/aspose.cells/worksheet/xmlmapquery/
---
## Worksheet.XmlMapQuery method

Consulta áreas de celdas que están mapeadas/enlazadas a la ruta específica del mapa XML.

```csharp
[Obsolete("Use Worksheet.GetAreasOfXmlMapQuery() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList XmlMapQuery(string path, XmlMap xmlMap)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| ruta | String | ruta del elemento xml |
| xmlMap | XmlMap | Especifique un mapa xml si desea consultar la ruta específica dentro de un mapa específico |

### Valor de retorno

[`CellArea`](../../cellarea/) list that mapped/linked to the specific path of xml map, an empty list is returned if nothing is mapped/linked.

### Observaciones

NOTA: Este método está ahora obsoleto. En su lugar, utilice el método Worksheet.GetAreasOfXmlMapQuery(). Esta propiedad será eliminada 12 meses después, a partir de agosto de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

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
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar una hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crear un mapa XML de ejemplo
            string xml = @"<?xml version='1.0' encoding='UTF-8'?>
                <ns1:Root xmlns:ns1='http://example.com'>
                    <ns1:Data>
                        <ns1:Item>Value1</ns1:Item>
                    </ns1:Data>
                </ns1:Root>";
            
            // Importar XML para crear el mapa
            workbook.ImportXml(xml, "Sheet1", 0, 0);
            
            // Obtener el mapa XML
            XmlMap xmlMap = workbook.Worksheets.XmlMaps[0];
            
            // Consultar el mapa XML
            ArrayList cellAreas = worksheet.XmlMapQuery("/ns1:Root/ns1:Data/ns1:Item", xmlMap);
            
            // Mostrar resultados
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

### Ver también

* class [XmlMap](../../xmlmap/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


