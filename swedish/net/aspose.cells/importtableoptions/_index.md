---
title: "Klass ImportTableOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.ImportTableOptions‑klass. Representerar alternativen för att importera data till celler"
type: docs
url: /sv/net/aspose.cells/importtableoptions/
---
## ImportTableOptions class

Representerar alternativen för att importera data till celler.

```csharp
public class ImportTableOptions
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [ImportTableOptions](importtableoptions/)() | Skapar standardalternativen för import. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [CheckMergedCells](../../aspose.cells/importtableoptions/checkmergedcells/) { get; set; } | Anger om sammanslagna celler ska kontrolleras. |
| [ColumnIndexes](../../aspose.cells/importtableoptions/columnindexes/) { get; set; } | Hämtar eller anger kolumnerna (0‑baserade) som ska importeras från datakällan. null betyder att alla kolumner ska importeras. |
| [ConvertGridStyle](../../aspose.cells/importtableoptions/convertgridstyle/) { get; set; } | Anger om stilen från rutnätsvyn ska tillämpas på celler. |
| [ConvertNumericData](../../aspose.cells/importtableoptions/convertnumericdata/) { get; set; } | Hämtar eller anger ett värde som indikerar om strängvärdet ska konverteras till numeriskt eller datumvärde. |
| [DateFormat](../../aspose.cells/importtableoptions/dateformat/) { get; set; } | Hämtar eller anger datumformatsträngen för celler med importerade datum‑ och tidsvärden. |
| [DefaultValues](../../aspose.cells/importtableoptions/defaultvalues/) { get; set; } | Standardvärdet för värdet i tabellen är null. |
| [ExportCaptionAsFieldName](../../aspose.cells/importtableoptions/exportcaptionasfieldname/) { get; set; } | Anger om rubriken ska exporteras som fältnamn |
| [InsertRows](../../aspose.cells/importtableoptions/insertrows/) { get; set; } | Anger om nya rader ska läggas till för att importera dataregister. |
| [IsFieldNameShown](../../aspose.cells/importtableoptions/isfieldnameshown/) { get; set; } | Anger om fältnamnet ska importeras. |
| [IsFormulas](../../aspose.cells/importtableoptions/isformulas/) { get; set; } | Anger om data är formler. |
| [IsHtmlString](../../aspose.cells/importtableoptions/ishtmlstring/) { get; set; } | Anger om värdet innehåller HTML‑taggar. |
| [NumberFormats](../../aspose.cells/importtableoptions/numberformats/) { get; set; } | Hämtar eller anger talformaten |
| [ShiftFirstRowDown](../../aspose.cells/importtableoptions/shiftfirstrowdown/) { get; set; } | Anger om den första raden ska flyttas nedåt vid infogning av rader. |
| [Styles](../../aspose.cells/importtableoptions/styles/) { get; set; } | Hämtar och anger stilarna för varje kolumn i tabellen. |
| [TotalColumns](../../aspose.cells/importtableoptions/totalcolumns/) { get; set; } | Hämtar eller anger totalt antal kolumner att importera från datakällan. -1 betyder att alla rader i den angivna datakällan importeras. |
| [TotalRows](../../aspose.cells/importtableoptions/totalrows/) { get; set; } | Hämtar eller anger totalt antal rader att importera från datakällan. -1 betyder alla rader i den angivna datakällan. |

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en DataTable för import
            DataTable dataTable = new DataTable("SampleData");
            dataTable.Columns.Add("ID", typeof(int));
            dataTable.Columns.Add("Name", typeof(string));
            dataTable.Columns.Add("Date", typeof(DateTime));
            dataTable.Rows.Add(1, "John Doe", DateTime.Now);
            dataTable.Rows.Add(2, "Jane Smith", DateTime.Now.AddDays(1));

            // Skapa en instans av ImportTableOptions
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

            // Importera DataTable till kalkylbladet
            worksheet.Cells.ImportData(dataTable, 0, 0, importOptions);

            // Spara arbetsboken
            workbook.Save("ImportTableOptionsExample.xlsx");
            workbook.Save("ImportTableOptionsExample.pdf");
            return;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


