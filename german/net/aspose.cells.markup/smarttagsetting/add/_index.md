---
title: "SmartTagSetting.Add"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SmartTagSetting-Methode. Fügt ein SmartTagCollection‑Objekt zu einer Zelle hinzu"
type: docs
url: /de/net/aspose.cells.markup/smarttagsetting/add/
---
## Add(int, int) {#add}

Fügt ein [`SmartTagCollection`](../../smarttagcollection/)‑Objekt zu einer Zelle hinzu.

```csharp
public int Add(int row, int column)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| row | Int32 | Die Zeile der Zelle. |
| column | Int32 | Die Spalte der Zelle. |

### Rückgabewert

Gibt den Index eines [`SmartTagCollection`](../../smarttagcollection/)‑Objekts im Arbeitsblatt zurück.

### Beispiele

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

### Siehe auch

* class [SmartTagSetting](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)

---

## Add(string) {#add_1}

Füge ein Zellen‑SmartTag hinzu.

```csharp
public int Add(string cellName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cellName | String | Der Name der Zelle. |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Rufen Sie die SmartTagSetting‑Instanz ab
            SmartTagSetting smartTagSetting = worksheet.SmartTagSetting;
            
            try
            {
                // Rufen Sie die Add‑Methode mit einem String‑Parameter auf
                int index = smartTagSetting.Add("A1");
                
                Console.WriteLine($"SmartTag added successfully at index: {index}");
                
                // Fügen Sie Inhalte hinzu, um die Wirkung zu demonstrieren
                worksheet.Cells["A1"].PutValue("This cell has a smart tag");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Ergebnis speichern
            workbook.Save("SmartTagSettingMethodAddWithStringDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [SmartTagSetting](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


