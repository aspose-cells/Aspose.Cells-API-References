---
title: "ImportTableOptions.ImportTableOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ImportTableOptions konstruktor. Skapar standardalternativen för import"
type: docs
url: /sv/net/aspose.cells/importtableoptions/importtableoptions/
---
## ImportTableOptions constructor

Skapar standardalternativen för import.

```csharp
public ImportTableOptions()
```

### Exempel

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsMethodCtorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            DataTable dt = new DataTable();
            dt.Columns.Add("Column1");
            dt.Rows.Add("<b>Bold Text</b>");
            
            Cells cells = workbook.Worksheets[0].Cells;
            ImportTableOptions options = new ImportTableOptions();
            options.IsHtmlString = true;
            options.IsFieldNameShown = true;
            
            cells.ImportData(dt, 0, 0, options);
            
            Console.WriteLine("Cell A2 is bold: " + cells["A2"].GetStyle().Font.IsBold);
        }
    }
}
```

### Se även

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


