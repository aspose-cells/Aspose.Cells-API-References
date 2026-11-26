---
title: "CustomXmlPart.Data"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CustomXmlPart. Obtiene o establece el contenido XML de esta parte de almacenamiento de datos XML personalizada"
type: docs
url: /es/net/aspose.cells.markup/customxmlpart/data/
---
## CustomXmlPart.Data property

Obtiene o establece el contenido XML de esta parte de almacenamiento de datos XML personalizada.

```csharp
public byte[] Data { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;
    using System.Text;

    public class CustomXmlPartPropertyDataDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            byte[] initialData = Encoding.UTF8.GetBytes("<root><data>Initial Value</data></root>");
            int xmlPartIndex = workbook.CustomXmlParts.Add(initialData, null);
            CustomXmlPart xmlPart = workbook.CustomXmlParts[xmlPartIndex];
            
            Console.WriteLine("Current Data value: " + Encoding.UTF8.GetString(xmlPart.Data));

            xmlPart.Data = Encoding.UTF8.GetBytes("<root><data>Modified Value</data></root>");

            workbook.CustomXmlParts.Add(xmlPart.Data, null);
            workbook.Save("CustomXmlPartDataDemo.xlsx");
        }
    }
}
```

### Ver también

* class [CustomXmlPart](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


