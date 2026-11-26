---
title: "CustomDocumentPropertyCollection.UpdateLinkedRange"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método CustomDocumentPropertyCollection. Actualiza todos los rangos que están vinculados a propiedades personalizadas usando el valor de la propiedad de documento personalizada para actualizar el valor de la celda del rango vinculado."
type: docs
url: /es/net/aspose.cells.properties/customdocumentpropertycollection/updatelinkedrange/
---
## CustomDocumentPropertyCollection.UpdateLinkedRange method

Actualiza todos los rangos que están vinculados a propiedades personalizadas (utiliza el valor de la propiedad de documento personalizada para actualizar el valor de celda del rango vinculado).

```csharp
public void UpdateLinkedRange()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class CustomDocumentPropertyCollectionMethodUpdateLinkedRangeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer un valor en la celda A1 que se vinculará
            worksheet.Cells["A1"].PutValue("Linked Cell Value");

            CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;
            
            // Agregar una propiedad vinculada
            customProperties.AddLinkToContent("LinkedRange", "Sheet1!A1");
            
            // Actualizar todas las propiedades vinculadas
            customProperties.UpdateLinkedRange();
            
            // Obtener y mostrar el valor de la propiedad vinculada
            DocumentProperty linkedProp = customProperties["LinkedRange"];
            Console.WriteLine($"Linked Property Value: {linkedProp.Value}");

            // Guarda el libro de trabajo
            workbook.Save("LinkedRangeExample.xlsx");
        }
    }
}
```

### Ver también

* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


