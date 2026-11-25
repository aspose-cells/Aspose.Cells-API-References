---
title: "SmartTag.Uri"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SmartTag. Ottiene l'URI dello spazio dei nomi del tag intelligente"
type: docs
url: /it/net/aspose.cells.markup/smarttag/uri/
---
## SmartTag.Uri property

Ottiene l'URI dello spazio dei nomi dello smart tag.

```csharp
public string Uri { get; }
```

### Esempi

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

            // Visualizza il valore della proprietà Uri (operazione di sola lettura)
            Console.WriteLine("SmartTag Uri: " + smartTag.Uri);

            // Dimostra altre proprietà
            Console.WriteLine("SmartTag Name: " + smartTag.Name);

            // Salva la cartella di lavoro
            workbook.Save("SmartTagUriDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [SmartTag](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


