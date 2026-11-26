---
title: "CustomXmlPartCollection.Add"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método CustomXmlPartCollection. Añade un elemento a la colección"
type: docs
url: /es/net/aspose.cells.markup/customxmlpartcollection/add/
---
## CustomXmlPartCollection.Add method

Agrega un elemento a la colección.

```csharp
public int Add(byte[] data, byte[] schemaData)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| datos | Byte[] | El contenido XML de esta parte de almacenamiento de datos XML personalizada. |
| schemaData | Byte[] | El conjunto de esquemas XML asociados con esta parte XML personalizada. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;
    using System.Text;

    public class CustomXmlPartCollectionMethodAddWithByteByteDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Obtener CustomXmlPartCollection directamente del libro de trabajo
            CustomXmlPartCollection customXmlParts = workbook.CustomXmlParts;
            
            // Preparar datos XML y esquema como matrices de bytes
            string xmlData = "<root><item>Test Data</item></root>";
            string schemaData = "<xs:schema xmlns:xs='http://www.w3.org/2001/XMLSchema'><xs:element name='root'><xs:complexType><xs:sequence><xs:element name='item' type='xs:string'/></xs:sequence></xs:complexType></xs:element></xs:schema>";
            
            byte[] xmlBytes = Encoding.UTF8.GetBytes(xmlData);
            byte[] schemaBytes = Encoding.UTF8.GetBytes(schemaData);

            try
            {
                // Llamar al método Add con parámetros de matriz de bytes
                int index = customXmlParts.Add(xmlBytes, schemaBytes);
                
                Console.WriteLine($"Custom XML part added successfully at index: {index}");
                
                // Guarda el libro de trabajo para demostrar el efecto
                workbook.Save("CustomXmlPartAddDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error adding custom XML part: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [CustomXmlPartCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


