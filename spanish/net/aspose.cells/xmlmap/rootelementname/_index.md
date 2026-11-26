---
title: "XmlMap.RootElementName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad XmlMap. Obtiene el nombre del elemento raíz"
type: docs
url: /es/net/aspose.cells/xmlmap/rootelementname/
---
## XmlMap.RootElementName property

Obtiene el nombre del elemento raíz.

```csharp
public string RootElementName { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlMapPropertyRootElementNameDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar datos de ejemplo
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);

            // Crear un mapa XML
            string xml = "<root><item><Name>Item1</Name><Value>100</Value></item></root>";
            int mapIndex = workbook.Worksheets.XmlMaps.Add(xml);
            
            // Obtener y mostrar el nombre del elemento raíz
            string rootElementName = workbook.Worksheets.XmlMaps[mapIndex].RootElementName;
            Console.WriteLine("Root Element Name: " + rootElementName);
        }
    }
}
```

### Ver también

* class [XmlMap](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


