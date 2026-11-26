---
title: "DocumentProperty.Source"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DocumentProperty. La fuente del contenido vinculado"
type: docs
url: /es/net/aspose.cells.properties/documentproperty/source/
---
## DocumentProperty.Source property

La fuente de contenido enlazado.

```csharp
public string Source { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class DocumentPropertyPropertySourceDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a las propiedades de documento personalizadas
            var properties = workbook.Worksheets.CustomDocumentProperties;

            // Agregue propiedades
            properties.Add("Author", "John Doe");
            properties.Add("CreatedDate", DateTime.Now);
            properties.Add("Revision", 1);
            
            // Obtenga las propiedades y muestre sus fuentes
            Console.WriteLine("Property Sources:");
            Console.WriteLine($"Author: {properties["Author"].Source}");
            Console.WriteLine($"CreatedDate: {properties["CreatedDate"].Source}");
            Console.WriteLine($"Revision: {properties["Revision"].Source}");

            // Guarda el libro de trabajo
            workbook.Save("DocumentPropertiesDemo.xlsx");
        }
    }
}
```

### Ver también

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


