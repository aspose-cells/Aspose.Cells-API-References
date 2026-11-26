---
title: "SmartTag.Uri"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SmartTag. Obtiene el URI del espacio de nombres de la etiqueta inteligente"
type: docs
url: /es/net/aspose.cells.markup/smarttag/uri/
---
## SmartTag.Uri property

Obtiene el URI del espacio de nombres de la etiqueta inteligente.

```csharp
public string Uri { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class SmartTagPropertyUriDemo
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

            // Muestra el valor de la propiedad Uri (operación de solo lectura)
            Console.WriteLine("SmartTag Uri: " + smartTag.Uri);

            // Demuestra otras propiedades
            Console.WriteLine("SmartTag Name: " + smartTag.Name);

            // Guarda el libro de trabajo
            workbook.Save("SmartTagUriDemo.xlsx");
        }
    }
}
```

### Ver también

* class [SmartTag](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


