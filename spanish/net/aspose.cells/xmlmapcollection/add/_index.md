---
title: "XmlMapCollection.Add"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método XmlMapCollection. Añada un XmlMap mediante la url/ruta de un archivo xml/xsd"
type: docs
url: /es/net/aspose.cells/xmlmapcollection/add/
---
## XmlMapCollection.Add method

Agregar un [`XmlMap`](../../xmlmap/) mediante la url/ruta de un archivo xml/xsd.

```csharp
public int Add(string url)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| url | String | url/ruta de un archivo xml/xsd. |

### Valor de retorno

[`XmlMap`](../../xmlmap/) object index.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlMapCollectionMethodAddWithStringDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            
            XmlMapCollection xmlMapCollection = wb.Worksheets.XmlMaps;
            
            // Agregar mapas XML usando esquemas y archivos XML
            xmlMapCollection.Add("schema.xsd");
            xmlMapCollection.Add("xml.xml");
            
            wb.Save("twoXmlMaps.xlsx");
        }
    }
}
```

### Ver también

* class [XmlMapCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


