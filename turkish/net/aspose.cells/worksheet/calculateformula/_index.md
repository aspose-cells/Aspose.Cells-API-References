---
title: "Worksheet.CalculateFormula"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet yöntemi. Bir formülü hesaplar"
type: docs
url: /tr/net/aspose.cells/worksheet/calculateformula/
---
## CalculateFormula(string) {#calculateformula}

Bir formülü hesaplar.

```csharp
public object CalculateFormula(string formula)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| formül | String | Hesaplanacak formül. |

### Dönüş Değeri

Hesaplanan formül sonucu.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodCalculateFormulaWithStringDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            wb.Settings.Region = CountryCode.USA;
            Worksheet sheet = wb.Worksheets[0];

            // Temel sayı dönüşümünü gösterin
            string formula = "=NUMBERVALUE(\"1.234\")";
            Console.WriteLine("NUMBERVALUE(\"1.234\") = " + sheet.CalculateFormula(formula));

            // Para birimi dönüşümünü gösterin
            formula = "=NUMBERVALUE(\"$1,234.56\")";
            Console.WriteLine("NUMBERVALUE(\"$1,234.56\") = " + sheet.CalculateFormula(formula));

            // Zaman dönüşümünü gösterin
            formula = "=NUMBERVALUE(\"0:25\")";
            Console.WriteLine("NUMBERVALUE(\"0:25\") = " + sheet.CalculateFormula(formula));

            // Tarih dönüşümünü gösterin
            formula = "=NUMBERVALUE(\"07/26/2023\")";
            Console.WriteLine("NUMBERVALUE(\"07/26/2023\") = " + sheet.CalculateFormula(formula));

            // Hata durumunu gösterin
            formula = "=NUMBERVALUE(\"invalid\")";
            Console.WriteLine("NUMBERVALUE(\"invalid\") = " + sheet.CalculateFormula(formula));
        }
    }
}
```

