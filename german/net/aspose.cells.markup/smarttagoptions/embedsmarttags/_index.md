---
title: "SmartTagOptions.EmbedSmartTags"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SmartTagOptions-Eigenschaft. Gibt an, ob Smart-Tags mit der Arbeitsmappe gespeichert werden"
type: docs
url: /de/net/aspose.cells.markup/smarttagoptions/embedsmarttags/
---
## SmartTagOptions.EmbedSmartTags property

Gibt an, ob SmartTags mit der Arbeitsmappe gespeichert werden.

```csharp
public bool EmbedSmartTags { get; set; }
```

### Beispiele

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
            // Die SmartTagOptions werden nun korrekt verwendet, falls von der API verlangt, obwohl die Zuweisung zu workbook.Settings nicht gültig ist

            Console.WriteLine("after setting value: Current EmbedSmartTags value: " + smartTagOptions.EmbedSmartTags);

            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("New York");

            // Greife auf SmartTags über SmartTagSetting zu
            int index = worksheet.SmartTagSetting.Add(cell.Name);
            SmartTagCollection smartTagCollection = worksheet.SmartTagSetting[index];
            int tagIndex = smartTagCollection.Add("urn:schemas-microsoft-com:office:smarttags#place", "Place");
            SmartTag smartTag = smartTagCollection[tagIndex];
            smartTag.Properties.Add("State", "NY");
            // Verwende Properties, um LinkedCell festzulegen
            smartTag.Properties.Add("LinkedCell", cell.Name);

            workbook.Save("PropertyEmbedSmartTagsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [SmartTagOptions](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


