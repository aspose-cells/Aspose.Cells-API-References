---
title: "Workbook.UpdateCustomFunctionDefinition"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Workbook yöntemi. Özel fonksiyonların tanımını günceller"
type: docs
url: /tr/net/aspose.cells/workbook/updatecustomfunctiondefinition/
---
## Workbook.UpdateCustomFunctionDefinition method

Özel işlevlerin tanımını günceller.

```csharp
public void UpdateCustomFunctionDefinition(CustomFunctionDefinition definition)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| tanım | CustomFunctionDefinition | Kullanıcının özel gereksinimi için özel fonksiyonların özel tanımı. |

### Açıklamalar

Bu yöntem bazı özel senaryolar için kullanılabilir. Örneğin, kullanıcı bazı özel fonksiyonların parametrelerinin dizi modunda hesaplanmasını istiyorsa, o fonksiyonlar için uygulanmış [`GetArrayModeParameters`](../../customfunctiondefinition/getarraymodeparameters/) içeren kendi tanımını sağlayabilir. Formüllerin verileri güncellendikten sonra, belirtilen parametreler ilgili özel fonksiyonlar hesaplanırken otomatik olarak dizi modunda hesaplanacaktır.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodUpdateCustomFunctionDefinitionWithCustomFunctionDDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Örnek veri ekleyin.
            sheet.Cells["B1"].PutValue(1);
            sheet.Cells["C1"].PutValue(2);
            sheet.Cells["B2"].PutValue(4);
            sheet.Cells["C2"].PutValue(8);

            // Özel bir hesaplama motoru oluştur
            var customEngine = new MyCustomCalculationEngine();
            
            // Özel motor ile hesaplama seçeneklerini ayarlayın
            CalculationOptions options = new CalculationOptions
            {
                CustomEngine = customEngine
            };

            // Özel fonksiyon tanımını güncelle
            wb.UpdateCustomFunctionDefinition(new MyCustomFunctionDefinition());

            // Özel fonksiyon kullanarak formül ayarla
            sheet.Cells["A1"].Formula = "=MYFUNC(B:B+C:C)";
            
            // Formülleri hesapla
            wb.CalculateFormula(options);

            // Sonucu çıktı olarak ver
            Console.WriteLine("Custom function result: " + sheet.Cells["A1"].Value);
        }
    }

    public class MyCustomFunctionDefinition : CustomFunctionDefinition
    {
        public override int[] GetArrayModeParameters(string functionName)
        {
            // Dizi modunda işlenmesi gereken parametre indekslerini döndür
            return new int[] { 0 }; // First parameter is array mode
        }
    }

    public class MyCustomCalculationEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName == "MYFUNC")
            {
                double sum = 0;
                var paramValue = data.GetParamValue(0);
                
                if (paramValue is object[,] arrayValue)
                {
                    foreach (var val in arrayValue)
                    {
                        if (val != null)
                        {
                            sum += Convert.ToDouble(val);
                        }
                    }
                }
                else
                {
                    sum += Convert.ToDouble(paramValue);
                }
                data.CalculatedValue = sum * 2; // Custom calculation logic
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [CustomFunctionDefinition](../../customfunctiondefinition/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


