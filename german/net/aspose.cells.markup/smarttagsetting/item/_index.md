---
title: "SmartTagSetting.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SmartTagSetting-Eigenschaft. Gibt ein SmartTagCollection‑Objekt anhand des Index zurück"
type: docs
url: /de/net/aspose.cells.markup/smarttagsetting/item/
---
## SmartTagSetting indexer (1 of 3)

Gibt ein [`SmartTagCollection`](../../smarttagcollection/)‑Objekt anhand des Index zurück.

```csharp
public SmartTagCollection this[int index] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| index | Der Index des [`SmartTagCollection`](../../smarttagcollection/)‑Objekts in der Liste. |

### Beispiele

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
            
            // Demonstriere die Verwendung der Item-Eigenschaft
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

### Siehe auch

* class [SmartTagCollection](../../smarttagcollection/)
* class [SmartTagSetting](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)

---

## SmartTagSetting indexer (2 of 3)

Ruft das [`SmartTagCollection`](../../smarttagcollection/) Objekt der Zelle ab.

```csharp
public SmartTagCollection this[int row, int column] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| row | Der Zeilenindex der Zelle. |
| column | Der Spaltenindex der Zelle |

### Rückgabewert

Gibt das [`SmartTagCollection`](../../smarttagcollection/) Objekt der Zelle zurück. Gibt null zurück, wenn keine SmartTags in der Zelle vorhanden sind.

### Beispiele

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

            // Demonstriere die Verwendung der Item-Eigenschaft
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

### Siehe auch

* class [SmartTagCollection](../../smarttagcollection/)
* class [SmartTagSetting](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)

---

## SmartTagSetting indexer (3 of 3)

Ruft das [`SmartTagCollection`](../../smarttagcollection/) Objekt der Zelle ab.

```csharp
public SmartTagCollection this[string cellName] { get; }
```

| Parameter | Beschreibung |
| --- | --- |
| cellName | Der Name der Zelle. |

### Rückgabewert

Gibt das [`SmartTagCollection`](../../smarttagcollection/) Objekt der Zelle zurück. Gibt null zurück, wenn keine SmartTags in der Zelle vorhanden sind.

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Hole das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Greift auf die SmartTagSetting für das Arbeitsblatt zu
                SmartTagSetting smartTagSetting = worksheet.SmartTagSetting;

                // Füge einen SmartTag zur Zelle A1 (Zeile 0, Spalte 0) hinzu
                int smartTagIndex = smartTagSetting.Add(0, 0);

                // Demonstriere die Verwendung der Item-Eigenschaft (Indexer)
                SmartTagCollection smartTagCollection = smartTagSetting[smartTagIndex];

                // Füge der Sammlung ein SmartTag hinzu
                smartTagCollection.Add("urn:schemas-microsoft-com:office:smarttags", "date");

                // Zeige Informationen über den SmartTag an
                Console.WriteLine("Number of smart tags in collection: " + smartTagCollection.Count);
                if (smartTagCollection.Count > 0)
                {
                    Console.WriteLine("First smart tag URI: " + smartTagCollection[0].Uri);
                    Console.WriteLine("First smart tag name: " + smartTagCollection[0].Name);
                }

                // Speichere die Arbeitsmappe
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

### Siehe auch

* class [SmartTagCollection](../../smarttagcollection/)
* class [SmartTagSetting](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


