---
title: "Klasse SheetRender"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Rendering.SheetRender Klasse. Stellt eine Arbeitsblatt‑Renderung dar, die das Arbeitsblatt in verschiedene Bilder wie BMP, PNG, JPEG, TIFF rendern kann. Der Konstruktor dieser Klasse muss nach der Änderung des Seiten‑Setup‑Zellstils verwendet werden."
type: docs
url: /de/net/aspose.cells.rendering/sheetrender/
---
## SheetRender class

Stellt ein Arbeitsblatt‑Rendern dar, das das Arbeitsblatt in verschiedene Bilder wie (BMP, PNG, JPEG, TIFF…) rendern kann. Der Konstruktor dieser Klasse muss nach der Änderung von pagesetup und cell style verwendet werden.

```csharp
public class SheetRender
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [SheetRender](sheetrender/)(Worksheet, ImageOrPrintOptions) | Der Konstruktor von SheetRender benötigt ein Arbeitsblatt und ImageOrPrintOptions als Parameter |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [PageCount](../../aspose.cells.rendering/sheetrender/pagecount/) { get; } | Gibt die Gesamtseitenzahl des aktuellen Arbeitsblatts zurück. |
| [PageScale](../../aspose.cells.rendering/sheetrender/pagescale/) { get; } | Gibt den berechneten Seitenskalierungsfaktor des Blatts zurück. Gibt die eingestellte Skalierung zurück, wenn [`Zoom`](../../aspose.cells/pagesetup/zoom/) gesetzt ist. Andernfalls wird die berechnete Skalierung gemäß [`FitToPagesWide`](../../aspose.cells/pagesetup/fittopageswide/) und [`FitToPagesTall`](../../aspose.cells/pagesetup/fittopagestall/) zurückgegeben. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [CustomPrint](../../aspose.cells.rendering/sheetrender/customprint/)(bool, PrintPageEventArgs) | Der Client kann die Seiteneinstellungen des Druckers steuern, wenn jede Seite mit dieser Funktion gedruckt wird. |
| [Dispose](../../aspose.cells.rendering/sheetrender/dispose/)() | Gibt Ressourcen frei, die für das Rendern erstellt und verwendet wurden. |
| [GetPageSizeInch](../../aspose.cells.rendering/sheetrender/getpagesizeinch/)(int) | Ermittelt die Seitengröße in Zoll des Ausgabebildes. |
| [ToImage](../../aspose.cells.rendering/sheetrender/toimage/#toimage)(int) | Rendert eine bestimmte Seite in ein Bitmap-Objekt. |
| [ToImage](../../aspose.cells.rendering/sheetrender/toimage/#toimage_3)(int, Stream) | Rendert eine bestimmte Seite in einen Stream. |
| [ToImage](../../aspose.cells.rendering/sheetrender/toimage/#toimage_4)(int, string) | Rendert eine bestimmte Seite in eine Datei. |
| [ToImage](../../aspose.cells.rendering/sheetrender/toimage/#toimage_1)(int, Graphics, float, float) | Bestimmte Seite in ein Graphics-Objekt rendern |
| [ToImage](../../aspose.cells.rendering/sheetrender/toimage/#toimage_2)(int, Graphics, float, float, float, float) | Bestimmte Seite in ein Graphics-Objekt rendern |
| [ToPrinter](../../aspose.cells.rendering/sheetrender/toprinter/#toprinter)(PrinterSettings) | Arbeitsblatt zum Drucker rendern |
| [ToPrinter](../../aspose.cells.rendering/sheetrender/toprinter/#toprinter_2)(string) | Arbeitsblatt zum Drucker rendern |
| [ToPrinter](../../aspose.cells.rendering/sheetrender/toprinter/#toprinter_1)(PrinterSettings, string) | Arbeitsblatt zum Drucker rendern |
| [ToPrinter](../../aspose.cells.rendering/sheetrender/toprinter/#toprinter_4)(string, string) | Arbeitsblatt zum Drucker rendern |
| [ToPrinter](../../aspose.cells.rendering/sheetrender/toprinter/#toprinter_3)(string, int, int) | (**Veraltet.**) Arbeitsblatt zum Drucker rendern |
| [ToTiff](../../aspose.cells.rendering/sheetrender/totiff/#totiff)(Stream) | Ganzes Arbeitsblatt als Tiff‑Bild in einen Stream rendern. |
| [ToTiff](../../aspose.cells.rendering/sheetrender/totiff/#totiff_1)(string) | Ganzes Arbeitsblatt als Tiff‑Bild in eine Datei rendern. |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class RenderingClassSheetRenderDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    sheet.Cells[i, j].PutValue($"Data {i},{j}");
                }
            }

            // Seitenlayout konfigurieren
            PageSetup pageSetup = sheet.PageSetup;
            pageSetup.PrintArea = "1:10";
            pageSetup.SetFitToPages(1, 1);

            // SheetRender erstellen und Kernfunktionalität demonstrieren
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            SheetRender sr = new SheetRender(sheet, options);
            
            Console.WriteLine($"Number of pages: {sr.PageCount}");
            Console.WriteLine($"Page scale: {sr.PageScale * 100}%");
            
            // Erste Seite als Bild rendern (Demonstration)
            sr.ToImage(0, "output_page1.png");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


