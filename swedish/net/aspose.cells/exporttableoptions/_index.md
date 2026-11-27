---
title: "Klass ExportTableOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.ExportTableOptions klass. Representerar alla alternativ för export av tabell"
type: docs
url: /sv/net/aspose.cells/exporttableoptions/
---
## ExportTableOptions class

Representerar alla exporttabellalternativ.

```csharp
public class ExportTableOptions
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [ExportTableOptions](exporttableoptions/)() | Standardkonstruktorn. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [AllowDBNull](../../aspose.cells/exporttableoptions/allowdbnull/) { get; set; } | Detta värde indikerar om DBNulls är tillåtna i denna tabell. |
| [CheckMixedValueType](../../aspose.cells/exporttableoptions/checkmixedvaluetype/) { get; set; } | False, Aspose.Cells kommer att sätta DataColumn-typen baserat på värdetypen i den första raden för prestanda. True, Aspose.Cells kommer att kontrollera om värdetypen i kolumnen är blandad innan DataColumn-typen sätts. Om värdetypen är blandad kommer DataColumn-typen att bli string. |
| [DataTable](../../aspose.cells/exporttableoptions/datatable/) { get; set; } | Hämtar och anger DataTable där kolumnernas datatyp tilldelas. |
| [ExportAsHtmlString](../../aspose.cells/exporttableoptions/exportashtmlstring/) { get; set; } | Exporterar cellernas HTML-strängvärde till DataTable. |
| [ExportAsString](../../aspose.cells/exporttableoptions/exportasstring/) { get; set; } | Exporterar cellernas strängvärde till DataTable. |
| [ExportColumnName](../../aspose.cells/exporttableoptions/exportcolumnname/) { get; set; } | Indikerar om data i den första raden exporteras till kolumnnamnet i DataTable. Standardvärdet är false. |
| [FormatStrategy](../../aspose.cells/exporttableoptions/formatstrategy/) { get; set; } | Hämtar och anger formatstrategin när värdet exporteras som strängvärde. |
| [Indexes](../../aspose.cells/exporttableoptions/indexes/) { get; set; } | Indexen för kolumner/rader som ska exporteras. |
| [IsVertical](../../aspose.cells/exporttableoptions/isvertical/) { get; set; } | True om en rad i Workbook-filen representerar en rad i DataTable. False om en kolumn i Workbook-filen representerar en rad i DataTable. |
| [PlotVisibleCells](../../aspose.cells/exporttableoptions/plotvisiblecells/) { get; set; } | Exporterar endast synliga celler. |
| [PlotVisibleColumns](../../aspose.cells/exporttableoptions/plotvisiblecolumns/) { get; set; } | Exporterar endast synliga kolumner. |
| [PlotVisibleRows](../../aspose.cells/exporttableoptions/plotvisiblerows/) { get; set; } | Exporterar endast synliga rader. |
| [RenameStrategy](../../aspose.cells/exporttableoptions/renamestrategy/) { get; set; } | Strategi för dubblettnamn på kolumner. |
| [SkipErrorValue](../../aspose.cells/exporttableoptions/skiperrorvalue/) { get; set; } | Indikerar om ogiltiga värden för kolumnen ska hoppas över. Till exempel, om kolumntypen är decimal, värdet är större än decimal.MaxValue och denna egenskap är true, kommer vi inte att kasta ett undantag igen. Standardvärdet är false. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| virtual [PreprocessExportedValue](../../aspose.cells/exporttableoptions/preprocessexportedvalue/)(int, int, CellValue) | Förprocessa värdet i den aktuella cellen som ska exporteras. |

### Anmärkningar

Om det finns särskilda krav på exporten, såsom att ignorera felvärden, kan användaren utöka den här klassen för att skriva över motsvarande API:er för att uppnå målet.

### Exempel

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
            // Skapa en ny arbetsbok och hämta det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite exempeldata i kalkylbladet
            worksheet.Cells[0, 0].PutValue("Name");
            worksheet.Cells[0, 1].PutValue("Age");
            worksheet.Cells[1, 0].PutValue("John");
            worksheet.Cells[1, 1].PutValue(30);
            worksheet.Cells[2, 0].PutValue("Jane");
            worksheet.Cells[2, 1].PutValue(25);

            // Skapa en instans av ExportTableOptions
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

            // Exportera data från kalkylbladet till en DataTable
            DataTable dataTable = worksheet.Cells.ExportDataTable(0, 0, 3, 2, exportOptions);

            // Visa den exporterade datan
            foreach (DataRow row in dataTable.Rows)
            {
                foreach (var item in row.ItemArray)
                {
                    Console.Write(item + "\t");
                }
                Console.WriteLine();
            }

            // Spara arbetsboken
            workbook.Save("ExportTableOptionsExample.xlsx");
            workbook.Save("ExportTableOptionsExample.pdf");
        }
    }

}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


