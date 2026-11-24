---
title: "Klasse XmlSaveOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.XmlSaveOptions‑Klasse. Stellt die Optionen zum Speichern der Arbeitsmappe als XML‑Datei dar"
type: docs
url: /de/net/aspose.cells/xmlsaveoptions/
---
## XmlSaveOptions class

Stellt die Optionen zum Speichern der Arbeitsmappe als XML‑Datei dar.

```csharp
public class XmlSaveOptions : SaveOptions
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [XmlSaveOptions](xmlsaveoptions/)() | Erstellt Optionen zum Speichern einer XML‑Datei. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | Der Ordner für temporäre Dateien, der als Daten-Cache verwendet werden kann.(Vererbt von [`SaveOptions`](../saveoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Ob Einschränkungen der Excel-Datei geprüft werden, wenn der Benutzer zellbezogene Objekte ändert. Zum Beispiel erlaubt Excel nicht, einen Zeichenwert länger als 32 K einzugeben. Wenn Sie einen Wert länger als 32 K eingeben, wird er abgeschnitten.(Vererbt von [`SaveOptions`](../saveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Leere das Arbeitsbuch nach dem Speichern der Datei.(Vererbt von [`SaveOptions`](../saveoptions/).) |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Wenn true und das Verzeichnis nicht existiert, wird das Verzeichnis vor dem Speichern der Datei automatisch erstellt.(Vererbt von [`SaveOptions`](../saveoptions/).) |
| [DataAsAttribute](../../aspose.cells/xmlsaveoptions/dataasattribute/) { get; set; } | Gibt an, ob Daten als Attribute des Elements exportiert werden. |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Gibt an, ob Dokumenteigenschaften beim Speichern als .xls-Datei verschlüsselt werden. Der Standardwert ist true.(Vererbt von [`SaveOptions`](../saveoptions/).) |
| [ExportArea](../../aspose.cells/xmlsaveoptions/exportarea/) { get; set; } | Liest oder setzt den Exportbereich. |
| [HasHeaderRow](../../aspose.cells/xmlsaveoptions/hasheaderrow/) { get; set; } | Gibt an, ob der Bereich eine Kopfzeilenzeile enthält. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Gibt an, ob die Bereiche der bedingten Formatierung und Validierung vor dem Speichern der Datei zusammengeführt werden.(Vererbt von [`SaveOptions`](../saveoptions/).) |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Gibt an, ob die neuesten Diagrammdaten zwischengespeichert werden sollen.(Vererbt von [`SaveOptions`](../saveoptions/).) |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Liest das Speicherdateiformat.(Vererbt von [`SaveOptions`](../saveoptions/).) |
| [SheetIndexes](../../aspose.cells/xmlsaveoptions/sheetindexes/) { get; set; } | Stellt die Indizes der exportierten Arbeitsblätter dar. |
| [SheetNameAsElementName](../../aspose.cells/xmlsaveoptions/sheetnameaselementname/) { get; set; } | Gibt an, ob der Name des Arbeitsblatts als Name des Elements exportiert wird. |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Gibt an, ob externe definierte Namen vor dem Speichern der Datei sortiert werden.(Vererbt von [`SaveOptions`](../saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Gibt an, ob definierte Namen vor dem Speichern der Datei sortiert werden.(Vererbt von [`SaveOptions`](../saveoptions/).) |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Gibt an, ob die SmartArt-Einstellungen aktualisiert werden. Der Standardwert ist false.(Vererbt von [`SaveOptions`](../saveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Gibt an, ob zusammengeführte Zellen vor dem Speichern der Datei validiert werden.(Vererbt von [`SaveOptions`](../saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Liest oder setzt den Warnungs-Callback.(Vererbt von [`SaveOptions`](../saveoptions/).) |
| [XmlMapName](../../aspose.cells/xmlsaveoptions/xmlmapname/) { get; set; } | Gibt an, ob die XML‑Map in der Datei exportiert wird. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class XmlSaveOptionsDemo
    {
        public static void XmlSaveOptionsExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füllen Sie einige Daten im Arbeitsblatt ein
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue("Data2");

            // Erstellen Sie eine Instanz von XmlSaveOptions
            XmlSaveOptions saveOptions = new XmlSaveOptions();

            // Eigenschaften festlegen
            saveOptions.ExportArea = new CellArea { StartRow = 0, EndRow = 1, StartColumn = 0, EndColumn = 1 };
            saveOptions.HasHeaderRow = true;
            saveOptions.SheetIndexes = new int[] { 0 };
            saveOptions.XmlMapName = "MyXmlMap";
            saveOptions.SheetNameAsElementName = true;
            saveOptions.DataAsAttribute = false;
            saveOptions.ClearData = false;
            saveOptions.CachedFileFolder = "C:\\Temp";
            saveOptions.ValidateMergedAreas = true;
            saveOptions.MergeAreas = false;
            saveOptions.SortNames = true;
            saveOptions.SortExternalNames = false;
            saveOptions.RefreshChartCache = true;
            saveOptions.UpdateSmartArt = false;

            // Speichern Sie die Arbeitsmappe als XML-Datei
            workbook.Save("XmlSaveOptionsExample.xml", saveOptions);

            return;
        }
    }
}
```

### Siehe auch

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


