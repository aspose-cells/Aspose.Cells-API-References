---
title: "Classe SmartTag"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Markup.SmartTag. Rappresenta uno smart tag"
type: docs
url: /it/net/aspose.cells.markup/smarttag/
---
## SmartTag class

Rappresenta uno smart tag.

```csharp
public class SmartTag
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Deleted](../../aspose.cells.markup/smarttag/deleted/) { get; set; } | Indica se lo smart tag è stato eliminato. |
| [Name](../../aspose.cells.markup/smarttag/name/) { get; } | Ottiene il nome dello smart tag. |
| [Properties](../../aspose.cells.markup/smarttag/properties/) { get; set; } | Ottiene e imposta le proprietà dello smart tag. |
| [Uri](../../aspose.cells.markup/smarttag/uri/) { get; } | Ottiene l'URI dello spazio dei nomi dello smart tag. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [SetLink](../../aspose.cells.markup/smarttag/setlink/)(string, string) | Modifica il nome e l'URI dello spazio dei nomi dello smart tag. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Markup;

namespace AsposeCellsExamples
{
    public class MarkupClassSmartTagDemo
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

            workbook.Save("SmartTagDemo.xlsx");
            Console.WriteLine("SmartTagDemo.xlsx created successfully.");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Markup](../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../)


