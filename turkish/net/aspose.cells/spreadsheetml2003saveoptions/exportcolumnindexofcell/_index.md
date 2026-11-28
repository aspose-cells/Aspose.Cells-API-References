---
title: "SpreadsheetML2003SaveOptions.ExportColumnIndexOfCell"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SpreadsheetML2003SaveOptions özelliği. Varsayılan değer false'tur; bu, hücre önceki hücreye bitişikse sütun indeksinin göz ardı edileceği anlamına gelir"
type: docs
url: /tr/net/aspose.cells/spreadsheetml2003saveoptions/exportcolumnindexofcell/
---
## SpreadsheetML2003SaveOptions.ExportColumnIndexOfCell property

Varsayılan değer false'tur, bu hücre önceki hücreye bitişikse sütun indeksinin yoksayılacağı anlamına gelir.

```csharp
public bool ExportColumnIndexOfCell { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SpreadsheetML2003SaveOptionsPropertyExportColumnIndexOfCellDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hücrelere örnek veri ekle
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            
            // ExportColumnIndexOfCell etkinleştirilmiş kaydetme seçenekleri oluşturun
            SpreadsheetML2003SaveOptions saveOptions = new SpreadsheetML2003SaveOptions();
            saveOptions.ExportColumnIndexOfCell = true;
            
            // Çalışma kitabını sütun indeksi bilgisiyle kaydedin
            workbook.Save("output_with_column_index.xml", saveOptions);
            
            Console.WriteLine("File saved with column index information.");
        }
    }
}
```

### Ayrıca Bakınız

* class [SpreadsheetML2003SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


