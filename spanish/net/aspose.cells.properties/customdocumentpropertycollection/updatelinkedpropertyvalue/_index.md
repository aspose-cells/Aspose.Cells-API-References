---
title: "CustomDocumentPropertyCollection.UpdateLinkedPropertyValue"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método CustomDocumentPropertyCollection. Actualiza los valores de todas las propiedades personalizadas que están vinculadas al contenido usando el valor de celda del rango vinculado para actualizar el valor de la propiedad personalizada"
type: docs
url: /es/net/aspose.cells.properties/customdocumentpropertycollection/updatelinkedpropertyvalue/
---
## CustomDocumentPropertyCollection.UpdateLinkedPropertyValue method

Actualiza los valores de todas las propiedades personalizadas que están vinculadas al contenido (utiliza el valor de celda del rango vinculado para actualizar el valor de la propiedad personalizada).

```csharp
public void UpdateLinkedPropertyValue()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CustomDocumentPropertyCollectionMethodUpdateLinkedPropertyValueDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar algunos datos a las celdas que se vincularán a las propiedades personalizadas
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "InitialValue1";
            worksheet.Cells["B1"].Value = "InitialValue2";

            // Agregar propiedades personalizadas vinculadas
            workbook.CustomDocumentProperties.AddLinkToContent("CompanyName", "A1");
            workbook.CustomDocumentProperties.AddLinkToContent("Department", "B1");

            // Actualizar los valores de las celdas
            worksheet.Cells["A1"].Value = "UpdatedValue1";
            worksheet.Cells["B1"].Value = "UpdatedValue2";

            // Actualizar los valores de las propiedades vinculadas
            workbook.CustomDocumentProperties.UpdateLinkedPropertyValue();

            // Mostrar los valores de las propiedades actualizadas
            Console.WriteLine("CompanyName: " + workbook.CustomDocumentProperties["CompanyName"].Value);
            Console.WriteLine("Department: " + workbook.CustomDocumentProperties["Department"].Value);

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [CustomDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


