---
title: "HtmlSaveOptions.ExportHiddenWorksheet"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HtmlSaveOptions Eigenschaft. Gibt an, ob der Inhalt des ausgeblendeten Arbeitsblatts exportiert wird. Der Standardwert ist true."
type: docs
url: /de/net/aspose.cells/htmlsaveoptions/exporthiddenworksheet/
---
## HtmlSaveOptions.ExportHiddenWorksheet property

Gibt an, ob versteckte Worksheet‑Inhalte exportiert werden. Der Standardwert ist true.

```csharp
public bool ExportHiddenWorksheet { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportHiddenWorksheetDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet1 = workbook.Worksheets[0];
            worksheet1.Name = "VisibleSheet";
            worksheet1.Cells["A1"].PutValue("Visible Data");

            Worksheet worksheet2 = workbook.Worksheets.Add("HiddenSheet");
            worksheet2.Cells["A1"].PutValue("Hidden Data");
            worksheet2.IsVisible = false;

            // HTML-Speicheroptionen festlegen
            HtmlSaveOptions saveOptions = new HtmlSaveOptions
            {
                ExportHiddenWorksheet = false, // Don't export hidden worksheets
                ExportActiveWorksheetOnly = false
            };

            // Speichern, wobei das ausgeblendete Arbeitsblatt nicht exportiert wird
            workbook.Save("output_without_hidden.html", saveOptions);

            // Option ändern, um ausgeblendete Arbeitsblätter zu exportieren
            saveOptions.ExportHiddenWorksheet = true;

            // Speichern, wobei das ausgeblendete Arbeitsblatt exportiert wird
            workbook.Save("output_with_hidden.html", saveOptions);
        }
    }
}
```

### Siehe auch

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


