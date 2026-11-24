---
title: "FontConfigs.SetFontFolder"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FontConfigs-Methode. Legt den Schriftordner fest"
type: docs
url: /de/net/aspose.cells/fontconfigs/setfontfolder/
---
## FontConfigs.SetFontFolder method

Legt den Schriftartenordner fest

```csharp
public static void SetFontFolder(string fontFolder, bool recursive)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fontFolder | String | Der Ordner, der TrueType-Schriften enthält. |
| rekursiv | Boolean | Bestimmt, ob Unterordner gescannt werden sollen oder nicht. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontConfigsMethodSetFontFolderWithStringBooleanDemo
    {
        public static void Run()
        {
            // Initialisieren Sie ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge etwas Text zu Zelle A1 hinzu
            worksheet.Cells["A1"].PutValue("Sample Text with Custom Font");
            
            // Lege einen benutzerdefinierten Schriftordner fest und gib an, ob Unterordner einbezogen werden sollen
            FontConfigs.SetFontFolder("Fonts", true);
            
            // Wende einen Schriftstil an, der möglicherweise Schriften aus dem benutzerdefinierten Ordner verwendet
            Style style = worksheet.Cells["A1"].GetStyle();
            style.Font.Name = "CustomFont"; // Assuming "CustomFont" exists in the Fonts folder
            style.Font.Size = 14;
            worksheet.Cells["A1"].SetStyle(style);
            
            // Arbeitsmappe als PDF speichern
            workbook.Save("output.pdf", SaveFormat.Pdf);
        }
    }
}
```

### Siehe auch

* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


