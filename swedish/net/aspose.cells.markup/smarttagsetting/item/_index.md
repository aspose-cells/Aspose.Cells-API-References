---
title: "SmartTagSetting.Item"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SmartTagSetting-egenskap. Hämtar ett SmartTagCollection-objekt via indexet"
type: docs
url: /sv/net/aspose.cells.markup/smarttagsetting/item/
---
## SmartTagSetting indexer (1 of 3)

Hämtar ett [`SmartTagCollection`](../../smarttagcollection/) objekt via indexet.

```csharp
public SmartTagCollection this[int index] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| index | Indexet för [`SmartTagCollection`](../../smarttagcollection/) objektet i listan. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Markup;

namespace AsposeCellsExamples
{
    public class SmartTagSettingPropertyItemDemo1
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            sheet.Cells["A1"].PutValue("Aspose");
            sheet.Cells["A2"].PutValue("Cells");

            SmartTagSetting smartTagSetting = sheet.SmartTagSetting;
            int smartTagIndex = smartTagSetting.Add(0, 0);
            
            // Demonstrera användning av Item-egenskapen
            SmartTagCollection smartTags = smartTagSetting[smartTagIndex];
            smartTags.Add("http://docs.aspose.com", "docs");
            
            SmartTag smartTag = smartTags[0];
            smartTag.SetLink("http://www.aspose.com", "AsposeLink");

            SmartTagPropertyCollection properties = smartTag.Properties;
            properties.Add("Author", "Aspose");
            properties.Add("Version", "1.0");

            workbook.Save("SmartTagPropertyDemo.xlsx");
            Console.WriteLine("SmartTagPropertyDemo.xlsx created successfully.");
        }
    }
}
```

### Se även

* class [SmartTagCollection](../../smarttagcollection/)
* class [SmartTagSetting](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)

---

## SmartTagSetting indexer (2 of 3)

Hämtar [`SmartTagCollection`](../../smarttagcollection/) objektet för cellen.

```csharp
public SmartTagCollection this[int row, int column] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| row | Radindex för cellen. |
| column | Kolumnindexet för cellen |

### Returvärde

Returnerar [`SmartTagCollection`](../../smarttagcollection/) objektet för cellen. Returnerar null om det inte finns några smarta taggar i cellen.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Markup;

namespace AsposeCellsExamples
{
    public class SmartTagSettingPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            SmartTagSetting smartTagSetting = worksheet.SmartTagSetting;
            smartTagSetting.Add(0, 0); // Add smart tag to cell A1

            // Demonstrera användning av Item-egenskapen
            SmartTagCollection smartTagCollection = smartTagSetting[0, 0];
            smartTagCollection.Add("urn:schemas-microsoft-com:office:smarttags", "date");

            Console.WriteLine("Smart tags in cell A1: " + smartTagCollection.Count);
            Console.WriteLine("Namespace URI: " + smartTagCollection[0].Uri);
            Console.WriteLine("Tag name: " + smartTagCollection[0].Name);

            workbook.Save("SmartTagDemo.xlsx");
        }
    }
}
```

### Se även

* class [SmartTagCollection](../../smarttagcollection/)
* class [SmartTagSetting](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)

---

## SmartTagSetting indexer (3 of 3)

Hämtar [`SmartTagCollection`](../../smarttagcollection/) objektet för cellen.

```csharp
public SmartTagCollection this[string cellName] { get; }
```

| Parameter | Beskrivning |
| --- | --- |
| cellName | Namnet på cellen. |

### Returvärde

Returnerar [`SmartTagCollection`](../../smarttagcollection/) objektet för cellen. Returnerar null om det inte finns några smarta taggar i cellen.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class SmartTagSettingPropertyItemDemo2
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Hämta det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Åtkomst till SmartTagSetting för arbetsbladet
                SmartTagSetting smartTagSetting = worksheet.SmartTagSetting;

                // Lägg till en smart tag i cell A1 (rad 0, kolumn 0)
                int smartTagIndex = smartTagSetting.Add(0, 0);

                // Demonstrera användning av Item-egenskapen (indexerare)
                SmartTagCollection smartTagCollection = smartTagSetting[smartTagIndex];

                // Lägg till en smart tagg i samlingen
                smartTagCollection.Add("urn:schemas-microsoft-com:office:smarttags", "date");

                // Visa information om smart tag
                Console.WriteLine("Number of smart tags in collection: " + smartTagCollection.Count);
                if (smartTagCollection.Count > 0)
                {
                    Console.WriteLine("First smart tag URI: " + smartTagCollection[0].Uri);
                    Console.WriteLine("First smart tag name: " + smartTagCollection[0].Name);
                }

                // Spara arbetsboken
                workbook.Save("SmartTagItemDemo.xlsx");
                Console.WriteLine("SmartTagItemDemo.xlsx created successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [SmartTagCollection](../../smarttagcollection/)
* class [SmartTagSetting](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


