---
title: "ImportTableOptions.IsFormulas"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ImportTableOptions özelliği. Verilerin formül olup olmadığını gösterir"
type: docs
url: /tr/net/aspose.cells/importtableoptions/isformulas/
---
## ImportTableOptions.IsFormulas property

Verilerin formül olup olmadığını gösterir.

```csharp
public bool[] IsFormulas { get; set; }
```

### Örnekler

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyIsFormulasDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Formül içeriğine sahip örnek veri tablosu oluştur
            DataTable dt = new DataTable();
            dt.Columns.Add("Column1");
            dt.Rows.Add("=SUM(1,2,3)");
            dt.Rows.Add("=AVERAGE(4,5,6)");

            // IsFormulas özelliği ile içe aktarma seçeneklerini ayarla
            ImportTableOptions options = new ImportTableOptions();
            options.IsFormulas = new bool[] { true }; // Treat first column as formulas
            
            // Formüllerle veri içe aktar
            workbook.Worksheets[0].Cells.ImportData(dt, 0, 0, options);

            // Formüllerin doğru bir şekilde içe aktarılıp aktarılmadığını doğrula
            Console.WriteLine("Cell A1 formula: " + workbook.Worksheets[0].Cells["A1"].Formula);
            Console.WriteLine("Cell A2 formula: " + workbook.Worksheets[0].Cells["A2"].Formula);

            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


