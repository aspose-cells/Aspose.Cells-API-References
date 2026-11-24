---
title: "Klasse SheetSet"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Rendering.SheetSet Klasse. Beschreibt eine Menge von Tabellenblättern"
type: docs
url: /de/net/aspose.cells.rendering/sheetset/
---
## SheetSet class

Beschreibt eine Menge von Arbeitsblättern.

```csharp
public class SheetSet
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [SheetSet](sheetset/#constructor)(params int[]) | Erstellt ein Blattset basierend auf genauen Blattindizes. |
| [SheetSet](sheetset/#constructor_1)(params string[]) | Erstellt ein Blattset basierend auf genauen Blattnamen. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| static [Active](../../aspose.cells.rendering/sheetset/active/) { get; } | Erhält ein Set mit dem aktiven Blatt der Arbeitsmappe. |
| static [All](../../aspose.cells.rendering/sheetset/all/) { get; } | Erhält ein Set mit allen Blättern der Arbeitsmappe in ihrer ursprünglichen Reihenfolge. |
| static [Visible](../../aspose.cells.rendering/sheetset/visible/) { get; } | Erhält ein Set mit sichtbaren Blättern der Arbeitsmappe in ihrer ursprünglichen Reihenfolge. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class SheetSetDemo
    {
        public static void SheetSetExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge dem Arbeitsblatt einige Daten hinzu
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["A3"].PutValue(456);   

            worksheet = workbook.Worksheets.Add("test1");
            worksheet.Cells["A1"].PutValue("test Data");
            worksheet.Cells["A2"].PutValue(234);
            worksheet.Cells["A3"].PutValue(333);
            worksheet.IsVisible = false;

            worksheet = workbook.Worksheets.Add("test2");
            worksheet.Cells["A1"].PutValue("test Data222");
            worksheet.Cells["A2"].PutValue(234444);
            worksheet.Cells["A3"].PutValue(333555);

            workbook.Worksheets.ActiveSheetIndex = 0;

            // Erstelle ein PdfSaveOptions-Objekt
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();

            // Setze die SheetSet-Eigenschaft, um nur das aktive Blatt einzuschließen
            pdfSaveOptions.SheetSet = SheetSet.Active;

            // Speichere die Arbeitsmappe in einer PDF-Datei
            workbook.Save("SheetSetExample_ActiveSheet.pdf", pdfSaveOptions);

            // Setze die SheetSet-Eigenschaft, um alle sichtbaren Blätter einzuschließen
            pdfSaveOptions.SheetSet = SheetSet.Visible;

            // Speichere die Arbeitsmappe in einer PDF-Datei
            workbook.Save("SheetSetExample_VisibleSheets.pdf", pdfSaveOptions);

            // Setze die SheetSet-Eigenschaft, um alle Blätter einzuschließen
            pdfSaveOptions.SheetSet = SheetSet.All;

            // Speichere die Arbeitsmappe in einer PDF-Datei
            workbook.Save("SheetSetExample_AllSheets.pdf", pdfSaveOptions);

            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


