---
title: "ExportTableOptions.CheckMixedValueType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ExportTableOptions-egenskap. False Aspose.Cells kommer att sätta DataColumns-typen baserat på värdetypen för den första raden för prestanda. True Aspose.Cells kommer att kontrollera om värdetypen i kolumnen är blandad innan DataColumns-typen sätts. Och om värdetypen är blandad blir DataColumns-typen string."
type: docs
url: /sv/net/aspose.cells/exporttableoptions/checkmixedvaluetype/
---
## ExportTableOptions.CheckMixedValueType property

False, Aspose.Cells kommer att sätta DataColumn-typen baserat på värdetypen i den första raden för prestanda. True, Aspose.Cells kommer att kontrollera om värdetypen i kolumnen är blandad innan DataColumn-typen sätts. Om värdetypen är blandad kommer DataColumn-typen att bli string.

```csharp
public bool CheckMixedValueType { get; set; }
```

### Exempel

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExportTableOptionsPropertyCheckMixedValueTypeDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till rubriker
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Value Date");

            // Lägg till exempeldata med blandade typer
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue(DateTime.Now);
            worksheet.Cells["A3"].PutValue(2.5);
            worksheet.Cells["B3"].PutValue("2023-01-15");
            worksheet.Cells["A4"].PutValue("3");
            worksheet.Cells["B4"].PutValue(DateTime.Now.AddDays(1));

            // Skapa exportalternativ med CheckMixedValueType aktiverat
            ExportTableOptions options = new ExportTableOptions
            {
                CheckMixedValueType = true,
                ExportColumnName = true
            };

            // Exportera data till DataTable
            DataTable dataTable = worksheet.Cells.ExportDataTable(0, 0, 4, 2, options);

            // Visa resultat
            Console.WriteLine("Columns: " + dataTable.Columns.Count);
            Console.WriteLine("Rows: " + dataTable.Rows.Count);
            Console.WriteLine("ID column type: " + dataTable.Columns["ID"].DataType);
            Console.WriteLine("Value Date column type: " + dataTable.Columns["Value Date"].DataType);
        }
    }
}
```

### Se även

* class [ExportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


