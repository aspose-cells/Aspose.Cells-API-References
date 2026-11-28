---
title: "CalculationData.CellColumn"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CalculationData özelliği. İşlevin bulunduğu hücrenin sütun indeksini alır"
type: docs
url: /tr/net/aspose.cells/calculationdata/cellcolumn/
---
## CalculationData.CellColumn property

Fonksiyonun bulunduğu hücrenin sütun indeksini alır.

```csharp
public int CellColumn { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationDataPropertyCellColumnDemo
    {
        public static void Run()
        {
            try
            {
                // Yeni bir çalışma kitabı oluştur
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Farklı sütunlarda formüller içeren örnek veri ekle
                worksheet.Cells["A1"].PutValue(10);
                worksheet.Cells["B1"].PutValue(20);
                worksheet.Cells["C1"].Formula = "=SUM(A1:B1)";

                // Özel bir motorla hesaplama seçenekleri oluştur
                CalculationOptions options = new CalculationOptions();
                options.CustomEngine = new CellColumnDemoEngine();

                // Formülleri hesapla
                workbook.CalculateFormula(options);

                // Hesaplanan sonucu gösterin
                Console.WriteLine("Calculated value in C1: " + worksheet.Cells["C1"].Value);

                // Sonucu kaydet
                workbook.Save("CellColumnDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }

    public class CellColumnDemoEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            if (data != null)
            {
                // Salt okunur CellColumn özelliğine eriş
                int columnIndex = data.CellColumn;
                Console.WriteLine($"Function is in column index: {columnIndex}");

                // Sütun bilgisini kullanmayı göster
                if (data.FunctionName == "SUM")
                {
                    double sum = 0;
                    for (int i = 0; i < data.ParamCount; i++)
                    {
                        object arg = data.GetParamValue(i);
                        if (arg is double)
                        {
                            sum += (double)arg;
                        }
                    }
                    data.CalculatedValue = sum;
                }
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


