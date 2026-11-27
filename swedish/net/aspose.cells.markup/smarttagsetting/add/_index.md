---
title: "SmartTagSetting.Add"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SmartTagSetting-metod. Lägger till ett SmartTagCollection-objekt i en cell"
type: docs
url: /sv/net/aspose.cells.markup/smarttagsetting/add/
---
## Add(int, int) {#add}

Lägger till ett [`SmartTagCollection`](../../smarttagcollection/) objekt i en cell.

```csharp
public int Add(int row, int column)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| row | Int32 | Raden i cellen. |
| column | Int32 | Kolumnen i cellen. |

### Returvärde

Returnerar index för ett [`SmartTagCollection`](../../smarttagcollection/) objekt i kalkylbladet.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Markup;

namespace AsposeCellsExamples
{
    public class SmartTagSettingMethodAddWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            SmartTagSetting smartTagSetting = worksheet.SmartTagSetting;
            int smartTagIndex = smartTagSetting.Add(0, 0); // Add to cell A1 (row 0, column 0)

            SmartTagCollection smartTagCollection = smartTagSetting[0, 0];
            smartTagCollection.Add("urn:schemas-microsoft-com:office:smarttags", "date");

            Console.WriteLine("Smart Tags Count: " + smartTagSetting.Count.ToString());
            workbook.Save("SmartTagDemo.xlsx");
        }
    }
}
```

### Se även

* class [SmartTagSetting](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)

---

## Add(string) {#add_1}

Lägg till en smart tagg i cellen.

```csharp
public int Add(string cellName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cellName | String | Namnet på cellen. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class SmartTagSettingMethodAddWithStringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hämta SmartTagSetting-instansen
            SmartTagSetting smartTagSetting = worksheet.SmartTagSetting;
            
            try
            {
                // Anropa Add-metoden med String-parameter
                int index = smartTagSetting.Add("A1");
                
                Console.WriteLine($"SmartTag added successfully at index: {index}");
                
                // Lägg till lite innehåll för att demonstrera effekten
                worksheet.Cells["A1"].PutValue("This cell has a smart tag");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Spara resultatet
            workbook.Save("SmartTagSettingMethodAddWithStringDemo.xlsx");
        }
    }
}
```

### Se även

* class [SmartTagSetting](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