### Ayrıca Bakınız

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CalculateFormula(string, CalculationOptions) {#calculateformula_1}

Bir formül ifadesini doğrudan hesaplar.

```csharp
public object CalculateFormula(string formula, CalculationOptions opts)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| formül | String | Hesaplanacak formül. |
| opts | CalculationOptions | Formül hesaplama seçenekleri |

### Dönüş Değeri

Verilen formülün hesaplanan sonucu. Döndürülen nesne, olası [`Value`](../../cell/value/) tiplerinden biri veya ReferredArea olabilir.

### Açıklamalar

Formül, A1 hücresine ayarlanmış gibi hesaplanacaktır. Ve formül normal bir formül olarak alınacaktır. Formülün dizi formülü olarak hesaplanması ve hesaplanan sonuç için bir dizi elde edilmesi gerekiyorsa, lütfen bunun yerine [`CalculateArrayFormula`](../calculatearrayformula/) kullanın.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodCalculateFormulaWithStringCalculationOptionsDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Biraz örnek veri doldurun
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            
            // Özel bir hesaplama motoru oluşturun
            CustomEngine customEngine = new CustomEngine();
            
            // Özel motor kullanarak formülü hesapla
            CalculationOptions options = new CalculationOptions
            {
                CustomEngine = customEngine
            };
            
            object result = worksheet.CalculateFormula("=SUM(A1:A3)", options);
            
            Console.WriteLine("Calculation result: " + result);
        }
    }

    public class CustomEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName == "SUM")
            {
                double sum = 0;
                for (int i = 0; i < data.ParamCount; i++)
                {
                    object value = data.GetParamValue(i);
                    if (value is double)
                    {
                        sum += (double)value;
                    }
                }
                data.CalculatedValue = sum;
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [CalculationOptions](../../calculationoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CalculateFormula(string, FormulaParseOptions, CalculationOptions, int, int, CalculationData) {#calculateformula_2}

Bir formül ifadesini doğrudan hesaplar.

```csharp
public object CalculateFormula(string formula, FormulaParseOptions pOpts, CalculationOptions cOpts, 
    int baseCellRow, int baseCellColumn, CalculationData calculationData)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| formül | String | Hesaplanacak formül. |
| pOpts | FormulaParseOptions | Formül ayrıştırma seçenekleri. |
| cOpts | CalculationOptions | Formül hesaplama seçenekleri. |
| baseCellRow | Int32 | Temel hücrenin satır indeksi. |
| baseCellColumn | Int32 | Temel hücrenin sütun indeksi. |
| calculationData | CalculationData | Hesaplama verileri. Kullanıcı, özel hesaplama motoru uygularken bazı statik formülleri hesaplaması gerektiğinde bu durum için kullanılır. Böyle bir durumda, kullanıcı bunu [`Calculate`](../../abstractcalculationengine/calculate/) için sağlanan hesaplama verileriyle belirtmelidir. |

### Dönüş Değeri

Verilen formülün hesaplanan sonucu. Döndürülen nesne, olası [`Value`](../../cell/value/) tiplerinden biri veya ReferredArea olabilir.

### Açıklamalar

Formül, belirtilen temel hücreye ayarlanmış gibi hesaplanacaktır. Ve formül normal bir formül olarak ele alınacaktır. Formülün dizi formülü olarak hesaplanması ve hesaplanan sonuç için bir dizi elde edilmesi gerekiyorsa, lütfen bunun yerine [`CalculateArrayFormula`](../calculatearrayformula/) kullanın.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodCalculateFormulaWithStringFormulaParseOptCalculati169472Demo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek verileri doldur
            worksheet.Cells["B1"].PutValue(5);
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["C1"].PutValue(2);
            worksheet.Cells["C2"].PutValue(4);

            // Hesaplama seçeneklerini tanımla
            CalculationOptions calculationOptions = new CalculationOptions();
            
            // Formül ayrıştırma seçeneklerini tanımla
            FormulaParseOptions formulaParseOptions = new FormulaParseOptions();
            
            // Formülü tüm parametrelerle hesapla
            object result = worksheet.CalculateFormula(
                "=SUM(B1:B2, C1:C2)",  // formula
                formulaParseOptions,   // parse options
                calculationOptions,    // calculation options
                0,                     // base cell row
                0,                     // base cell column
                null                   // calculation data
            );

            // Sonucu çıktı olarak ver
            Console.WriteLine("Calculation result: " + result);
        }
    }
}
```

### Ayrıca Bakınız

* class [FormulaParseOptions](../../formulaparseoptions/)
* class [CalculationOptions](../../calculationoptions/)
* class [CalculationData](../../calculationdata/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CalculateFormula(CalculationOptions, bool) {#calculateformula_3}

Bu çalışma sayfasındaki tüm formülleri hesaplar.

```csharp
public void CalculateFormula(CalculationOptions options, bool recursive)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| seçenekler | CalculationOptions | Hesaplama seçenekleri |
| recursive | Boolean | True, çalışma sayfasının hücreleri diğer çalışma sayfalarının hücrelerine bağımlıysa, diğer çalışma sayfalarındaki bağımlı hücrelerin de hesaplanacağı anlamına gelir. False, çalışma sayfasındaki tüm formüllerin hesaplandığı ve değerlerin doğru olduğu anlamına gelir. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodCalculateFormulaWithCalculationOptionsBooleanDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ve formülleri ayarla
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["B1"].PutValue("=SUM(A1:A3)");
            
            // Hesaplama seçenekleri oluştur
            CalculationOptions options = new CalculationOptions();
            options.Recursive = true;
            options.IgnoreError = false;
            
            // Formülü seçeneklerle hesapla ve tam hesaplamayı zorla
            worksheet.CalculateFormula(options, true);
            
            // Hesaplanan sonucu çıktı olarak ver
            Console.WriteLine("Calculated value: " + worksheet.Cells["B1"].StringValue);
        }
    }
}
```

### Ayrıca Bakınız

* class [CalculationOptions](../../calculationoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


