---
title: "CalculationData.Workbook"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CalculationData özelliği. Fonksiyonun bulunduğu Workbook nesnesini alır"
type: docs
url: /tr/net/aspose.cells/calculationdata/workbook/
---
## CalculationData.Workbook property

Fonksiyonun bulunduğu Workbook nesnesini alır.

```csharp
public Workbook Workbook { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationDataPropertyWorkbookDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ve formül ekle
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["B1"].Formula = "=CUSTOMFUNC()";

            // Hesaplama seçeneklerini oluştur ve özel hesaplama motorunu kaydet
            CalculationOptions options = new CalculationOptions();
            options.CustomEngine = new CustomCalcEngine();

            // Workbook özelliğinin kullanımını göstermek için seçeneklerle hesaplamayı tetikle
            workbook.CalculateFormula(options);

            // Hesaplamadan elde edilen sonucu göster
            Console.WriteLine("Calculated value in B1: " + worksheet.Cells["B1"].Value);
            Console.WriteLine("Modified value in C1: " + worksheet.Cells["C1"].Value);

            // Sonucu kaydet
            workbook.Save("PropertyWorkbookDemo.xlsx");
        }

        private class CustomCalcEngine : AbstractCalculationEngine
        {
            public override void Calculate(CalculationData data)
            {
                if (data.FunctionName == "CUSTOMFUNC")
                {
                    // CalculationData üzerinden Workbook özelliğine eriş
                    Workbook currentWorkbook = data.Workbook;
                    Worksheet currentSheet = currentWorkbook.Worksheets[0];

                    // Verileri manipüle etmek için workbook kullanımını göster
                    double inputValue = (double)currentSheet.Cells["A1"].Value;
                    currentSheet.Cells["C1"].PutValue(inputValue * 2);

                    // Hesaplanmış sonucu ayarla
                    data.CalculatedValue = inputValue * 3;
                }
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Workbook](../../workbook/)
* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


