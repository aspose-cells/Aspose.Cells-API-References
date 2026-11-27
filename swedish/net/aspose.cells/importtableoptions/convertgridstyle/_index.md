---
title: "ImportTableOptions.ConvertGridStyle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ImportTableOptions‑egenskap. Anger om stilen för rutnätsvyn ska tillämpas på celler"
type: docs
url: /sv/net/aspose.cells/importtableoptions/convertgridstyle/
---
## ImportTableOptions.ConvertGridStyle property

Anger om stilen från rutnätsvyn ska tillämpas på celler.

```csharp
public bool ConvertGridStyle { get; set; }
```

### Exempel

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyConvertGridStyleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa exempeldata
            DataTable dataTable = new DataTable("Products");
            dataTable.Columns.Add("ID", typeof(int));
            dataTable.Columns.Add("Product", typeof(string));
            dataTable.Columns.Add("Price", typeof(decimal));
            dataTable.Rows.Add(101, "Laptop", 999.99m);
            dataTable.Rows.Add(102, "Monitor", 249.50m);

            // Ställ in importalternativ med ConvertGridStyle aktiverat
            ImportTableOptions options = new ImportTableOptions();
            options.ConvertGridStyle = true; // This will apply grid styling to the imported data
            options.IsFieldNameShown = true;

            // Importera data med formatering
            worksheet.Cells.ImportData(dataTable, 0, 0, options);

            // Spara resultatet
            workbook.Save("ImportWithGridStyle.xlsx");
        }
    }
}
```

### Se även

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


