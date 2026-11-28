---
title: "Worksheet.CalculateArrayFormula"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet yöntemi. Formülü dizi formülü olarak hesaplar"
type: docs
url: /tr/net/aspose.cells/worksheet/calculatearrayformula/
---
## CalculateArrayFormula(string, CalculationOptions) {#calculatearrayformula}

Formülü dizi formülü olarak hesaplar.

```csharp
public object[][] CalculateArrayFormula(string formula, CalculationOptions opts)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| formül | String | Hesaplanacak formül. |
| opts | CalculationOptions | Formül hesaplama seçenekleri |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodCalculateArrayFormulaWithStringCalculationOptionsDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Biraz örnek veri doldurun
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["A2"].PutValue(2);
            worksheet.Cells["A3"].PutValue(3);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(5);
            worksheet.Cells["B3"].PutValue(6);

            // Bir dizi formülü tanımla
            string arrayFormula = "=SUM(A1:B3)";
            
            // Dizi formülünü hesaplama seçenekleriyle hesapla
            object[][] result = worksheet.CalculateArrayFormula(arrayFormula, new CalculationOptions());
            
            // Sonucu çıktı olarak ver
            Console.WriteLine("Result of array formula calculation: " + result[0][0]);
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

## CalculateArrayFormula(string, CalculationOptions, int, int) {#calculatearrayformula_1}

Formülü dizi formülü olarak hesaplar.

```csharp
public object[][] CalculateArrayFormula(string formula, CalculationOptions opts, int maxRowCount, 
    int maxColumnCount)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| formül | String | Hesaplanacak formül. |
| opts | CalculationOptions | Formül hesaplama seçenekleri |
| maxRowCount | Int32 | sonuç verisinin maksimum satır sayısı. Eğer pozitif olmayan bir değer ya da gerçek satır sayısından büyükse, gerçek satır sayısı kullanılacaktır. |
| maxColumnCount | Int32 | sonuç verisinin maksimum sütun sayısı. Eğer pozitif olmayan bir değer ya da gerçek sütun sayısından büyükse, gerçek sütun sayısı kullanılacaktır. |

### Dönüş Değeri

Hesaplanan formül sonucu.

### Açıklamalar

Formül, boyutu ve sonucu hesaplamak için dinamik dizi formülü olarak alınacaktır. Kullanıcı tarafından belirtilen maksimum boyut, hesaplanan sonucun büyük bir veri kümesi olduğu durumlarda (örneğin, hesaplanan sonuç bir bütün satır veya sütun verisine karşılık gelebilir) ancak iş gereksinimi veya performans düşüncesi nedeniyle kullanıcının bu kadar büyük bir diziye ihtiyacı olmadığında kullanılır.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodCalculateArrayFormulaWithStringCalculationOptionsInt32IDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur ve ilk çalışma sayfasına eriş
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Örnek 1: Basit dizi formülü hesaplaması
            string formula = "=ISBLANK(IF(TRUE,B2:B5))";
            CalculationOptions options = new CalculationOptions();
            object[][] result = sheet.CalculateArrayFormula(formula, options, 1, 1);
            Console.WriteLine("Result of ISBLANK(IF(TRUE,B2:B5)): " + result[0][0]);

            // Örnek 2: Dinamik aralıklı dizi formülü
            formula = "=LEN(IF({1;2;3;4},B2:B5))";
            result = sheet.CalculateArrayFormula(formula, options, 1, 1);
            Console.WriteLine("Result of LEN(IF({1;2;3;4},B2:B5)): " + result[0][0]);

            // Örnek 3: MATCH işlevli dizi formülü
            // Bazı test verileri oluştur
            sheet.Cells["B2"].PutValue(5);
            sheet.Cells["B3"].PutValue(10);
            sheet.Cells["C2"].PutValue(1);
            sheet.Cells["C3"].PutValue(2);
            sheet.Cells["D2"].PutValue(0);
            sheet.Cells["D3"].PutValue(0);

            formula = "=MATCH(1,IF(B2:B5=5,C2:C5,D2:D5),0)";
            result = sheet.CalculateArrayFormula(formula, options, 1, 1);
            Console.WriteLine("Result of MATCH formula: " + result[0][0]);
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

## CalculateArrayFormula(string, FormulaParseOptions, CalculationOptions, int, int, int, int, CalculationData) {#calculatearrayformula_2}

Formülü dizi formülü olarak hesaplar.

```csharp
public object[][] CalculateArrayFormula(string formula, FormulaParseOptions pOpts, 
    CalculationOptions cOpts, int baseCellRow, int baseCellColumn, int maxRowCount, 
    int maxColumnCount, CalculationData calculationData)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| formül | String | Hesaplanacak formül. |
| pOpts | FormulaParseOptions | Formül ayrıştırma seçenekleri |
| cOpts | CalculationOptions | Formül hesaplama seçenekleri |
| baseCellRow | Int32 | Temel hücrenin satır indeksi. |
| baseCellColumn | Int32 | Temel hücrenin sütun indeksi. |
| maxRowCount | Int32 | Sonuç verisinin maksimum satır sayısı. Eğer pozitif olmayan ya da gerçek satır sayısından büyükse, gerçek satır sayısı kullanılacaktır. |
| maxColumnCount | Int32 | Sonuç verisinin maksimum sütun sayısı. Eğer pozitif olmayan ya da gerçek satır sayısından büyükse, gerçek sütun sayısı kullanılacaktır. |
| calculationData | CalculationData | Hesaplama verileri. Kullanıcı, özel hesaplama motoru uygularken bazı statik formülleri hesaplaması gerektiğinde bu durum için kullanılır. Böyle bir durumda, kullanıcı bunu [`Calculate`](../../abstractcalculationengine/calculate/) için sağlanan hesaplama verileriyle belirtmelidir. |

### Dönüş Değeri

Hesaplanan formül sonucu.

### Açıklamalar

Formül, boyutu ve sonucu hesaplamak için dinamik dizi formülü olarak alınacaktır. Kullanıcı tarafından belirtilen maksimum boyut, hesaplanan sonucun büyük bir veri kümesi olduğu durumlarda (örneğin, hesaplanan sonuç bir bütün satır veya sütun verisine karşılık gelebilir) ancak iş gereksinimi veya performans düşüncesi nedeniyle kullanıcının bu kadar büyük bir diziye ihtiyacı olmadığında kullanılır.

### Ayrıca Bakınız

* class [FormulaParseOptions](../../formulaparseoptions/)
* class [CalculationOptions](../../calculationoptions/)
* class [CalculationData](../../calculationdata/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


