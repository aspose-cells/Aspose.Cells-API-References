---
title: "Klasse TxtSaveOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.TxtSaveOptions Klasse. Stellt die Speicheroptionen für CSV/Tab-getrennte/andere Textformate dar"
type: docs
url: /de/net/aspose.cells/txtsaveoptions/
---
## TxtSaveOptions class

Stellt die Speicheroptionen für CSV/Tab‑getrenntes/anderes Textformat dar.

```csharp
public class TxtSaveOptions : SaveOptions
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [TxtSaveOptions](txtsaveoptions/#constructor)() | Erstellt Optionen zum Speichern von Textdateien. |
| [TxtSaveOptions](txtsaveoptions/#constructor_1)(SaveFormat) | Erstellt Optionen zum Speichern von Textdateien. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [AlwaysQuoted](../../aspose.cells/txtsaveoptions/alwaysquoted/) { get; set; } | (**Obsolete.**) Gibt an, ob immer '\"' für jedes Feld hinzugefügt wird. Wenn true, werden alle Werte in Anführungszeichen gesetzt; wenn false, werden Werte nur bei Bedarf in Anführungszeichen gesetzt (z. B. wenn Werte Sonderzeichen wie '\"', '\\n' oder das Trennzeichen enthalten). Standard ist false. |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | Der Ordner für temporäre Dateien, der als Daten-Cache verwendet werden kann.(Vererbt von [`SaveOptions`](../saveoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Ob Einschränkungen der Excel-Datei geprüft werden, wenn der Benutzer zellbezogene Objekte ändert. Zum Beispiel erlaubt Excel nicht, einen Zeichenwert länger als 32 K einzugeben. Wenn Sie einen Wert länger als 32 K eingeben, wird er abgeschnitten.(Vererbt von [`SaveOptions`](../saveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Leere das Arbeitsbuch nach dem Speichern der Datei.(Vererbt von [`SaveOptions`](../saveoptions/).) |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Wenn true und das Verzeichnis nicht existiert, wird das Verzeichnis vor dem Speichern der Datei automatisch erstellt.(Vererbt von [`SaveOptions`](../saveoptions/).) |
| [Encoding](../../aspose.cells/txtsaveoptions/encoding/) { get; set; } | Liest und setzt die Standardkodierung. |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Gibt an, ob Dokumenteigenschaften beim Speichern als .xls-Datei verschlüsselt werden. Der Standardwert ist true.(Vererbt von [`SaveOptions`](../saveoptions/).) |
| [ExportAllSheets](../../aspose.cells/txtsaveoptions/exportallsheets/) { get; set; } | Gibt an, ob alle Arbeitsblätter in die Textdatei exportiert werden. Wenn false, wird nur das aktive Arbeitsblatt exportiert, ähnlich wie in MS Excel. |
| [ExportArea](../../aspose.cells/txtsaveoptions/exportarea/) { get; set; } | Der zu exportierende Zellbereich. |
| [ExportQuotePrefix](../../aspose.cells/txtsaveoptions/exportquoteprefix/) { get; set; } | Gibt an, ob das einfache Anführungszeichen als Teil des Zellwerts exportiert werden soll, wenn [`QuotePrefix`](../style/quoteprefix/) dafür true ist. Standard ist false. |
| [FormatStrategy](../../aspose.cells/txtsaveoptions/formatstrategy/) { get; set; } | Liest und setzt die Formatstrategie beim Export des Zellenwerts als Zeichenkette. |
| [KeepSeparatorsForBlankRow](../../aspose.cells/txtsaveoptions/keepseparatorsforblankrow/) { get; set; } | Gibt an, ob Trennzeichen für leere Zeilen ausgegeben werden sollen. Der Standardwert ist false, sodass der Inhalt einer leeren Zeile standardmäßig leer ist. |
| [LightCellsDataProvider](../../aspose.cells/txtsaveoptions/lightcellsdataprovider/) { get; set; } | Der Datenanbieter zum Speichern der Arbeitsmappe im Light‑Modus. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Gibt an, ob die Bereiche der bedingten Formatierung und Validierung vor dem Speichern der Datei zusammengeführt werden.(Vererbt von [`SaveOptions`](../saveoptions/).) |
| [QuoteType](../../aspose.cells/txtsaveoptions/quotetype/) { get; set; } | Liest oder setzt, wie Werte in der exportierten Textdatei in Anführungszeichen gesetzt werden. |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Gibt an, ob die neuesten Diagrammdaten zwischengespeichert werden sollen.(Vererbt von [`SaveOptions`](../saveoptions/).) |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Liest das Speicherdateiformat.(Vererbt von [`SaveOptions`](../saveoptions/).) |
| [Separator](../../aspose.cells/txtsaveoptions/separator/) { get; set; } | Liest und setzt das Zeichen‑Trennzeichen der Textdatei. |
| [SeparatorString](../../aspose.cells/txtsaveoptions/separatorstring/) { get; set; } | Liest und setzt einen Zeichenkettenwert als Trennzeichen. |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Gibt an, ob externe definierte Namen vor dem Speichern der Datei sortiert werden.(Vererbt von [`SaveOptions`](../saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Gibt an, ob definierte Namen vor dem Speichern der Datei sortiert werden.(Vererbt von [`SaveOptions`](../saveoptions/).) |
| [TrimLeadingBlankRowAndColumn](../../aspose.cells/txtsaveoptions/trimleadingblankrowandcolumn/) { get; set; } | Gibt an, ob führende leere Zeilen und Spalten wie in MS Excel entfernt werden sollen. Standard ist true. |
| [TrimTailingBlankCells](../../aspose.cells/txtsaveoptions/trimtailingblankcells/) { get; set; } | Gibt an, ob nachfolgende leere Zellen in einer Zeile entfernt werden sollen. Standard ist false. |
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

    public class TxtSaveOptionsDemo
    {
        public static void TxtSaveOptionsExample()
        {
            // Erstelle eine Arbeitsmappe mit einigen Daten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John Doe");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Jane Smith");
            worksheet.Cells["B3"].PutValue(25);

            // Erstelle ein TxtSaveOptions‑Objekt und setze die Eigenschaften
            TxtSaveOptions saveOptions = new TxtSaveOptions
            {
                Separator = ',',
                SeparatorString = ",",
                Encoding = Encoding.UTF8,
                AlwaysQuoted = false,
                QuoteType = TxtValueQuoteType.Normal,
                FormatStrategy = CellValueFormatStrategy.DisplayStyle,
                TrimLeadingBlankRowAndColumn = true,
                TrimTailingBlankCells = false,
                KeepSeparatorsForBlankRow = false,
                ExportArea = new CellArea { StartRow = 0, EndRow = 2, StartColumn = 0, EndColumn = 1 },
                ExportQuotePrefix = false,
                ExportAllSheets = false,
                ClearData = false,
                CachedFileFolder = "cache",
                ValidateMergedAreas = true,
                MergeAreas = true,
                SortNames = true,
                SortExternalNames = true,
                RefreshChartCache = true,
                UpdateSmartArt = false
            };

            // Speichere die Arbeitsmappe als Textdatei mit den angegebenen Optionen
            workbook.Save("TxtSaveOptionsExample.txt", saveOptions);

            Console.WriteLine("Workbook saved successfully with TxtSaveOptions.");
        }
    }
}
```

### Siehe auch

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


