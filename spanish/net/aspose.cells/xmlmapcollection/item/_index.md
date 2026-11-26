---
title: "XmlMapCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad XmlMapCollection. Obtiene el mapa xml por el índice específico"
type: docs
url: /es/net/aspose.cells/xmlmapcollection/item/
---
## XmlMapCollection indexer

Obtiene el mapa xml por el índice específico.

```csharp
public XmlMap this[int index] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| índice | El índice. |

### Valor de retorno

El mapa xml

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlMapCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceda a XmlMapCollection desde el libro de trabajo
            XmlMapCollection xmlMaps = workbook.Worksheets.XmlMaps;

            // Agregue un nuevo XmlMap a la colección
            int xmlMapIndex = xmlMaps.Add("data.xsd");

            // Acceder al XmlMap usando la propiedad Item
            XmlMap xmlMap = xmlMaps[xmlMapIndex];

            // Mostrar el nombre del XmlMap
            Console.WriteLine("XmlMap Name: " + xmlMap.Name);

            // Guarda el libro de trabajo
            workbook.Save("XmlMapCollectionExample.xlsx");
        }
    }
}
```

### Ver también

* class [XmlMap](../../xmlmap/)
* class [XmlMapCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


