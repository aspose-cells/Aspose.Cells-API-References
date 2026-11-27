---
title: "ImportTableOptions.DateFormat"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ImportTableOptions-egenskap. Hämtar eller anger datumformatsträng för celler med importerade datum/tid-värden"
type: docs
url: /sv/net/aspose.cells/importtableoptions/dateformat/
---
## ImportTableOptions.DateFormat property

Hämtar eller anger datumformatsträngen för celler med importerade datum‑ och tidsvärden.

```csharp
public string DateFormat { get; set; }
```

### Exempel

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyDateFormatDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en exempel-DataTable med datumvärden
            DataTable dataTable = new DataTable();
            dataTable.Columns.Add("DateColumn", typeof(DateTime));
            dataTable.Rows.Add(new DateTime(2023, 1, 15));
            dataTable.Rows.Add(new DateTime(2023, 2, 20));
            dataTable.Rows.Add(new DateTime(2023, 3, 25));

            // Definiera importintervallet
            Aspose.Cells.Range range = worksheet.Cells.CreateRange(0, 0, 10, 1);

            // Importera data med anpassat datumformat
            worksheet.Cells.ImportData(dataTable, 0, 0, new ImportTableOptions()
            {
                IsFieldNameShown = true,
                DateFormat = "YYYY-MM-DD"
            });

            // Spara arbetsboken för att demonstrera resultatet
            workbook.Save("DateFormatDemoOutput.xlsx");
        }
    }
}
```

### Se även

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


