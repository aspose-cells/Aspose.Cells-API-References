---
title: "CalculationOptions.LinkedDataSources"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CalculationOptions özelliği. Formüllerde kullanılan dış bağlantılar için veri kaynaklarını belirtir"
type: docs
url: /tr/net/aspose.cells/calculationoptions/linkeddatasources/
---
## CalculationOptions.LinkedDataSources property

Formüllerde kullanılan harici bağlantılar için veri kaynaklarını belirtir.

```csharp
public Workbook[] LinkedDataSources { get; set; }
```

### Açıklamalar

[`UpdateLinkedDataSource`](../../workbook/updatelinkeddatasource/) gibi, burada hesaplanacak formüllerde kullanılan dış bağlantılar için, özellikle INDIRECT işlevinde kullanılanlar, veri kaynaklarını belirtebilirsiniz. INDIRECT işlevinde kullanılan bu dış bağlantılar, çalışma kitabının dış bağlantılarının bir parçası olarak kabul edilmez ve [`UpdateLinkedDataSource`](../../workbook/updatelinkeddatasource/) tarafından güncellenemez. Bu çalışma kitaplarının dış bağlantılarla eşleşmesi, [`FileName`](../../workbook/filename/) ve [`DataSource`](../../externallink/datasource/) tarafından belirlenir. Bu nedenle, her çalışma kitabı için [`FileName`](../../workbook/filename/) uygun bir değerle (genellikle karşılık gelen [`DataSource`](../../externallink/datasource/) ile aynı olmalıdır) belirtilmiş olduğundan emin olun, böylece beklenen şekilde bağlanabilirler.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationOptionsPropertyLinkedDataSourcesDemo
    {
        public static void Run()
        {
            // Veri içeren dış çalışma kitabı oluştur
            Workbook wbExt = new Workbook();
            wbExt.Worksheets[0].Cells["A2"].PutValue(100);
            wbExt.Worksheets.Add("Sheet2").Cells["A2"].PutValue(200);
            
            // Dış çalışma kitabına adlandırılmış aralıklar ekle
            int nameIndex1 = wbExt.Worksheets.Names.Add("Sheet1!ExtNamedRange1");
            wbExt.Worksheets.Names[nameIndex1].RefersTo = "=Sheet1!$A$2";
            int nameIndex2 = wbExt.Worksheets.Names.Add("Sheet2!ExtNamedRange2");
            wbExt.Worksheets.Names[nameIndex2].RefersTo = "=Sheet2!$A$2";
            int nameIndex3 = wbExt.Worksheets.Names.Add("GlobalNamedRange");
            wbExt.Worksheets.Names[nameIndex3].RefersTo = "=Sheet1!$A$2";

            // Ana çalışma kitabı oluştur
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Dış çalışma kitabına başvuran formülleri ayarla
            sheet.Cells["A1"].Formula = "=[External.xlsx]Sheet1!$A$2";
            sheet.Cells["A2"].Formula = "=INDIRECT(\"[External.xlsx]Sheet1!$A$2\")";
            sheet.Cells["A3"].Formula = "=INDIRECT(\"[External.xlsx]Sheet1!ExtNamedRange1\")";
            sheet.Cells["A4"].Formula = "=INDIRECT(\"[External.xlsx]!GlobalNamedRange\")";

            // LinkedDataSources kullanarak formülleri hesapla
            CalculationOptions options = new CalculationOptions();
            options.LinkedDataSources = new Workbook[] { wbExt };
            
            Console.WriteLine("Before calculation:");
            PrintCellValues(sheet);

            wb.CalculateFormula(options);
            
            Console.WriteLine("\nAfter calculation:");
            PrintCellValues(sheet);
        }

        private static void PrintCellValues(Worksheet sheet)
        {
            for (int i = 0; i < 4; i++)
            {
                Console.WriteLine($"Cell A{i+1}: {sheet.Cells[$"A{i+1}"].StringValue}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Workbook](../../workbook/)
* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


