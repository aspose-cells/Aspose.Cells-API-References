---
title: "Sınıf CalculationOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.CalculationOptions sınıfı. Hesaplama seçeneklerini temsil eder"
type: docs
url: /tr/net/aspose.cells/calculationoptions/
---
## CalculationOptions class

Hesaplama seçeneklerini temsil eder.

```csharp
public class CalculationOptions
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [CalculationOptions](calculationoptions/)() | Varsayılan yapıcı. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [CalcStackSize](../../aspose.cells/calculationoptions/calcstacksize/) { get; set; } | Hücreleri özyinelemeli olarak hesaplamak için yığın boyutu. Varsayılan değer 200. |
| [CalculationMonitor](../../aspose.cells/calculationoptions/calculationmonitor/) { get; set; } | Kullanıcının formül hesaplama ilerlemesini izleyebilmesi için izleyici. |
| [CharacterEncoding](../../aspose.cells/calculationoptions/characterencoding/) { get; set; } | Formüller hesaplanırken karakterlerin kodlanması/kod çözülmesi için kullanılan kodlamayı belirtir. CHAR, CODE gibi işlevler için hesaplanan sonuç bölge ayarları ve ortamın varsayılan karakter kümesine bağlıdır. Bu özellik sayesinde kullanıcı, bu işlevler için beklenen sonucu elde etmek üzere uygun kodlamayı belirtebilir. |
| [CustomEngine](../../aspose.cells/calculationoptions/customengine/) { get; set; } | Aspose.Cells'in varsayılan hesaplama motorunu genişletmek için özel formül hesaplama motoru. |
| [IgnoreError](../../aspose.cells/calculationoptions/ignoreerror/) { get; set; } | Formüller hesaplanırken karşılaşılan hataların göz ardı edilip edilmediğini gösterir. Hata, desteklenmeyen işlev, harici bağlantılar vb. olabilir. Varsayılan değer true'dur. |
| [LinkedDataSources](../../aspose.cells/calculationoptions/linkeddatasources/) { get; set; } | Formüllerde kullanılan harici bağlantılar için veri kaynaklarını belirtir. |
| [PrecisionStrategy](../../aspose.cells/calculationoptions/precisionstrategy/) { get; set; } | Hesaplama hassasiyetinin işlenme stratejisini belirtir. |
| [Recursive](../../aspose.cells/calculationoptions/recursive/) { get; set; } | Bir hücre hesaplanırken ve diğer hücrelere bağımlıysa bağımlı hücrelerin yinelemeli olarak hesaplanıp hesaplanmayacağını gösterir. Varsayılan değer true'dur. |
| [RefreshDynamicArrayFormula](../../aspose.cells/calculationoptions/refreshdynamicarrayformula/) { get; set; } | Dinamik dizi formüllerinin formüller hesaplanmadan önce yenilenip yenilenmeyeceğini gösterir. |
| [UserSpecifiedRefreshDynamicArrayFormula](../../aspose.cells/calculationoptions/userspecifiedrefreshdynamicarrayformula/) { get; } | Kullanıcının, belirtilen formüller hesaplanmadan önce dinamik dizi formüllerinin yenilenme davranışını açıkça belirleyip belirlemediğini gösterir. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Text;

    public class CalculationOptionsDemo
    {
        public static void CalculationOptionsExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin
            worksheet.Cells["A1"].PutValue(10.555);
            worksheet.Cells["A2"].PutValue(20.6666);
            worksheet.Cells["A3"].PutValue(30.7777);
            worksheet.Cells["A4"].Formula = "=SUM(A1:A3)";

            // CalculationOptions sınıfının bir örneğini oluşturun
            CalculationOptions calcOptions = new CalculationOptions
            {
                IgnoreError = true,
                Recursive = true,
                CalcStackSize = 200,
                PrecisionStrategy = CalculationPrecisionStrategy.Round,
                CharacterEncoding = Encoding.UTF8
            };

            // İsteğe bağlı olarak, özel bir hesaplama motoru veya izleyici ayarlayabilirsiniz
            // calcOptions.CustomEngine = new MyCustomEngine();
            // calcOptions.CalculationMonitor = new MyCalculationMonitor();

            // Belirtilen seçeneklerle çalışma kitabındaki formülleri hesaplayın
            workbook.CalculateFormula(calcOptions);

            // Çalışma kitabını kaydedin
            workbook.Save("CalculationOptionsExample.xlsx");
            workbook.Save("CalculationOptionsExample.pdf");

        }
    }

    // Örnek özel hesaplama motoru (gerekiyorsa)
    public class MyCustomEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            // Özel hesaplama mantığı
            string funcName = data.FunctionName.ToUpper();
            if (funcName == "MYFUNC")
            {
                // Örnek özel fonksiyon mantığı
                int count = data.ParamCount;
                object result = null;
                for (int i = 0; i < count; i++)
                {
                    object paramValue = data.GetParamValue(i);
                    if (paramValue is ReferredArea)
                    {
                        ReferredArea ra = (ReferredArea)paramValue;
                        paramValue = ra.GetValue(0, 0);
                    }
                    // Parametreyi burada işleyin
                    // result = ...;
                }
                data.CalculatedValue = result;
            }
        }
    }

    // Örnek özel hesaplama izleyicisi (gerekiyorsa)
    public class MyCalculationMonitor : AbstractCalculationMonitor
    {
        public override void BeforeCalculate(int sheetIndex, int rowIndex, int colIndex)
        {
            // Hesaplamadan önceki mantık
            Console.WriteLine($"Before calculating cell at Sheet {sheetIndex}, Row {rowIndex}, Column {colIndex}");
        }

        public override void AfterCalculate(int sheetIndex, int rowIndex, int colIndex)
        {
            // Hesaplamadan sonraki mantık
            Console.WriteLine($"After calculating cell at Sheet {sheetIndex}, Row {rowIndex}, Column {colIndex}");
        }

        public override bool OnCircular(System.Collections.IEnumerator circularCellsData)
        {
            // Döngüsel referansları ele al
            Console.WriteLine("Circular reference detected.");
            return true; // Continue calculation
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


