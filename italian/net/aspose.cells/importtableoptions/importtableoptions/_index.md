---
title: "ImportTableOptions.ImportTableOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Costruttore ImportTableOptions. Crea le opzioni di importazione predefinite"
type: docs
url: /it/net/aspose.cells/importtableoptions/importtableoptions/
---
## ImportTableOptions constructor

Crea le opzioni di importazione predefinite.

```csharp
public ImportTableOptions()
```

### Esempi

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

### Vedi anche

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


