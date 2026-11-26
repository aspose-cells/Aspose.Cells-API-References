---
title: "ImportTableOptions.ImportTableOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "ImportTableOptions constructor. Crea las opciones de importación predeterminadas"
type: docs
url: /es/net/aspose.cells/importtableoptions/importtableoptions/
---
## ImportTableOptions constructor

Crea las opciones de importación predeterminadas.

```csharp
public ImportTableOptions()
```

### Ejemplos

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

### Ver también

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


