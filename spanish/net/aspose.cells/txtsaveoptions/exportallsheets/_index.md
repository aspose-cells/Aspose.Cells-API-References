---
title: "TxtSaveOptions.ExportAllSheets"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TxtSaveOptions. Indica si se exportan todas las hojas al archivo de texto. Si es false, solo se exporta la hoja activa, al igual que MS Excel"
type: docs
url: /es/net/aspose.cells/txtsaveoptions/exportallsheets/
---
## TxtSaveOptions.ExportAllSheets property

Indica si se exportan todas las hojas al archivo de texto. Si es falso, solo se exporta la hoja activa, como en MS Excel.

```csharp
public bool ExportAllSheets { get; set; }
```

### Observaciones

El valor predeterminado es false.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsPropertyExportAllSheetsDemo
    {
        public static void Run()
        {
            // Cree un libro de trabajo con dos hojas
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            
            // Agregar datos de ejemplo a ambas hojas
            workbook.Worksheets[0].Cells["A1"].PutValue("Sheet1 Data");
            workbook.Worksheets[0].Cells["A2"].PutValue(1);
            workbook.Worksheets[1].Cells["A1"].PutValue("Sheet2 Data");
            workbook.Worksheets[1].Cells["A2"].PutValue(2);

            // Guarde con ExportAllSheets=false (predeterminado)
            TxtSaveOptions saveOptions = new TxtSaveOptions(SaveFormat.Csv);
            workbook.Save("output_single_sheet.csv", saveOptions);

            // Guarde con ExportAllSheets=true
            saveOptions.ExportAllSheets = true;
            workbook.Save("output_all_sheets.csv", saveOptions);
        }
    }
}
```

### Ver también

* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


