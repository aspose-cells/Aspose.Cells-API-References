---
title: "LoadOptions.StandardFont"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LoadOptions-Eigenschaft. Legt den Standard‑Schriftartnamen fest"
type: docs
url: /de/net/aspose.cells/loadoptions/standardfont/
---
## LoadOptions.StandardFont property

Legt den Standard‑Schriftartnamen fest

```csharp
[Obsolete("Use DefaultStyleSettings.FontName property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string StandardFont { get; set; }
```

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen DefaultStyleSettings. Diese Eigenschaft wird 12 Monate später, seit März 2022, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erlebt haben.

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyStandardFontDemo
    {
        public static void Run()
        {
            // Erstelle eine Beispiel-Excel-Datei im Speicher
            MemoryStream ms = new MemoryStream();
            using (Workbook workbook = new Workbook())
            {
                workbook.Worksheets[0].Cells["A1"].PutValue("Standard Font Test");
                workbook.Save(ms, SaveFormat.Xlsx);
            }
            ms.Position = 0;

            // Ladeoptionen mit StandardFont festlegen
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.StandardFont = "SimSun";
            
            // Arbeitsmappe mit der angegebenen Schriftart laden
            Workbook workbookWithFont = new Workbook(ms, loadOptions);
            
            // Demonstrieren, dass die Schriftart gesetzt ist, indem der Standardstil überprüft wird
            Console.WriteLine("Default font after loading: " + 
                workbookWithFont.DefaultStyle.Font.Name);
        }
    }
}
```

### Siehe auch

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


