---
title: "Klasse MarkdownSaveOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.MarkdownSaveOptions Klasse. Stellt die Speicheroptionen für Markdown dar."
type: docs
url: /de/net/aspose.cells/markdownsaveoptions/
---
## MarkdownSaveOptions class

Stellt die Speicheroptionen für Markdown dar.

```csharp
public class MarkdownSaveOptions : SaveOptions
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [MarkdownSaveOptions](markdownsaveoptions/)() | Erstellt Optionen zum Speichern eines Markdown-Dokuments |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [AlignColumnPadding](../../aspose.cells/markdownsaveoptions/aligncolumnpadding/) { get; set; } | Gibt an, ob die Spaltenausrichtung für erzeugte Markdown-Tabellen aktiviert ist. Wenn aktiviert, werden die Spalten durch Auffüllen des Zelleninhalts mit dem angegebenen Zeichen (typischerweise ' ' für Leerzeichen) ausgerichtet. Setzen Sie es auf '\0', um die Spaltenausrichtung zu deaktivieren (Standard). |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | Der Ordner für temporäre Dateien, der als Daten-Cache verwendet werden kann.(Vererbt von [`SaveOptions`](../saveoptions/).) |
| [CalculateFormula](../../aspose.cells/markdownsaveoptions/calculateformula/) { get; set; } | Gibt an, ob Formeln vor dem Speichern der Markdown-Datei berechnet werden sollen. |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Ob Einschränkungen der Excel-Datei geprüft werden, wenn der Benutzer zellbezogene Objekte ändert. Zum Beispiel erlaubt Excel nicht, einen Zeichenwert länger als 32 K einzugeben. Wenn Sie einen Wert länger als 32 K eingeben, wird er abgeschnitten.(Vererbt von [`SaveOptions`](../saveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Leere das Arbeitsbuch nach dem Speichern der Datei.(Vererbt von [`SaveOptions`](../saveoptions/).) |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Wenn true und das Verzeichnis nicht existiert, wird das Verzeichnis vor dem Speichern der Datei automatisch erstellt.(Vererbt von [`SaveOptions`](../saveoptions/).) |
| [Encoding](../../aspose.cells/markdownsaveoptions/encoding/) { get; set; } | Liest und setzt die Standardkodierung. |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Gibt an, ob Dokumenteigenschaften beim Speichern als .xls-Datei verschlüsselt werden. Der Standardwert ist true.(Vererbt von [`SaveOptions`](../saveoptions/).) |
| [ExportHyperlinkAsReference](../../aspose.cells/markdownsaveoptions/exporthyperlinkasreference/) { get; set; } | Gibt an, ob Hyperlinks mithilfe von Referenzdefinitionen anstelle des Inline-Formats exportiert werden sollen. Der Standardwert ist false. |
| [ExportImagesAsBase64](../../aspose.cells/markdownsaveoptions/exportimagesasbase64/) { get; set; } | Gibt an, ob Bilder im Base64-Format in Markdown gespeichert werden. Der Standardwert ist true. |
| [FormatStrategy](../../aspose.cells/markdownsaveoptions/formatstrategy/) { get; set; } | Liest und setzt die Formatstrategie beim Export des Zellenwerts als Zeichenkette. |
| [ImageOptions](../../aspose.cells/markdownsaveoptions/imageoptions/) { get; } | Rufen Sie das ImageOrPrintOptions‑Objekt vor dem Exportieren ab. |
| [LightCellsDataProvider](../../aspose.cells/markdownsaveoptions/lightcellsdataprovider/) { get; set; } | Der Datenanbieter, der Zellen­daten zum Speichern der Arbeitsmappe im Light‑Modus bereitstellt. |
| [LineSeparator](../../aspose.cells/markdownsaveoptions/lineseparator/) { get; set; } | Liest und setzt den Zeilen­separator. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Gibt an, ob die Bereiche der bedingten Formatierung und Validierung vor dem Speichern der Datei zusammengeführt werden.(Vererbt von [`SaveOptions`](../saveoptions/).) |
| [OfficeMathOutputType](../../aspose.cells/markdownsaveoptions/officemathoutputtype/) { get; set; } | Gibt an, wie OfficeMath‑Objekte nach Markdown exportiert werden. Der Standardwert ist Image. |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Gibt an, ob die neuesten Diagrammdaten zwischengespeichert werden sollen.(Vererbt von [`SaveOptions`](../saveoptions/).) |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Liest das Speicherdateiformat.(Vererbt von [`SaveOptions`](../saveoptions/).) |
| [SheetSet](../../aspose.cells/markdownsaveoptions/sheetset/) { get; set; } | Liest oder setzt die zu rendernden Arbeitsblätter. Standard ist alle sichtbaren Arbeitsblätter in der Arbeitsmappe: [`Active`](../../aspose.cells.rendering/sheetset/active/). |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Gibt an, ob externe definierte Namen vor dem Speichern der Datei sortiert werden.(Vererbt von [`SaveOptions`](../saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Gibt an, ob definierte Namen vor dem Speichern der Datei sortiert werden.(Vererbt von [`SaveOptions`](../saveoptions/).) |
| [SplitTablesByBlankRow](../../aspose.cells/markdownsaveoptions/splittablesbyblankrow/) { get; set; } | Gibt an, ob leere Zeilen im Arbeitsblatt beim Export nach Markdown als Tabellentrennzeichen behandelt werden sollen. Der Standardwert ist false. |
| [StreamProvider](../../aspose.cells/markdownsaveoptions/streamprovider/) { get; set; } | Liest oder setzt den IStreamProvider zum Exportieren von Objekten. Wenn `null`, werden die exportierten Objekte im selben Verzeichnis wie die Ausgabedatei gespeichert. |
| [TableHeaderType](../../aspose.cells/markdownsaveoptions/tableheadertype/) { get; set; } | Liest und setzt, wie die Kopfzeile der Tabelle festgelegt wird. |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Gibt an, ob die SmartArt-Einstellungen aktualisiert werden. Der Standardwert ist false.(Vererbt von [`SaveOptions`](../saveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Gibt an, ob zusammengeführte Zellen vor dem Speichern der Datei validiert werden.(Vererbt von [`SaveOptions`](../saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Liest oder setzt den Warnungs-Callback.(Vererbt von [`SaveOptions`](../saveoptions/).) |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Text;

    public class MarkdownSaveOptionsDemo
    {
        public static void MarkdownSaveOptionsExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge dem Arbeitsblatt einige Daten hinzu
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");

            // Erstelle eine Instanz von MarkdownSaveOptions
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions
            {
                Encoding = Encoding.UTF8,
                FormatStrategy = CellValueFormatStrategy.DisplayString,
                LineSeparator = "\n",
                ClearData = false,
                CachedFileFolder = "C:\\Temp",
                ValidateMergedAreas = true,
                MergeAreas = true,
                SortNames = false,
                SortExternalNames = false,
                RefreshChartCache = false,
                UpdateSmartArt = false
            };

            // Speichere die Arbeitsmappe als Markdown-Datei
            workbook.Save("MarkdownSaveOptionsExample.md", saveOptions);

            Console.WriteLine("Workbook saved as Markdown file successfully.");
        }
    }
}
```

### Siehe auch

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


