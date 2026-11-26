---
title: "DocumentProperty.Name"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DocumentProperty. Devuelve el nombre de la propiedad"
type: docs
url: /es/net/aspose.cells.properties/documentproperty/name/
---
## DocumentProperty.Name property

Devuelve el nombre de la propiedad.

```csharp
public string Name { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class DocumentPropertyPropertyNameDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceda a las propiedades del documento
            BuiltInDocumentPropertyCollection builtInProps = workbook.BuiltInDocumentProperties;
            CustomDocumentPropertyCollection customProps = workbook.CustomDocumentProperties;
            
            // Agregue una propiedad personalizada y demuestre el uso de Name
            DocumentProperty authorProperty = customProps.Add("Author", "John Doe");
            Console.WriteLine("Property Name: " + authorProperty.Name);
            Console.WriteLine("Property Value: " + authorProperty.Value);
            
            // Acceda a una propiedad incorporada por nombre
            DocumentProperty titleProperty = builtInProps["Title"];
            titleProperty.Value = "Sample Document";
            Console.WriteLine("Title Property Name: " + titleProperty.Name);
            Console.WriteLine("Title Property Value: " + titleProperty.Value);
        }
    }
}
```

### Ver también

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


