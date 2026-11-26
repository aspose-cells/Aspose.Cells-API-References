---
title: "DocumentProperty.IsGeneratedName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "DocumentProperty property. Devuelve true si esta propiedad no tiene un nombre en el almacenamiento OLE2 y se generó un nombre único solo para la API pública"
type: docs
url: /es/net/aspose.cells.properties/documentproperty/isgeneratedname/
---
## DocumentProperty.IsGeneratedName property

Devuelve true si esta propiedad no tiene un nombre en el almacenamiento OLE2 y se generó un nombre único solo para la API pública.

```csharp
public bool IsGeneratedName { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class DocumentPropertyPropertyIsGeneratedNameDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a las propiedades de documento incorporadas
            DocumentPropertyCollection properties = workbook.Worksheets.BuiltInDocumentProperties;
            
            // Accede a las propiedades de documento personalizadas para agregar
            CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;

            // Agregar una propiedad personalizada
            DocumentProperty customProperty = customProperties.Add("CustomProperty", "Test Value");
            
            // Muestra IsGeneratedName para la propiedad incorporada
            DocumentProperty authorProperty = properties["Author"];
            Console.WriteLine("Author property IsGeneratedName: " + authorProperty.IsGeneratedName);
            
            // Muestra IsGeneratedName para la propiedad personalizada
            Console.WriteLine("Custom property IsGeneratedName: " + customProperty.IsGeneratedName);

            // Crea un escenario donde una propiedad pueda tener un nombre generado
            // (Nota: En la práctica, IsGeneratedName es de solo lectura y se establece internamente por Aspose.Cells)
            DocumentProperty generatedNameProperty = properties["_PID_GUID"];
            if (generatedNameProperty != null)
            {
                Console.WriteLine("Generated name property IsGeneratedName: " + generatedNameProperty.IsGeneratedName);
            }

            // Guarda el libro de trabajo
            workbook.Save("PropertyIsGeneratedNameDemo.xlsx");
        }
    }
}
```

### Ver también

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


