---
title: "SmartTag.Uri"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SmartTag-Eigenschaft. Gibt die Namespace-URI des SmartTags zurück"
type: docs
url: /de/net/aspose.cells.markup/smarttag/uri/
---
## SmartTag.Uri property

Liest den Namespace‑URI des Smart‑Tags.

```csharp
public string Uri { get; }
```

### Beispiele

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

            // Zeigen Sie den Wert der Uri‑Eigenschaft an (Nur‑Lese‑Operation)
            Console.WriteLine("SmartTag Uri: " + smartTag.Uri);

            // Demonstrieren Sie weitere Eigenschaften
            Console.WriteLine("SmartTag Name: " + smartTag.Name);

            // Speichere die Arbeitsmappe
            workbook.Save("SmartTagUriDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [SmartTag](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


