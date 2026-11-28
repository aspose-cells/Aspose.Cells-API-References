---
title: "CalculationData.CalculatedValue"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CalculationData özelliği. Bu fonksiyon için hesaplanmış değeri alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells/calculationdata/calculatedvalue/
---
## CalculationData.CalculatedValue property

Bu fonksiyon için hesaplanan değeri alır veya ayarlar.

```csharp
public object CalculatedValue { get; set; }
```

### Açıklamalar

Kullanıcı, motorun desteklediği fonksiyonlar için bu özelliği kendi özel hesaplama motorunda ayarlamalıdır; ayarlanan değer daha sonra bu özellik alındığında döndürülür. Ayarlanan değer, olası [`Value`](../../cell/value/) türlerinden biri, bu tür değerlerin bir dizisi, bir Range, Name veya ReferredArea olabilir. Bu özelliği değeri ayarlamadan önce almak, fonksiyonun Aspose.Cells'in varsayılan hesaplama motoru tarafından hesaplanmasına ve ardından hesaplanmış değerin döndürülmesine neden olur (genellikle kullanıcı tanımlı fonksiyonlar için #NAME? olmalıdır).

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationDataPropertyCalculatedValueDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veriyi ayarla
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].Formula = "=SUM(A1:A2)";

            // Özel bir motorla hesaplama seçenekleri oluştur
            CalculationOptions options = new CalculationOptions();
            options.CustomEngine = new CustomCalculationEngine();

            // Seçeneklerle formülleri hesaplayın.
            workbook.CalculateFormula(options);

            // Hesaplanmış değeri al
            Console.WriteLine("A3 calculated value: " + worksheet.Cells["A3"].Value);
        }
    }

    public class CustomCalculationEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
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
```

### Ayrıca Bakınız

* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


