---
title: "SmartTagOptions.EmbedSmartTags"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SmartTagOptions. Indica si se guardan las etiquetas inteligentes con el libro de trabajo"
type: docs
url: /es/net/aspose.cells.markup/smarttagoptions/embedsmarttags/
---
## SmartTagOptions.EmbedSmartTags property

Indica si se guardan las smart tags con el libro de trabajo.

```csharp
public bool EmbedSmartTags { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class SmartTagOptionsPropertyEmbedSmartTagsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            SmartTagOptions smartTagOptions = new SmartTagOptions();
            Console.WriteLine("Current EmbedSmartTags value: " + smartTagOptions.EmbedSmartTags);

            smartTagOptions.EmbedSmartTags = true;
            // El SmartTagOptions ahora se usa correctamente si lo requiere la API, aunque la asignación a workbook.Settings no es válida

            Console.WriteLine("after setting value: Current EmbedSmartTags value: " + smartTagOptions.EmbedSmartTags);

            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("New York");

            // Accede a SmartTags a través de SmartTagSetting
            int index = worksheet.SmartTagSetting.Add(cell.Name);
            SmartTagCollection smartTagCollection = worksheet.SmartTagSetting[index];
            int tagIndex = smartTagCollection.Add("urn:schemas-microsoft-com:office:smarttags#place", "Place");
            SmartTag smartTag = smartTagCollection[tagIndex];
            smartTag.Properties.Add("State", "NY");
            // Usa Properties para establecer LinkedCell
            smartTag.Properties.Add("LinkedCell", cell.Name);

            workbook.Save("PropertyEmbedSmartTagsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [SmartTagOptions](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


