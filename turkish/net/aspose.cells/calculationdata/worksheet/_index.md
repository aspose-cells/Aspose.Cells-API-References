---
title: "CalculationData.Worksheet"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CalculationData özelliği. Fonksiyonun bulunduğu Worksheet nesnesini alır"
type: docs
url: /tr/net/aspose.cells/calculationdata/worksheet/
---
## CalculationData.Worksheet property

Fonksiyonun bulunduğu Worksheet nesnesini alır.

```csharp
public Worksheet Worksheet { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationDataPropertyWorksheetDemo
    {
        public static void Run()
        {
            try
            {
                // Yeni bir çalışma kitabı oluştur
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Örneği anlamlı kılmak için bazı veriler ekleyin
                worksheet.Cells["A1"].PutValue(10);
                worksheet.Cells["A2"].PutValue(20);
                worksheet.Cells["A3"].Formula = "=SUM(A1:A2)";

                // Özel bir motorla hesaplama seçenekleri oluştur
                CalculationOptions options = new CalculationOptions();
                options.CustomEngine = new WorksheetDemoEngine();

                // Seçeneklerle formülleri hesaplayın.
                workbook.CalculateFormula(options);

                // Sonucu göster
                Console.WriteLine("A3 calculated value: " + worksheet.Cells["A3"].Value);

                // Sonucu kaydet
                workbook.Save("WorksheetDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }

    public class WorksheetDemoEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName == "SUM")
            {
                // Yalnızca okunabilir Worksheet özelliğine erişin
                Worksheet worksheet = data.Worksheet;
                Console.WriteLine($"Function is in worksheet: {worksheet.Name}");

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
```

### Ayrıca Bakınız

* class [Worksheet](../../worksheet/)
* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


