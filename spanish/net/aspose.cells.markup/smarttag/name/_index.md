---
title: "SmartTag.Name"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SmartTag. Obtiene el nombre del smart tag"
type: docs
url: /es/net/aspose.cells.markup/smarttag/name/
---
## SmartTag.Name property

Obtiene el nombre de la etiqueta inteligente.

```csharp
public string Name { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class SmartTagPropertyNameDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            sheet.Cells["A1"].PutValue("Aspose");
            sheet.Cells["A2"].PutValue("Cells");

            SmartTagSetting smartTagSetting = sheet.SmartTagSetting;
            int smartTagIndex = smartTagSetting.Add(0, 0);
            SmartTagCollection smartTags = smartTagSetting[smartTagIndex];

            smartTags.Add("http://docs.aspose.com", "docs");
            SmartTag smartTag = smartTags[0];
            smartTag.SetLink("http://www.aspose.com", "AsposeLink");

            SmartTagPropertyCollection properties = smartTag.Properties;
            properties.Add("Author", "Aspose");
            properties.Add("Description", "Aspose.Cells SmartTag");

            // Demostrar la propiedad Name (operación de solo lectura)
            Console.WriteLine("SmartTag Name: " + smartTag.Name);

            // Guarda el libro de trabajo
            workbook.Save("SmartTagNameDemo.xlsx");
        }
    }
}
```

### Ver también

* class [SmartTag](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


