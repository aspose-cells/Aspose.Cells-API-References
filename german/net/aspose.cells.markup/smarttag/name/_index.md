---
title: "SmartTag.Name"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SmartTag-Eigenschaft. Gibt den Namen des SmartTags zurück"
type: docs
url: /de/net/aspose.cells.markup/smarttag/name/
---
## SmartTag.Name property

Liest den Namen des Smart‑Tags.

```csharp
public string Name { get; }
```

### Beispiele

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

            // Demonstrieren Sie die Name‑Eigenschaft (Nur‑Lese‑Operation)
            Console.WriteLine("SmartTag Name: " + smartTag.Name);

            // Speichere die Arbeitsmappe
            workbook.Save("SmartTagNameDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [SmartTag](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


