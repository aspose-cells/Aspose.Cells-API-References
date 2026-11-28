---
title: "ImportTableOptions.ImportTableOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ImportTableOptions yapıcı. Varsayılan içe aktarma seçeneklerini oluşturur"
type: docs
url: /tr/net/aspose.cells/importtableoptions/importtableoptions/
---
## ImportTableOptions constructor

Varsayılan içe aktarma seçeneklerini oluşturur.

```csharp
public ImportTableOptions()
```

### Örnekler

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

### Ayrıca Bakınız

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


