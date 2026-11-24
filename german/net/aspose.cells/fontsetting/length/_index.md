---
title: "FontSetting.Length"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FontSetting-Eigenschaft. Gibt die Länge der Zeichen zurück"
type: docs
url: /de/net/aspose.cells/fontsetting/length/
---
## FontSetting.Length property

Ermittelt die Länge der Zeichen.

```csharp
public int Length { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontSettingPropertyLengthDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe und greifen Sie auf das erste Arbeitsblatt zu
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge etwas Text zu Zelle A1 hinzu
            worksheet.Cells["A1"].PutValue("Hello World");

            // Erstellen Sie Schriftarteinstellungen für den Text in Zelle A1
            FontSetting fontSetting = worksheet.Cells["A1"].Characters(0, 5);
            
            // Demonstrieren Sie die Verwendung der Length-Eigenschaft
            Console.WriteLine("Original Length: " + fontSetting.Length);
            
            // Ändern Sie die Länge der Schriftarteinstellung
            fontSetting = worksheet.Cells["A1"].Characters(0, 11);
            Console.WriteLine("Modified Length: " + fontSetting.Length);
            
            // Wenden Sie Formatierungen auf die Schriftarteinstellung an
            fontSetting.Font.Color = System.Drawing.Color.Red;
            fontSetting.Font.IsBold = true;
            
            // Speichere die Arbeitsmappe
            workbook.Save("FontSettingLengthDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [FontSetting](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


