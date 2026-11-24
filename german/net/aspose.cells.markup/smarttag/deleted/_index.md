---
title: "SmartTag.Deleted"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SmartTag‑Eigenschaft. Gibt an, ob das Smart‑Tag gelöscht ist"
type: docs
url: /de/net/aspose.cells.markup/smarttag/deleted/
---
## SmartTag.Deleted property

Gibt an, ob das Smart‑Tag gelöscht ist.

```csharp
public bool Deleted { get; set; }
```

### Beispiele

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

            // Setzen Sie die Deleted-Eigenschaft auf true
            smartTag.Deleted = true;
            Console.WriteLine("After setting Deleted: " + smartTag.Deleted);

            // Speichere die Arbeitsmappe
            workbook.Save("SmartTagDeletedDemo.xlsx");

        }
    }
}
```

### Siehe auch

* class [SmartTag](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


