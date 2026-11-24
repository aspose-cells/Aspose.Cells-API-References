---
title: "Klasse FontSetting"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.FontSetting Klasse. Stellt einen Bereich von Zeichen im Zellen-Text dar"
type: docs
url: /de/net/aspose.cells/fontsetting/
---
## FontSetting class

Stellt einen Zeichenbereich innerhalb des Zelleninhalts dar.

```csharp
public class FontSetting
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [FontSetting](fontsetting/)(int, int, WorksheetCollection) |  |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Font](../../aspose.cells/fontsetting/font/) { get; } | Gibt die Schriftart dieses Objekts zurück. |
| [Length](../../aspose.cells/fontsetting/length/) { get; } | Ermittelt die Länge der Zeichen. |
| [StartIndex](../../aspose.cells/fontsetting/startindex/) { get; } | Ermittelt den Startindex der Zeichen. |
| [TextOptions](../../aspose.cells/fontsetting/textoptions/) { get; } | Gibt die Textoptionen zurück. |
| virtual [Type](../../aspose.cells/fontsetting/type/) { get; } | Ermittelt den Typ des Textknotens. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [SetWordArtStyle](../../aspose.cells/fontsetting/setwordartstyle/)(PresetWordArtStyle) | Setzt den voreingestellten WordArt-Stil. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class FontSettingDemo
    {
        public static void FontSettingExample()
        {
            // Instanziieren eines Workbook-Objekts
            Workbook workbook = new Workbook();

            // Ein neues Arbeitsblatt zum Excel-Objekt hinzufügen
            workbook.Worksheets.Add();

            // Abrufen der Referenz des neu hinzugefügten Arbeitsblatts durch Übergabe seines Blattindexes
            Worksheet worksheet = workbook.Worksheets[0];

            // Zugriff auf die Zelle "A1" aus dem Arbeitsblatt
            Aspose.Cells.Cell cell = worksheet.Cells["A1"];

            // Hinzufügen eines Werts zur Zelle "A1"
            cell.PutValue("Visit Aspose!");

            // Abrufen des Zeichenbereichs
            FontSetting character = cell.Characters(6, 7);

            // Festlegen der Schriftart ausgewählter Zeichen auf fett
            character.Font.IsBold = true;

            // Festlegen der Schriftfarbe ausgewählter Zeichen auf blau
            character.Font.Color = Color.Blue;

            // Die Excel-Datei speichern
            workbook.Save("FontSettingExample.xlsx");
            workbook.Save("FontSettingExample.pdf");

        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


