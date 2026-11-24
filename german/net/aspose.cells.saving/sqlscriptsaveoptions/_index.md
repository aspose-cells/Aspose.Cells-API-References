---
title: "Klasse SqlScriptSaveOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Saving.SqlScriptSaveOptions Klasse. Stellt die Optionen zum Speichern von SQL dar"
type: docs
url: /de/net/aspose.cells.saving/sqlscriptsaveoptions/
---
## SqlScriptSaveOptions class

Stellt die Optionen zum Speichern von sql dar.

```csharp
public class SqlScriptSaveOptions : SaveOptions
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [SqlScriptSaveOptions](sqlscriptsaveoptions/)() | Erstellt Optionen zum Speichern einer SQL-Datei. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [AddBlankLineBetweenRows](../../aspose.cells.saving/sqlscriptsaveoptions/addblanklinebetweenrows/) { get; set; } | Füge eine leere Zeile zwischen jedem Datensatz ein. |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | Der Ordner für temporäre Dateien, die als Daten‑Cache verwendet werden können (geerbt von [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [CheckAllDataForColumnType](../../aspose.cells.saving/sqlscriptsaveoptions/checkalldataforcolumntype/) { get; set; } | Überprüfe alle Daten, um den Datentyp der Spalten zu ermitteln. |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Ob Beschränkungen der Excel‑Datei überprüft werden, wenn der Benutzer zellbezogene Objekte ändert. Zum Beispiel erlaubt Excel nicht, einen Zeichenkettenwert länger als 32 KB einzugeben. Wenn Sie einen Wert länger als 32 KB eingeben, wird er abgeschnitten (geerbt von [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [CheckIfTableExists](../../aspose.cells.saving/sqlscriptsaveoptions/checkiftableexists/) { get; set; } | Überprüfen, ob der Tabellenname vor dem Erstellen bereits existiert |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Leert die Arbeitsmappe nach dem Speichern der Datei (geerbt von [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [ColumnTypeMap](../../aspose.cells.saving/sqlscriptsaveoptions/columntypemap/) { get; set; } | Liest und setzt die Zuordnung von Spaltentypen für verschiedene Datenbanken. |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Wenn true und das Verzeichnis nicht existiert, wird das Verzeichnis vor dem Speichern der Datei automatisch erstellt (geerbt von [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [CreateTable](../../aspose.cells.saving/sqlscriptsaveoptions/createtable/) { get; set; } | Gibt an, ob das SQL zum Erstellen der Tabelle exportiert wird. |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Gibt an, ob Dokumenteigenschaften beim Speichern als .xls‑Datei verschlüsselt werden. Der Standardwert ist true.(Vererbt von [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [ExportArea](../../aspose.cells.saving/sqlscriptsaveoptions/exportarea/) { get; set; } | Liest oder setzt den Exportbereich. |
| [ExportAsString](../../aspose.cells.saving/sqlscriptsaveoptions/exportasstring/) { get; set; } | Gibt an, ob alle Daten als Zeichenfolgenwert exportiert werden. |
| [HasHeaderRow](../../aspose.cells.saving/sqlscriptsaveoptions/hasheaderrow/) { get; set; } | Gibt an, ob der Bereich eine Kopfzeilenzeile enthält. |
| [IdName](../../aspose.cells.saving/sqlscriptsaveoptions/idname/) { get; set; } | Liest und setzt den Namen der ID-Spalte. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Gibt an, ob die Bereiche der bedingten Formatierung und Validierung vor dem Speichern der Datei zusammengeführt werden.(Vererbt von [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [OperatorType](../../aspose.cells.saving/sqlscriptsaveoptions/operatortype/) { get; set; } | Liest und setzt den Operator‑Typ des SQL. |
| [PrimaryKey](../../aspose.cells.saving/sqlscriptsaveoptions/primarykey/) { get; set; } | Gibt an, welche Spalte der Primärschlüssel der Datentabelle ist. |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Gibt an, ob die neuesten Daten des Diagramms zwischengespeichert werden sollen.(Vererbt von [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Ermittelt das Speicherdateiformat.(Vererbt von [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [Separator](../../aspose.cells.saving/sqlscriptsaveoptions/separator/) { get; set; } | Liest und setzt das Zeichen‑Trennzeichen des SQL‑Skripts. |
| [SheetIndexes](../../aspose.cells.saving/sqlscriptsaveoptions/sheetindexes/) { get; set; } | Stellt die Indizes der exportierten Arbeitsblätter dar. |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Gibt an, ob externe definierte Namen vor dem Speichern der Datei sortiert werden.(Vererbt von [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Gibt an, ob definierte Namen vor dem Speichern der Datei sortiert werden.(Vererbt von [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [StartId](../../aspose.cells.saving/sqlscriptsaveoptions/startid/) { get; set; } | Liest und setzt die Start‑ID. |
| [TableName](../../aspose.cells.saving/sqlscriptsaveoptions/tablename/) { get; set; } | Liest und setzt den Tabellennamen. |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Gibt an, ob die SmartArt-Einstellung aktualisiert wird. Der Standardwert ist false.(Vererbt von [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Gibt an, ob zusammengeführte Zellen vor dem Speichern der Datei validiert werden.(Vererbt von [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Ermittelt oder legt den Warnungs-Callback fest.(Vererbt von [`SaveOptions`](../../aspose.cells/saveoptions/).) |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Saving;
    using System;

    public class SqlScriptSaveOptionsDemo
    {
        public static void SqlScriptSaveOptionsExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Arbeitsblatt mit einigen Daten füllen
            worksheet.Cells[0, 0].PutValue("ID");
            worksheet.Cells[0, 1].PutValue("Name");
            worksheet.Cells[1, 0].PutValue(1);
            worksheet.Cells[1, 1].PutValue("John Doe");
            worksheet.Cells[2, 0].PutValue(2);
            worksheet.Cells[2, 1].PutValue("Jane Doe");

            // Erstelle eine Instanz von SqlScriptSaveOptions
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
            {
                CheckIfTableExists = true,
                ColumnTypeMap = new SqlScriptColumnTypeMap(),
                CheckAllDataForColumnType = true,
                AddBlankLineBetweenRows = false,
                Separator = ';',
                OperatorType = SqlScriptOperatorType.Insert,
                PrimaryKey = 0,
                CreateTable = true,
                IdName = "ID",
                StartId = 1,
                TableName = "MyTable",
                ExportAsString = false,
                ExportArea = new CellArea { StartRow = 0, EndRow = 2, StartColumn = 0, EndColumn = 1 },
                HasHeaderRow = true,
                ClearData = false,
                CachedFileFolder = "C:\\Temp",
                ValidateMergedAreas = true,
                MergeAreas = false,
                SortNames = false,
                SortExternalNames = false,
                RefreshChartCache = false,
                WarningCallback = null,
                UpdateSmartArt = false
            };

            // Speichere die Arbeitsmappe als SQL‑Skript
            workbook.Save("MyTable.sql", saveOptions);

            return;
        }
    }
}
```

### Siehe auch

* class [SaveOptions](../../aspose.cells/saveoptions/)
* namespace [Aspose.Cells.Saving](../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../)


