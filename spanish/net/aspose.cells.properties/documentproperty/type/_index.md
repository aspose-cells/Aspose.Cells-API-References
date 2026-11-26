---
title: "DocumentProperty.Type"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DocumentProperty. Obtiene el tipo de datos de la propiedad"
type: docs
url: /es/net/aspose.cells.properties/documentproperty/type/
---
## DocumentProperty.Type property

Obtiene el tipo de datos de la propiedad.

```csharp
public PropertyType Type { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class DocumentPropertyPropertyTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceda a propiedades personalizadas del documento (no incorporadas)
            CustomDocumentPropertyCollection properties = workbook.Worksheets.CustomDocumentProperties;
            
            // Agregue propiedades personalizadas con diferentes tipos
            properties.Add("Author", "John Doe");
            properties.Add("CreatedDate", DateTime.Now);
            properties.Add("Revision", 5);
            properties.Add("IsApproved", true);
            
            // Demostrar el uso de la propiedad Type
            Console.WriteLine("Document Properties and Their Types:");
            foreach (DocumentProperty prop in properties)
            {
                Console.WriteLine($"Name: {prop.Name}, Value: {prop.Value}, Type: {prop.Type}");
            }
            
            // Acceda a una propiedad específica y verifique su tipo
            DocumentProperty dateProp = properties["CreatedDate"];
            if (dateProp.Type == PropertyType.DateTime)
            {
                Console.WriteLine("\nCreatedDate is a DateTime property");
                Console.WriteLine($"Value as DateTime: {dateProp.ToDateTime()}");
            }
        }
    }
}
```

### Ver también

* enum [PropertyType](../../propertytype/)
* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


