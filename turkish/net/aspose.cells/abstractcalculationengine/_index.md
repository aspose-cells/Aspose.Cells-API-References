---
title: "Class AbstractCalculationEngine"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.AbstractCalculationEngine sınıfı. Aspose.Cells'in varsayılan hesaplama motorunu genişletmek için kullanıcıların özel hesaplama motorunu temsil eder."
type: docs
url: /tr/net/aspose.cells/abstractcalculationengine/
---
## AbstractCalculationEngine class

Kullanıcının, Aspose.Cells'in varsayılan hesaplama motorunu genişletmek için özel hesaplama motorunu temsil eder.

```csharp
public abstract class AbstractCalculationEngine
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| virtual [IsParamArrayModeRequired](../../aspose.cells/abstractcalculationengine/isparamarraymoderequired/) { get; } | Bu motorun parametrenin dizi modunda hesaplanması gerekip gerekmediğini gösterir. Varsayılan değer false'tur. Özel fonksiyonlar hesaplanırken [`GetParamValueInArrayMode`](../calculationdata/getparamvalueinarraymode/) gerekli ise ve kullanıcı bu fonksiyonların tanımını ([`UpdateCustomFunctionDefinition`](../workbook/updatecustomfunctiondefinition/) ile) güncellememişse, bu özelliğin true olarak ayarlanması gerekir. |
| virtual [IsParamLiteralRequired](../../aspose.cells/abstractcalculationengine/isparamliteralrequired/) { get; } | Bu motorun bir hesaplama yaparken parametrenin gerçek metnini gerekip gerektirmediğini gösterir. Varsayılan değer false'tur. |
| virtual [ProcessBuiltInFunctions](../../aspose.cells/abstractcalculationengine/processbuiltinfunctions/) { get; } | Yerleşik motor tarafından desteklenen yerleşik fonksiyonların bu uygulama tarafından kontrol edilip işlenip işlenmeyeceği. Varsayılan değer false'tur. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| abstract [Calculate](../../aspose.cells/abstractcalculationengine/calculate/)(CalculationData) | Verilen verilerle bir fonksiyonu hesaplar. |
| virtual [ForceRecalculate](../../aspose.cells/abstractcalculationengine/forcerecalculate/)(string) | Paylaşılan formüller hesaplanırken verilen fonksiyonun her zaman yeniden hesaplanmasını zorlayıp zorlamayacağı. |
| [SkipCalculation](../../aspose.cells/abstractcalculationengine/skipcalculation/)() | Şu anda değerlendirilmekte olan fonksiyona başvuran tüm formülün hesaplamasını atlar. |

### Açıklamalar

Kullanıcı, bu uygulamada Workbook'un herhangi bir bölümünü doğrudan değiştirmemelidir (özel fonksiyonun hesaplanan sonucu, CalculationData.CalculatedValue özelliği ile ayarlanabilir dışında). Aksi takdirde beklenmeyen sonuçlar veya Exception oluşabilir. Kullanıcı, bazı özel fonksiyonlar için hesaplanan sonuç dışındaki diğer verileri (örneğin hücrenin formülünü, stilini vb.) değiştirmesi gerekiyorsa, bu verileri bu uygulama içinde toplamalı ve formül hesaplaması kapsamı dışına çıkararak değiştirmelidir.

### Örnekler

```csharp
using Aspose.Cells;
using System;

namespace AsposeCellsExamples
{
    public class CustomCalculationEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            // Örnek: "MYFUNC" adlı bir fonksiyon için özel uygulama
            if (data.FunctionName.ToUpper() == "MYFUNC")
            {
                // MYFUNC iki parametre alır ve bunların toplamını döndürür varsayalım
                Aspose.Cells.ReferredArea paramArea1 = (Aspose.Cells.ReferredArea)data.GetParamValue(0);
                Aspose.Cells.ReferredArea paramArea2 = (Aspose.Cells.ReferredArea)data.GetParamValue(1);

                double param1 = Convert.ToDouble(paramArea1.GetValue(0, 0));
                double param2 = Convert.ToDouble(paramArea2.GetValue(0, 0));
                data.CalculatedValue = param1 + param2;
            }
        }

        public override bool ForceRecalculate(string functionName)
        {
            // "MYFUNC" özel fonksiyonu için yeniden hesaplamayı zorla
            return functionName.ToUpper() == "MYFUNC";
        }
    }

    public class CalculationEngineDemo
    {
        public static void Test()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Hücrelere bazı değerler girin
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);

            // Özel fonksiyonu kullanan bir formül ekleyin
            sheet.Cells["A3"].Formula = "=MYFUNC(A1, A2)";

            // Özel motor ile hesaplama seçeneklerini ayarlayın
            CalculationOptions options = new CalculationOptions
            {
                CustomEngine = new CustomCalculationEngine(),
                IgnoreError = false,
                Recursive = true
            };

            // Formülleri özel motor ile hesaplayın
            workbook.CalculateFormula(options);

            // Özel fonksiyonun sonucunu yazdırın
            Console.WriteLine("Result of MYFUNC(A1, A2): " + sheet.Cells["A3"].Value);

            // Çalışma kitabını kaydedin
            workbook.Save("CustomCalculationEngineExample.xlsx");
            workbook.Save("CustomCalculationEngineExample.pdf");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


