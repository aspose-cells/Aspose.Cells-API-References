---
title: "FontSetting.FontSetting"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FontSetting Konstruktor."
type: docs
url: /de/net/aspose.cells/fontsetting/fontsetting/
---
## FontSetting constructor

```csharp
public FontSetting(int startIndex, int length, WorksheetCollection sheets)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startIndex | Int32 |  |
| Länge | Int32 |  |
| Blätter | WorksheetCollection |  |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontSettingMethodCtorWithInt32Int32WorksheetCollectionDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieltext zur Zelle hinzufügen
            worksheet.Cells["A1"].PutValue("Hello World");
            
            // Erstellen Sie eine Schriftarteinstellung für die ersten 5 Zeichen (0-4) in allen Arbeitsblättern
            FontSetting fontSetting = new FontSetting(0, 5, workbook.Worksheets);
            
            // Formatierung anwenden
            fontSetting.Font.Color = System.Drawing.Color.Red;
            fontSetting.Font.IsBold = true;
            fontSetting.Font.Size = 14;
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [WorksheetCollection](../../worksheetcollection/)
* class [FontSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


