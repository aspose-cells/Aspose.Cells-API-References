---
title: "Klasse DefaultStyleSettings"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.DefaultStyleSettings-Klasse. Einstellungen für die Standardwerte der Stil‑Eigenschaften von Arbeitsmappen"
type: docs
url: /de/net/aspose.cells/defaultstylesettings/
---
## DefaultStyleSettings class

Einstellungen für die Standardwerte der Stil‑Eigenschaften des Arbeitsblatts.

```csharp
public class DefaultStyleSettings
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [BuiltInPreference](../../aspose.cells/defaultstylesettings/builtinpreference/) { get; set; } | Gibt an, ob die Eigenschaft für das Zahlenformat vorzuziehen ist, wenn der Stil sowohl integrierte Zahlen als auch ein benutzerdefiniertes Muster definiert. Der Standardwert ist false, das bedeutet, dass standardmäßig das benutzerdefinierte Muster verwendet wird, um Werte zu formatieren, solange es für einen Stil nicht leer ist. |
| [FontName](../../aspose.cells/defaultstylesettings/fontname/) { get; set; } | Liest/Setzt den Standard‑Schriftartnamen für die Arbeitsmappe |
| [FontSize](../../aspose.cells/defaultstylesettings/fontsize/) { get; set; } | Liest/Setzt die Standard‑Schriftgröße für die Arbeitsmappe. |
| [HorizontalAlignment](../../aspose.cells/defaultstylesettings/horizontalalignment/) { get; set; } | Liest/Setzt den Standardwert für die horizontale Ausrichtung |
| [VerticalAlignment](../../aspose.cells/defaultstylesettings/verticalalignment/) { get; set; } | Liest/Setzt den Standardwert für die vertikale Ausrichtung |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DefaultStyleSettingsDemo
    {
        public static void DefaultStyleSettingsExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf die Standard-Style-Einstellungen der Arbeitsmappe
            DefaultStyleSettings defaultStyleSettings = workbook.Settings.DefaultStyleSettings;

            // Eigenschaften festlegen
            defaultStyleSettings.BuiltInPreference = false;
            defaultStyleSettings.FontName = "Arial";
            defaultStyleSettings.FontSize = 12.0;
            defaultStyleSettings.HorizontalAlignment = TextAlignmentType.Center;
            defaultStyleSettings.VerticalAlignment = TextAlignmentType.Center;

            // Wenden Sie die Standard-Style-Einstellungen auf das erste Arbeitsblatt an
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells.ApplyStyle(workbook.CreateStyle(), new StyleFlag() { All = true });

            // Speichere die Arbeitsmappe
            workbook.Save("DefaultStyleSettingsExample.xlsx");
            workbook.Save("DefaultStyleSettingsExample.pdf");

            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


