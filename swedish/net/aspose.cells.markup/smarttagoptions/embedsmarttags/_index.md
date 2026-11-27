---
title: "SmartTagOptions.EmbedSmartTags"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SmartTagOptions-egenskap. Anger om smarttaggar sparas med arbetsboken"
type: docs
url: /sv/net/aspose.cells.markup/smarttagoptions/embedsmarttags/
---
## SmartTagOptions.EmbedSmartTags property

Anger om smarta taggar sparas med arbetsboken.

```csharp
public bool EmbedSmartTags { get; set; }
```

### Exempel

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
            // SmartTagOptions används nu korrekt om API:et kräver det, men tilldelning till workbook.Settings är inte giltig

            Console.WriteLine("after setting value: Current EmbedSmartTags value: " + smartTagOptions.EmbedSmartTags);

            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("New York");

            // Åtkomst till SmartTags via SmartTagSetting
            int index = worksheet.SmartTagSetting.Add(cell.Name);
            SmartTagCollection smartTagCollection = worksheet.SmartTagSetting[index];
            int tagIndex = smartTagCollection.Add("urn:schemas-microsoft-com:office:smarttags#place", "Place");
            SmartTag smartTag = smartTagCollection[tagIndex];
            smartTag.Properties.Add("State", "NY");
            // Använd egenskaper för att ange LinkedCell
            smartTag.Properties.Add("LinkedCell", cell.Name);

            workbook.Save("PropertyEmbedSmartTagsDemo.xlsx");
        }
    }
}
```

### Se även

* class [SmartTagOptions](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


