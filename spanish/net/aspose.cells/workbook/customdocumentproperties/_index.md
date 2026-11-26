---
title: "Workbook.CustomDocumentProperties"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Workbook property. Devuelve una colección DocumentProperty que representa todas las propiedades de documento personalizadas de la hoja de cálculo"
type: docs
url: /es/net/aspose.cells/workbook/customdocumentproperties/
---
## Workbook.CustomDocumentProperties property

Devuelve una colección [`DocumentProperty`](../../../aspose.cells.properties/documentproperty/) que representa todas las propiedades de documento personalizadas de la hoja de cálculo.

```csharp
public CustomDocumentPropertyCollection CustomDocumentProperties { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyCustomDocumentPropertiesDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar propiedades de documento personalizadas
            workbook.CustomDocumentProperties.Add("Author", "John Doe");
            workbook.CustomDocumentProperties.Add("Created Date", DateTime.Now);
            workbook.CustomDocumentProperties.Add("Revision", 1);
            workbook.CustomDocumentProperties.Add("Approved", true);
            
            // Acceder y mostrar las propiedades personalizadas
            Console.WriteLine("Custom Document Properties:");
            foreach (Aspose.Cells.Properties.DocumentProperty prop in workbook.CustomDocumentProperties)
            {
                Console.WriteLine($"{prop.Name}: {prop.Value} ({prop.Type})");
            }
            
            // Guarda el libro de trabajo
            workbook.Save("CustomDocumentPropertiesDemo.xlsx");
        }
    }
}
```

### Ver también

* class [CustomDocumentPropertyCollection](../../../aspose.cells.properties/customdocumentpropertycollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


