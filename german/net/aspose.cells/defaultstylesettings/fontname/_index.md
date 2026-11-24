---
title: "DefaultStyleSettings.FontName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DefaultStyleSettings-Eigenschaft. Gibt/Setzt den Standard‑Schriftartnamen für die Arbeitsmappe"
type: docs
url: /de/net/aspose.cells/defaultstylesettings/fontname/
---
## DefaultStyleSettings.FontName property

Liest/Setzt den Standard‑Schriftartnamen für die Arbeitsmappe

```csharp
public string FontName { get; set; }
```

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DefaultStyleSettingsPropertyFontNameDemo
    {
        public static void Run()
        {
            // Ladeoptionen erstellen und Schriftartnamen festlegen
            LoadOptions loadOptions = new LoadOptions(LoadFormat.Xlsx);
            loadOptions.DefaultStyleSettings.FontName = "SimSun";

            // Ein neues Arbeitsbuch mit den Ladeoptionen erstellen
            Workbook workbook = new Workbook();
            workbook.DefaultStyle.Font.Name = loadOptions.DefaultStyleSettings.FontName;

            // Auf den Standardstil zugreifen und den Schriftartnamen überprüfen
            Style defaultStyle = workbook.DefaultStyle;
            Console.WriteLine("Default Font Name: " + defaultStyle.Font.Name);

            // Ein Arbeitsblatt erstellen und Zellenwert festlegen
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Font Name Test");

            // Speichere die Arbeitsmappe
            using (MemoryStream stream = new MemoryStream())
            {
                workbook.Save(stream, SaveFormat.Xlsx);
                Console.WriteLine("Workbook saved with default font: SimSun");
            }
        }
    }
}
```

### Siehe auch

* class [DefaultStyleSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


