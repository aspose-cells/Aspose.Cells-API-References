---
title: "BuiltInDocumentPropertyCollection.ScaleCrop"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad BuiltInDocumentPropertyCollection. Indica el modo de visualización de la miniatura del documento"
type: docs
url: /es/net/aspose.cells.properties/builtindocumentpropertycollection/scalecrop/
---
## BuiltInDocumentPropertyCollection.ScaleCrop property

Indica el modo de visualización de la miniatura del documento.

```csharp
public bool ScaleCrop { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyScaleCropDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a las propiedades de documento incorporadas
            BuiltInDocumentPropertyCollection properties = workbook.BuiltInDocumentProperties;
            
            // Establecer la propiedad ScaleCrop
            properties.ScaleCrop = true;
            
            // Mostrar el valor de la propiedad ScaleCrop
            Console.WriteLine("ScaleCrop property value: " + properties.ScaleCrop);
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


