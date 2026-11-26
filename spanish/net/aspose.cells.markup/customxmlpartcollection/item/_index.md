---
title: "CustomXmlPartCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CustomXmlPartCollection. Obtiene un elemento en el índice especificado"
type: docs
url: /es/net/aspose.cells.markup/customxmlpartcollection/item/
---
## CustomXmlPartCollection indexer

Obtiene un elemento en el índice especificado.

```csharp
public CustomXmlPart this[int index] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| índice | El índice. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class CustomXmlPartCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a CustomXmlPartCollection directamente desde el libro de trabajo
            CustomXmlPartCollection customXmlParts = workbook.CustomXmlParts;
            
            // Datos XML de ejemplo
            string xmlData = "<root><item>Test Data</item></root>";
            byte[] xmlBytes = System.Text.Encoding.UTF8.GetBytes(xmlData);
            
            // Agregar una parte XML personalizada
            int index = customXmlParts.Add(xmlBytes, null);
            
            // Acceder al elemento usando la propiedad Item
            CustomXmlPart part = customXmlParts[index];
            
            // Mostrar el ID de la parte XML personalizada
            Console.WriteLine("Custom XML Part ID: " + part.ID);
            
            // Obtener los datos XML de la parte
            string retrievedXml = System.Text.Encoding.UTF8.GetString(part.Data);
            Console.WriteLine("XML Content: " + retrievedXml);
            
            // Guarda el libro de trabajo
            workbook.Save("CustomXmlPartDemo.xlsx");
        }
    }
}
```

### Ver también

* class [CustomXmlPart](../../customxmlpart/)
* class [CustomXmlPartCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


