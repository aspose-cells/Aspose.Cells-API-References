---
title: "CustomDocumentPropertyCollection.AddLinkToContent"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método CustomDocumentPropertyCollection. Crea una nueva propiedad de documento personalizada que se vincula al contenido"
type: docs
url: /es/net/aspose.cells.properties/customdocumentpropertycollection/addlinktocontent/
---
## CustomDocumentPropertyCollection.AddLinkToContent method

Crea una nueva propiedad de documento personalizada que enlaza con contenido.

```csharp
public DocumentProperty AddLinkToContent(string name, string source)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | String | El nombre de la propiedad. |
| origen | String | El origen de la propiedad. Debe ser el nombre del rango nombrado. |

### Valor de retorno

El objeto de propiedad recién creado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class CustomDocumentPropertyCollectionMethodAddLinkToContentWithStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer un valor en la celda A1 que se vinculará
            worksheet.Cells["A1"].PutValue("Linked Cell Value");

            CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;
            
            // Agregar una propiedad regular para comparación
            customProperties.Add("RegularProperty", "Static Value");
            
            // Agregar una propiedad vinculada
            customProperties.AddLinkToContent("LinkedProperty", "Sheet1!A1");
            
            // Actualizar el valor vinculado
            customProperties.UpdateLinkedRange();

            // Mostrar las propiedades
            Console.WriteLine($"Regular Property: {customProperties["RegularProperty"].Value}");
            Console.WriteLine($"Linked Property: {customProperties["LinkedProperty"].Value}");

            workbook.Save("LinkedPropertyExample.xlsx");
        }
    }
}
```

### Ver también

* class [DocumentProperty](../../documentproperty/)
* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


