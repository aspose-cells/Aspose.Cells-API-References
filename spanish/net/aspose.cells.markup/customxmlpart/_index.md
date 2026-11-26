---
title: "Clase CustomXmlPart"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Markup.CustomXmlPart. Representa una parte de almacenamiento de datos XML personalizada (Custom XML Data Storage Part) dentro de un paquete"
type: docs
url: /es/net/aspose.cells.markup/customxmlpart/
---
## CustomXmlPart class

Representa una parte de almacenamiento de datos XML personalizada (datos XML personalizados dentro de un paquete).

```csharp
public class CustomXmlPart
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Data](../../aspose.cells.markup/customxmlpart/data/) { get; set; } | Obtiene o establece el contenido XML de esta parte de almacenamiento de datos XML personalizada. |
| [ID](../../aspose.cells.markup/customxmlpart/id/) { get; set; } | Obtiene y establece el id de la parte XML personalizada. |
| [SchemaData](../../aspose.cells.markup/customxmlpart/schemadata/) { get; set; } | Obtiene o establece el contenido XML de esta parte de almacenamiento de datos de esquema XML personalizada. |

### Ejemplos

```csharp
using System;
using System.Text;
using Aspose.Cells;
using Aspose.Cells.Markup;

namespace AsposeCellsExamples
{
    public class MarkupClassCustomXmlPartDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            CustomXmlPartCollection xmlParts = workbook.CustomXmlParts;

            string xmlData = "<root><item>Sample Data</item></root>";
            byte[] dataBytes = Encoding.UTF8.GetBytes(xmlData);

            string originalId = Guid.NewGuid().ToString();
            int index = xmlParts.Add(dataBytes, null);
            CustomXmlPart newPart = xmlParts[index];
            newPart.ID = originalId;

            Console.WriteLine("Original ID: " + originalId);
            Console.WriteLine("Stored ID: " + newPart.ID);

            string newId = Guid.NewGuid().ToString();
            newPart.ID = newId;
            Console.WriteLine("Updated ID: " + newId);

            workbook.Save("output.xlsx");

            Workbook loadedWorkbook = new Workbook("output.xlsx");
            CustomXmlPart retrievedPart = loadedWorkbook.CustomXmlParts.SelectByID(newId);
            Console.WriteLine("Retrieved ID: " + (retrievedPart != null ? retrievedPart.ID : "Not found"));
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Markup](../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../)


