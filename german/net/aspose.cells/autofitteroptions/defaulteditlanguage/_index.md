---
title: "AutoFitterOptions.DefaultEditLanguage"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "AutoFitterOptions-Eigenschaft. Gibt die Standardsprache für die Bearbeitung zurück oder legt sie fest"
type: docs
url: /de/net/aspose.cells/autofitteroptions/defaulteditlanguage/
---
## AutoFitterOptions.DefaultEditLanguage property

Liest oder setzt die Standardsprache für die Bearbeitung.

```csharp
public DefaultEditLanguage DefaultEditLanguage { get; set; }
```

### Hinweise

Es kann unterschiedliche Layouts für Textabsätze anzeigen/rendern, wenn verschiedene Bearbeitungssprachen festgelegt sind. Standard ist Auto.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFitterOptionsPropertyDefaultEditLanguageDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispiel-CJK-Text in einer Zelle festlegen
            worksheet.Cells["A1"].PutValue("日本語のテキスト");

            AutoFitterOptions options = new AutoFitterOptions();
            options.DefaultEditLanguage = DefaultEditLanguage.CJK;

            // Zeile automatisch anpassen mit CJK-Sprachoptionen
            worksheet.AutoFitRows(options);

            Console.WriteLine("Auto-fit completed with DefaultEditLanguage: " + options.DefaultEditLanguage);
            workbook.Save("DefaultEditLanguageDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [DefaultEditLanguage](../../defaulteditlanguage/)
* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


