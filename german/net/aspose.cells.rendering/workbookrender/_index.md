---
title: "Klasse WorkbookRender"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Rendering.WorkbookRender class. Stellt eine Arbeitsmappen-Darstellung dar. Der Konstruktor dieser Klasse muss nach der Änderung des Seitenlayouts‑Zellstils verwendet werden."
type: docs
url: /de/net/aspose.cells.rendering/workbookrender/
---
## WorkbookRender class

Stellt ein Arbeitsmappen‑Rendern dar. Der Konstruktor dieser Klasse muss nach der Änderung von pagesetup und cell style verwendet werden.

```csharp
public class WorkbookRender
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [WorkbookRender](workbookrender/)(Workbook, ImageOrPrintOptions) | Der Aufbau von WorkbookRender |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [PageCount](../../aspose.cells.rendering/workbookrender/pagecount/) { get; } | Ermittelt die Gesamtseitenzahl der Arbeitsmappe. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [CustomPrint](../../aspose.cells.rendering/workbookrender/customprint/)(bool, PrintPageEventArgs) | Der Client kann die Seiteneinstellungen des Druckers steuern, wenn jede Seite mit dieser Funktion gedruckt wird. |
| [Dispose](../../aspose.cells.rendering/workbookrender/dispose/)() | Gibt Ressourcen frei, die für das Rendern erstellt und verwendet wurden. |
| [GetPageSizeInch](../../aspose.cells.rendering/workbookrender/getpagesizeinch/)(int) | Ermittelt die Seitengröße in Zoll des Ausgabebildes. |
| [ToImage](../../aspose.cells.rendering/workbookrender/toimage/#toimage)(int) | Rendert eine bestimmte Seite in ein Bitmap-Objekt. |
| [ToImage](../../aspose.cells.rendering/workbookrender/toimage/#toimage_3)(Stream) | Rendert die gesamte Arbeitsmappe als TIFF-Bild in einen Stream. |
| [ToImage](../../aspose.cells.rendering/workbookrender/toimage/#toimage_4)(string) | Rendert die gesamte Arbeitsmappe als TIFF-Bild in eine Datei. |
| [ToImage](../../aspose.cells.rendering/workbookrender/toimage/#toimage_1)(int, Stream) | Rendert eine bestimmte Seite in einen Stream. |
| [ToImage](../../aspose.cells.rendering/workbookrender/toimage/#toimage_2)(int, string) | Rendert eine bestimmte Seite in eine Datei. |
| [ToPrinter](../../aspose.cells.rendering/workbookrender/toprinter/#toprinter)(PrinterSettings) | Rendert die Arbeitsmappe zum Drucker |
| [ToPrinter](../../aspose.cells.rendering/workbookrender/toprinter/#toprinter_2)(string) | Rendert die Arbeitsmappe zum Drucker |
| [ToPrinter](../../aspose.cells.rendering/workbookrender/toprinter/#toprinter_1)(PrinterSettings, string) | Rendert die Arbeitsmappe zum Drucker |
| [ToPrinter](../../aspose.cells.rendering/workbookrender/toprinter/#toprinter_4)(string, string) | Rendert die Arbeitsmappe zum Drucker |
| [ToPrinter](../../aspose.cells.rendering/workbookrender/toprinter/#toprinter_3)(string, int, int) | (**Obsolete.**) Rendert die Arbeitsmappe zum Drucker |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class RenderingClassWorkbookRenderDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten hinzufügen und Seitengröße festlegen
            worksheet.Cells["A1"].PutValue("Workbook Render Demo");
            worksheet.PageSetup.PaperSize = PaperSizeType.PaperLetter;

            // Bildoptionen erstellen
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            
            // Arbeitsmappen-Render erstellen und Seitengröße ermitteln
            WorkbookRender render = new WorkbookRender(workbook, options);
            float[] pageSize = render.GetPageSizeInch(0);
            
            // Ergebnisse ausgeben
            Console.WriteLine($"Page Width: {pageSize[0]} inches");
            Console.WriteLine($"Page Height: {pageSize[1]} inches");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


