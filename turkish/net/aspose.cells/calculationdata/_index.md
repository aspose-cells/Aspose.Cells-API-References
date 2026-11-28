---
title: "Sınıf CalculationData"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.CalculationData sınıfı. Bir fonksiyon (örneğin fonksiyon adı, parametreler ... vb.) hesaplanırken gereken verileri temsil eder."
type: docs
url: /tr/net/aspose.cells/calculationdata/
---
## CalculationData class

Bir fonksiyon hesaplanırken gerekli verileri temsil eder; örneğin fonksiyon adı, parametreler, ...vb.

```csharp
public class CalculationData
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [CalculatedValue](../../aspose.cells/calculationdata/calculatedvalue/) { get; set; } | Bu fonksiyon için hesaplanan değeri alır veya ayarlar. |
| [Cell](../../aspose.cells/calculationdata/cell/) { get; } | Fonksiyonun bulunduğu Cell nesnesini alır. |
| [CellColumn](../../aspose.cells/calculationdata/cellcolumn/) { get; } | Fonksiyonun bulunduğu hücrenin sütun indeksini alır. |
| [CellRow](../../aspose.cells/calculationdata/cellrow/) { get; } | Fonksiyonun bulunduğu hücrenin satır indeksini alır. |
| [FunctionName](../../aspose.cells/calculationdata/functionname/) { get; } | Hesaplanacak fonksiyon adını alır. |
| [ParamCount](../../aspose.cells/calculationdata/paramcount/) { get; } | Parametre sayısını alır. |
| [Workbook](../../aspose.cells/calculationdata/workbook/) { get; } | Fonksiyonun bulunduğu Workbook nesnesini alır. |
| [Worksheet](../../aspose.cells/calculationdata/worksheet/) { get; } | Fonksiyonun bulunduğu Worksheet nesnesini alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [GetParamText](../../aspose.cells/calculationdata/getparamtext/)(int) | Verilen indeksdeki parametrenin gerçek metnini alır. |
| [GetParamValue](../../aspose.cells/calculationdata/getparamvalue/)(int) | Verilen indeksdeki parametrenin temsil edilen değer nesnesini alır. |
| [GetParamValueInArrayMode](../../aspose.cells/calculationdata/getparamvalueinarraymode/)(int, int, int) | Verilen indeksdeki parametrenin değer(ler)ini alır. Parametre hesaplanması gereken bir ifade ise, dizi modunda hesaplanır. |

### Açıklamalar

Bu sınıf tarafından sağlanan tüm nesneler yalnızca "okuma" amaçlıdır. Kullanıcı, formül hesaplama sürecinde Workbook'taki verileri değiştirmemelidir, aksi takdirde beklenmeyen sonuçlar veya istisna oluşabilir.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassCalculationDataDemo
    {
        public static void Run()
        {
            try
            {
                // Basit bir workbook ve worksheet hazırlayın
                Workbook workbook = new Workbook();
                Worksheet sheet = workbook.Worksheets[0];
                sheet.Name = "DemoSheet";

                // Özel bir fonksiyonda parametre olarak kullanılacak bazı değerleri koyun
                sheet.Cells["A1"].PutValue(5);
                sheet.Cells["A2"].PutValue(10);

                // Özel fonksiyonu çağıran bir formül ayarlayın
                sheet.Cells["B1"].Formula = "=MYFUNC(A1, A2)";

                // Özel bir motor kullanmak için hesaplama seçeneklerini yapılandırın
                CalculationOptions options = new CalculationOptions();
                options.CustomEngine = new DemoEngine();

                // Hesaplamayı gerçekleştirin – özel motor bir CalculationData örneği alacak
                workbook.CalculateFormula(options);

                // Özel işlevin sonucunu çıktı olarak verin
                Console.WriteLine("Custom function result (B1): " + sheet.Cells["B1"].Value);

                // Tamamlayıcılık için çalışma kitabını kaydedin
                workbook.Save("CalculationDataDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error while working with CalculationData: {ex.Message}");
            }
        }

        // CalculationData üyelerine erişimi gösteren özel hesaplama motoru
        private class DemoEngine : AbstractCalculationEngine
        {
            public override void Calculate(CalculationData data)
            {
                // Beklenen özel işlevi işlediğimizden emin olun
                if (data.FunctionName != null &&
                    data.FunctionName.Equals("MYFUNC", StringComparison.OrdinalIgnoreCase))
                {
                    // Parametre değerlerini alın (nesneler olarak döndürülürler)
                    object param0 = data.GetParamValue(0);
                    object param1 = data.GetParamValue(1);

                    // Parametreleri hesaplama için double'a dönüştürün
                    double val0 = Convert.ToDouble(param0);
                    double val1 = Convert.ToDouble(param1);
                    double result = val0 + val1; // simple addition

                    // Hesaplanan sonucu atayın
                    data.CalculatedValue = result;

                    // Yalnızca okunan özelliklerin okunmasını gösterin
                    Console.WriteLine("[Engine] FunctionName : " + data.FunctionName);
                    Console.WriteLine("[Engine] ParamCount   : " + data.ParamCount);
                    Console.WriteLine("[Engine] CellRow      : " + data.CellRow);
                    Console.WriteLine("[Engine] CellColumn   : " + data.CellColumn);
                }
            }
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


