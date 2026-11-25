---
title: "SmartTag.Deleted"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SmartTag. Indica se il tag intelligente è eliminato"
type: docs
url: /it/net/aspose.cells.markup/smarttag/deleted/
---
## SmartTag.Deleted property

Indica se lo smart tag è stato eliminato.

```csharp
public bool Deleted { get; set; }
```

### Esempi

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

            // Imposta la proprietà Deleted su true
            smartTag.Deleted = true;
            Console.WriteLine("After setting Deleted: " + smartTag.Deleted);

            // Salva la cartella di lavoro
            workbook.Save("SmartTagDeletedDemo.xlsx");

        }
    }
}
```

### Vedi anche

* class [SmartTag](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


