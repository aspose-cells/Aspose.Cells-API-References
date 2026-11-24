---
title: "Klasse ImportTableOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.ImportTableOptions-Klasse. Stellt die Optionen für das Importieren von Daten in Zellen dar"
type: docs
url: /de/net/aspose.cells/importtableoptions/
---
## ImportTableOptions class

Stellt die Optionen zum Importieren von Daten in Zellen dar.

```csharp
public class ImportTableOptions
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [ImportTableOptions](importtableoptions/)() | Erstellt die Standard-Importoptionen. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [CheckMergedCells](../../aspose.cells/importtableoptions/checkmergedcells/) { get; set; } | Gibt an, ob zusammengeführte Zellen überprüft werden. |
| [ColumnIndexes](../../aspose.cells/importtableoptions/columnindexes/) { get; set; } | Liest oder legt die Spalten (0-basiert) fest, die aus der Datenquelle importiert werden sollen. Null bedeutet, dass alle Spalten importiert werden. |
| [ConvertGridStyle](../../aspose.cells/importtableoptions/convertgridstyle/) { get; set; } | Gibt an, ob der Stil der Grid-Ansicht auf Zellen angewendet wird. |
| [ConvertNumericData](../../aspose.cells/importtableoptions/convertnumericdata/) { get; set; } | Liest oder legt einen Wert fest, der angibt, ob der Zeichenfolgenwert in einen numerischen oder Datumswert konvertiert werden soll. |
| [DateFormat](../../aspose.cells/importtableoptions/dateformat/) { get; set; } | Liest oder legt das Datumsformat für Zellen mit importierten Datums‑Zeit‑Werten fest. |
| [DefaultValues](../../aspose.cells/importtableoptions/defaultvalues/) { get; set; } | Der Standardwert für den Wert in der Tabelle ist null. |
| [ExportCaptionAsFieldName](../../aspose.cells/importtableoptions/exportcaptionasfieldname/) { get; set; } | Gibt an, ob die Beschriftung als Feldname exportiert wird |
| [InsertRows](../../aspose.cells/importtableoptions/insertrows/) { get; set; } | Gibt an, ob neue Zeilen für das Importieren von Datensätzen hinzugefügt werden sollen. |
| [IsFieldNameShown](../../aspose.cells/importtableoptions/isfieldnameshown/) { get; set; } | Gibt an, ob Feldnamen importiert werden sollen. |
| [IsFormulas](../../aspose.cells/importtableoptions/isformulas/) { get; set; } | Gibt an, ob die Daten Formeln sind. |
| [IsHtmlString](../../aspose.cells/importtableoptions/ishtmlstring/) { get; set; } | Gibt an, ob der Wert HTML‑Tags enthält. |
| [NumberFormats](../../aspose.cells/importtableoptions/numberformats/) { get; set; } | Liest oder legt die Zahlenformate fest |
| [ShiftFirstRowDown](../../aspose.cells/importtableoptions/shiftfirstrowdown/) { get; set; } | Gibt an, ob die erste Zeile beim Einfügen von Zeilen nach unten verschoben wird. |
| [Styles](../../aspose.cells/importtableoptions/styles/) { get; set; } | Liest und legt die Stile für jede Spalte der Tabelle fest |
| [TotalColumns](../../aspose.cells/importtableoptions/totalcolumns/) { get; set; } | Liest oder legt die Gesamtanzahl der zu importierenden Spalten aus der Datenquelle fest. -1 bedeutet, dass alle Zeilen der angegebenen Datenquelle importiert werden. |
| [TotalRows](../../aspose.cells/importtableoptions/totalrows/) { get; set; } | Liest oder legt die Gesamtanzahl der zu importierenden Zeilen aus der Datenquelle fest. -1 bedeutet, dass alle Zeilen der angegebenen Datenquelle importiert werden. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Data;

    public class ImportTableOptionsDemo
    {
        public static void ImportTableOptionsExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Eine DataTable zum Importieren erstellen
            DataTable dataTable = new DataTable("SampleData");
            dataTable.Columns.Add("ID", typeof(int));
            dataTable.Columns.Add("Name", typeof(string));
            dataTable.Columns.Add("Date", typeof(DateTime));
            dataTable.Rows.Add(1, "John Doe", DateTime.Now);
            dataTable.Rows.Add(2, "Jane Smith", DateTime.Now.AddDays(1));

            // Erstellen Sie eine Instanz von ImportTableOptions
            ImportTableOptions importOptions = new ImportTableOptions
            {
                ConvertGridStyle = true,
                ConvertNumericData = true,
                InsertRows = true,
                ShiftFirstRowDown = false,
                IsFieldNameShown = true,
                ExportCaptionAsFieldName = false,
                DateFormat = "yyyy-MM-dd",
                TotalRows = -1, // Import all rows
                TotalColumns = -1, // Import all columns
                IsHtmlString = false,
                CheckMergedCells = false
            };

            // Importieren Sie die DataTable in das Arbeitsblatt
            worksheet.Cells.ImportData(dataTable, 0, 0, importOptions);

            // Speichere die Arbeitsmappe
            workbook.Save("ImportTableOptionsExample.xlsx");
            workbook.Save("ImportTableOptionsExample.pdf");
            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


