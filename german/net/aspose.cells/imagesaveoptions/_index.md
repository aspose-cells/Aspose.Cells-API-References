---
title: "Klasse ImageSaveOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.ImageSaveOptions-Klasse. Stellt Bildspeicheroptionen dar. Für erweiterte Verwendung verwenden Sie bitte WorkbookRender oder SheetRender"
type: docs
url: /de/net/aspose.cells/imagesaveoptions/
---
## ImageSaveOptions class

Stellt Bildspeicheroptionen dar. Für erweiterte Verwendung verwenden Sie bitte [`WorkbookRender`](../../aspose.cells.rendering/workbookrender/) oder [`SheetRender`](../../aspose.cells.rendering/sheetrender/).

```csharp
public class ImageSaveOptions : SaveOptions
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [ImageSaveOptions](imagesaveoptions/#constructor)() | Erstellt die Optionen zum Speichern einer Bilddatei. |
| [ImageSaveOptions](imagesaveoptions/#constructor_1)(SaveFormat) | Erstellt die Optionen zum Speichern einer Bilddatei. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | Der Ordner für temporäre Dateien, der als Daten-Cache verwendet werden kann.(Vererbt von [`SaveOptions`](../saveoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Ob Einschränkungen der Excel-Datei geprüft werden, wenn der Benutzer zellbezogene Objekte ändert. Zum Beispiel erlaubt Excel nicht, einen Zeichenwert länger als 32 K einzugeben. Wenn Sie einen Wert länger als 32 K eingeben, wird er abgeschnitten.(Vererbt von [`SaveOptions`](../saveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Leere das Arbeitsbuch nach dem Speichern der Datei.(Vererbt von [`SaveOptions`](../saveoptions/).) |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Wenn true und das Verzeichnis nicht existiert, wird das Verzeichnis vor dem Speichern der Datei automatisch erstellt.(Vererbt von [`SaveOptions`](../saveoptions/).) |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Gibt an, ob Dokumenteigenschaften beim Speichern als .xls-Datei verschlüsselt werden. Der Standardwert ist true.(Vererbt von [`SaveOptions`](../saveoptions/).) |
| [ImageOrPrintOptions](../../aspose.cells/imagesaveoptions/imageorprintoptions/) { get; } | Zusätzliche Bild-Erstellungsoptionen. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Gibt an, ob die Bereiche der bedingten Formatierung und Validierung vor dem Speichern der Datei zusammengeführt werden.(Vererbt von [`SaveOptions`](../saveoptions/).) |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Gibt an, ob die neuesten Diagrammdaten zwischengespeichert werden sollen.(Vererbt von [`SaveOptions`](../saveoptions/).) |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Liest das Speicherdateiformat.(Vererbt von [`SaveOptions`](../saveoptions/).) |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Gibt an, ob externe definierte Namen vor dem Speichern der Datei sortiert werden.(Vererbt von [`SaveOptions`](../saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Gibt an, ob definierte Namen vor dem Speichern der Datei sortiert werden.(Vererbt von [`SaveOptions`](../saveoptions/).) |
| [StreamProvider](../../aspose.cells/imagesaveoptions/streamprovider/) { get; set; } | Liest oder setzt den IStreamProvider für den Export von Objekten. |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Gibt an, ob die SmartArt-Einstellungen aktualisiert werden. Der Standardwert ist false.(Vererbt von [`SaveOptions`](../saveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Gibt an, ob zusammengeführte Zellen vor dem Speichern der Datei validiert werden.(Vererbt von [`SaveOptions`](../saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Liest oder setzt den Warnungs-Callback.(Vererbt von [`SaveOptions`](../saveoptions/).) |

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassImageSaveOptionsDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Image Export");

            // Legen Sie den Zielpfad fest
            string destPath = "output.png";

            // Erstellen Sie Bildspeicheroptionen
            ImageSaveOptions saveOptions = new ImageSaveOptions(SaveFormat.Png);
            
            // Passen Sie die Speicheroptionen an
            saveOptions.ImageOrPrintOptions.OnePagePerSheet = true;
            saveOptions.ImageOrPrintOptions.OnlyArea = true;

            // Arbeitsmappe mit Bildoptionen speichern
            workbook.Save(destPath, saveOptions);

            Console.WriteLine("Image saved successfully to: " + destPath);
        }
    }
}
```

### Siehe auch

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


