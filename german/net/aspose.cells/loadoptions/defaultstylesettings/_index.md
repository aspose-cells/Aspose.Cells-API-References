---
title: "LoadOptions.DefaultStyleSettings"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LoadOptions-Eigenschaft. Ruft die Standardeinstellungsstile ab, die zum Initialisieren der Stile der Arbeitsmappe verwendet werden."
type: docs
url: /de/net/aspose.cells/loadoptions/defaultstylesettings/
---
## LoadOptions.DefaultStyleSettings property

Liest die Standard‑Stil‑Einstellungen zum Initialisieren der Stile der Arbeitsmappe.

```csharp
public DefaultStyleSettings DefaultStyleSettings { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyDefaultStyleSettingsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Ladeoptionen mit Standardeinstellungsstilen festlegen
            LoadOptions loadOptions = new LoadOptions(LoadFormat.Xlsx);
            loadOptions.DefaultStyleSettings.VerticalAlignment = TextAlignmentType.Bottom;
            
            // Erstellen Sie ein Arbeitsblatt und holen Sie die Zellen
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Werte festlegen, um den Standardstil zu demonstrieren
            cells["A1"].PutValue("Default Style Applied");
            cells["A2"].PutValue("Should have bottom alignment");
            
            // Erstellen Sie eine Zelle mit benutzerdefiniertem Stil (im Gegensatz zum Standard)
            Cell customCell = cells["B1"];
            customCell.PutValue("Custom Style");
            Style customStyle = customCell.GetStyle();
            customStyle.VerticalAlignment = TextAlignmentType.Center;
            customCell.SetStyle(customStyle);
            
            // Speichere die Arbeitsmappe
            workbook.Save("DefaultStyleSettingsDemo.xlsx");
            
            // Überprüfen Sie die Stile
            Console.WriteLine("A1 Vertical Alignment: " + cells["A1"].GetStyle().VerticalAlignment);
            Console.WriteLine("B1 Vertical Alignment: " + cells["B1"].GetStyle().VerticalAlignment);
        }
    }
}
```

### Siehe auch

* class [DefaultStyleSettings](../../defaultstylesettings/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


