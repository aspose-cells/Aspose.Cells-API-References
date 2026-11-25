---
title: "SmartTag.Properties"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SmartTag. Ottiene e imposta le proprietà del tag intelligente"
type: docs
url: /it/net/aspose.cells.markup/smarttag/properties/
---
## SmartTag.Properties property

Ottiene e imposta le proprietà dello smart tag.

```csharp
public SmartTagPropertyCollection Properties { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Markup;

namespace AsposeCellsExamples
{
    public class SmartTagPropertyPropertiesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            SmartTagSetting smartTagSetting = sheet.SmartTagSetting;
            int smartTagIndex = smartTagSetting.Add(0, 0);
            SmartTagCollection smartTags = smartTagSetting[smartTagIndex];

            smartTags.Add("http://docs.aspose.com", "docs");
            SmartTag smartTag = smartTags[0];

            SmartTagPropertyCollection properties = smartTag.Properties;
            properties.Add("Author", "John Doe");
            properties.Add("Version", "1.0");
            properties.Add("Category", "Demo");

            Console.WriteLine("Smart Tag Properties:");
            foreach (SmartTagProperty prop in properties)
            {
                Console.WriteLine($"{prop.Name}: {prop.Value}");
            }

            workbook.Save("SmartTagPropertiesDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [SmartTagPropertyCollection](../../smarttagpropertycollection/)
* class [SmartTag](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


