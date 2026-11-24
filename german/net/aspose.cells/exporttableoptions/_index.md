---
title: "Klasse ExportTableOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.ExportTableOptions Klasse. Stellt alle Export‑Tabellenoptionen dar"
type: docs
url: /de/net/aspose.cells/exporttableoptions/
---
## ExportTableOptions class

Stellt alle Exporttabellenoptionen dar.

```csharp
public class ExportTableOptions
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [ExportTableOptions](exporttableoptions/)() | Der Standardkonstruktor. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [AllowDBNull](../../aspose.cells/exporttableoptions/allowdbnull/) { get; set; } | Dieser Wert gibt an, ob DBNulls in dieser Tabelle zulässig sind. |
| [CheckMixedValueType](../../aspose.cells/exporttableoptions/checkmixedvaluetype/) { get; set; } | False: Aspose.Cells setzt den Typ der DataColumn anhand des Wertetyps der ersten Zeile aus Performance‑Gründen. True: Aspose.Cells prüft, ob der Wertetyp in der Spalte gemischt ist, bevor der Typ der DataColumn festgelegt wird. Ist der Wertetyp gemischt, wird der Typ der DataColumn zu string. |
| [DataTable](../../aspose.cells/exporttableoptions/datatable/) { get; set; } | Liest und setzt die DataTable, deren Spalten-Datentyp zugewiesen ist. |
| [ExportAsHtmlString](../../aspose.cells/exporttableoptions/exportashtmlstring/) { get; set; } | Exportiert den HTML-Stringwert der Zellen in die DataTable. |
| [ExportAsString](../../aspose.cells/exporttableoptions/exportasstring/) { get; set; } | Exportiert den Zeichenkettenwert der Zellen in die DataTable. |
| [ExportColumnName](../../aspose.cells/exporttableoptions/exportcolumnname/) { get; set; } | Gibt an, ob die Daten in der ersten Zeile in den Spaltennamen der DataTable exportiert werden. Der Standardwert ist false. |
| [FormatStrategy](../../aspose.cells/exporttableoptions/formatstrategy/) { get; set; } | Liest und setzt die Formatstrategie beim Exportieren des Werts als Zeichenkette. |
| [Indexes](../../aspose.cells/exporttableoptions/indexes/) { get; set; } | Die Indizes der Spalten/Zeilen, die exportiert werden sollen. |
| [IsVertical](../../aspose.cells/exporttableoptions/isvertical/) { get; set; } | True, wenn eine Zeile in der Arbeitsmappendatei eine Zeile in der DataTable darstellt. False, wenn eine Spalte in der Arbeitsmappendatei eine Zeile in der DataTable darstellt. |
| [PlotVisibleCells](../../aspose.cells/exporttableoptions/plotvisiblecells/) { get; set; } | Exportiert nur sichtbare Zellen. |
| [PlotVisibleColumns](../../aspose.cells/exporttableoptions/plotvisiblecolumns/) { get; set; } | Exportiert nur sichtbare Spalten. |
| [PlotVisibleRows](../../aspose.cells/exporttableoptions/plotvisiblerows/) { get; set; } | Exportiert nur sichtbare Zeilen. |
| [RenameStrategy](../../aspose.cells/exporttableoptions/renamestrategy/) { get; set; } | Strategie für doppelte Spaltennamen. |
| [SkipErrorValue](../../aspose.cells/exporttableoptions/skiperrorvalue/) { get; set; } | Gibt an, ob ungültige Werte für die Spalte übersprungen werden sollen. Zum Beispiel, wenn der Spaltentyp decimal ist, der Wert größer als decimal.MaxValue ist und diese Eigenschaft true ist, wird keine Ausnahme mehr ausgelöst. Der Standardwert ist false. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| virtual [PreprocessExportedValue](../../aspose.cells/exporttableoptions/preprocessexportedvalue/)(int, int, CellValue) | Verarbeitet den Wert der aktuellen zu exportierenden Zelle vor. |

### Hinweise

Wenn es spezielle Anforderungen beim Export gibt, z. B. das Ignorieren von Fehlerwerten, kann der Benutzer diese Klasse erweitern, um die entsprechenden APIs zu überschreiben und das Ziel zu erreichen.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Data;

    public class ExportTableOptionsDemo
    {
        public static void ExportTableOptionsExample()
        {
            // Erstellen Sie eine neue Arbeitsmappe und rufen Sie das erste Arbeitsblatt ab
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge einige Beispieldaten zum Arbeitsblatt hinzu
            worksheet.Cells[0, 0].PutValue("Name");
            worksheet.Cells[0, 1].PutValue("Age");
            worksheet.Cells[1, 0].PutValue("John");
            worksheet.Cells[1, 1].PutValue(30);
            worksheet.Cells[2, 0].PutValue("Jane");
            worksheet.Cells[2, 1].PutValue(25);

            // Erstelle eine Instanz von ExportTableOptions
            ExportTableOptions exportOptions = new ExportTableOptions
            {
                ExportColumnName = true,
                SkipErrorValue = true,
                PlotVisibleCells = true,
                PlotVisibleRows = true,
                PlotVisibleColumns = true,
                ExportAsString = false,
                ExportAsHtmlString = false,
                FormatStrategy = CellValueFormatStrategy.DisplayStyle,
                CheckMixedValueType = true,
                AllowDBNull = true,
                IsVertical = true,
                RenameStrategy = RenameStrategy.Digit
            };

            // Exportiere die Daten vom Arbeitsblatt in eine DataTable
            DataTable dataTable = worksheet.Cells.ExportDataTable(0, 0, 3, 2, exportOptions);

            // Zeige die exportierten Daten an
            foreach (DataRow row in dataTable.Rows)
            {
                foreach (var item in row.ItemArray)
                {
                    Console.Write(item + "\t");
                }
                Console.WriteLine();
            }

            // Speichere die Arbeitsmappe
            workbook.Save("ExportTableOptionsExample.xlsx");
            workbook.Save("ExportTableOptionsExample.pdf");
        }
    }

}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


