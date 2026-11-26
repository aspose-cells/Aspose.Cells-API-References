---
title: "SmartTag.Deleted"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SmartTag. Indica si el smart tag está eliminado"
type: docs
url: /es/net/aspose.cells.markup/smarttag/deleted/
---
## SmartTag.Deleted property

Indica si la etiqueta inteligente está eliminada.

```csharp
public bool Deleted { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class SmartTagPropertyDeletedDemo
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

            Console.WriteLine("Initial Deleted value: " + smartTag.Deleted);

            // Establecer la propiedad Deleted a true
            smartTag.Deleted = true;
            Console.WriteLine("After setting Deleted: " + smartTag.Deleted);

            // Guarda el libro de trabajo
            workbook.Save("SmartTagDeletedDemo.xlsx");

        }
    }
}
```

### Ver también

* class [SmartTag](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


