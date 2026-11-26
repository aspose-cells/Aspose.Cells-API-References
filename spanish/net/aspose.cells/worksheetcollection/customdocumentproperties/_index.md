---
title: "WorksheetCollection.CustomDocumentProperties"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorksheetCollection. Devuelve una colección DocumentProperty que representa todas las propiedades de documento personalizadas de la hoja de cálculo"
type: docs
url: /es/net/aspose.cells/worksheetcollection/customdocumentproperties/
---
## WorksheetCollection.CustomDocumentProperties property

Devuelve una colección [`DocumentProperty`](../../../aspose.cells.properties/documentproperty/) que representa todas las propiedades de documento personalizadas de la hoja de cálculo.

```csharp
public CustomDocumentPropertyCollection CustomDocumentProperties { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyCustomDocumentPropertiesDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar propiedades de documento personalizadas
            workbook.Worksheets.CustomDocumentProperties.Add("Author", "John Doe");
            workbook.Worksheets.CustomDocumentProperties.Add("CreatedDate", DateTime.Now);
            workbook.Worksheets.CustomDocumentProperties.Add("Version", 1.2);
            
            // Acceder y mostrar las propiedades
            Console.WriteLine("Author: " + workbook.Worksheets.CustomDocumentProperties["Author"]);
            Console.WriteLine("Created: " + workbook.Worksheets.CustomDocumentProperties["CreatedDate"]);
            Console.WriteLine("Version: " + workbook.Worksheets.CustomDocumentProperties["Version"]);
        }
    }
}
```

### Ver también

* class [CustomDocumentPropertyCollection](../../../aspose.cells.properties/customdocumentpropertycollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


