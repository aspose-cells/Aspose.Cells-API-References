---
title: "Cell.SetDynamicArrayFormula"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cell yöntemi. Dinamik dizi formülünü ayarlar ve mümkünse formülün komşu hücrelere yayılmasını sağlar"
type: docs
url: /tr/net/aspose.cells/cell/setdynamicarrayformula/
---
## SetDynamicArrayFormula(string, FormulaParseOptions, bool) {#setdynamicarrayformula}

Dinamik dizi formülünü ayarlar ve mümkünse formülün komşu hücrelere yayılmasını sağlar.

```csharp
public CellArea SetDynamicArrayFormula(string arrayFormula, FormulaParseOptions options, 
    bool calculateValue)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arrayFormula | String | formül ifadesi |
| seçenekler | FormulaParseOptions | formülü ayrıştırma seçenekleri. "Parse" seçeneği yoksayılacak ve formül her zaman hemen ayrıştırılacaktır |
| calculateValue | Boolean | bu dinamik dizi formülünü yayılmış aralıktaki hücreler için hesaplayıp hesaplamama. |

### Dönüş Değeri

formülün yayılması gereken aralık.

### Açıklamalar

döndürülen aralık, bu dinamik dizi formülünün yayılacağı gerçek aralıkla aynı olmayabilir. Eğer aralıkta boş olmayan hücreler varsa, formül yalnızca mevcut hücreye ayarlanacak ve "#SPILL!" olarak işaretlenecektir. Ancak bu tür bir durumda bile, bu formülün yayılması gereken tüm aralığı döndürürüz.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodSetDynamicArrayFormulaWithStringFormulaParseOptionsBooleDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;

            // A1 hücresine dinamik dizi formülü ayarla
            Cell cell1 = cells["A1"];
            cell1.SetDynamicArrayFormula("=SEQUENCE(B2)", new FormulaParseOptions(), true);

            // SEQUENCE formülünü etkileyecek B2 hücresine değeri ayarla
            cells["B2"].PutValue(3);

            // Formülleri hesapla ve dinamik dizileri yenile
            wb.CalculateFormula();
            wb.RefreshDynamicArrayFormulas(false);

            // Yayılmış aralıktaki sonuçları çıktı olarak ver
            Console.WriteLine("Dynamic array results:");
            for (int i = 0; i < 3; i++)
            {
                Console.WriteLine(cells[0, i].Value);
            }
        }
    }
}
```

### Ayrıca Bakınız

* struct [CellArea](../../cellarea/)
* class [FormulaParseOptions](../../formulaparseoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDynamicArrayFormula(string, FormulaParseOptions, object[][], bool, bool) {#setdynamicarrayformula_1}

Dinamik dizi formülünü ayarlar ve mümkünse formülün komşu hücrelere yayılmasını sağlar.

```csharp
public CellArea SetDynamicArrayFormula(string arrayFormula, FormulaParseOptions options, 
    object[][] values, bool calculateRange, bool calculateValue)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arrayFormula | String | formül ifadesi |
| seçenekler | FormulaParseOptions | formülü ayrıştırma seçenekleri. "Parse" seçeneği yoksayılacak ve formül her zaman hemen ayrıştırılacaktır |
| değerler | Object[][] | verilen dinamik dizi formülüne sahip hücreler için değerler (hesaplanmış sonuçlar) |
| calculateRange | Boolean | Bu dinamik dizi formülü için yayılmış aralığı hesaplayıp hesaplamama. "values" parametresi null değil ve bu bayrak false ise, yayılmış aralığın yüksekliği values.Length ve genişliği values[0].Length olacaktır. |
| calculateValue | Boolean | "values" null olduğunda veya bir hücre için "values" içindeki karşılık gelen öğe null olduğunda, bu dinamik dizi formülünü yayılmış aralıktaki hücreler için hesaplayıp hesaplamama. |

### Dönüş Değeri

formülün yayılması gereken aralık.

### Açıklamalar

döndürülen aralık, bu dinamik dizi formülünün yayılacağı gerçek aralıkla aynı olmayabilir. Eğer aralıkta boş olmayan hücreler varsa, formül yalnızca mevcut hücreye ayarlanacak ve "#SPILL!" olarak işaretlenecektir. Ancak bu tür bir durumda bile, bu formülün yayılması gereken tüm aralığı döndürürüz.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetDynamicArrayFormulaWithStringFormulaParseOptionsObjecDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            Cell cell = cells["A1"];
            cell.PutValue(10);
            cell = cells["A2"];
            cell.PutValue(20);
            cell = cells["B1"];
            cell.PutValue(60);
            cell = cells["B2"];
            cell.PutValue(80);

            // Dinamik dizi formülünün ayarlanacağı C1 hücresini al
            cell = worksheet.Cells["C1"];

            // Dinamik dizi formülünü tanımla
            string formula = "=A1:B2 * 2";
            
            // Formül ayrıştırma seçeneklerini oluştur
            FormulaParseOptions options = new FormulaParseOptions
            {
                Parse = true // Enable formula parsing
            };

            // Formül sonuç hücrelerini doldurmak için değerleri hazırla
            object[][] values = new object[2][];
            values[0] = new object[] { 2, 4 };
            values[1] = new object[] { 6, 8 };

            try
            {
                // Önceden hesaplanmış değerlerle dinamik dizi formülünü ayarla
                CellArea result = cell.SetDynamicArrayFormula(
                    formula,
                    options,
                    values,
                    calculateRange: false,  // Use values array dimensions for spill range
                    calculateValue: false  // Use provided values instead of calculating
                );

                Console.WriteLine($"Dynamic array formula set. Affected range: Rows {result.StartRow}-{result.EndRow}, Columns {result.StartColumn}-{result.EndColumn}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetDynamicArrayFormula: {ex.Message}");
            }

            // Çalışma kitabını değişikliklerle kaydet
            workbook.Save("SetDynamicArrayFormulaDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* struct [CellArea](../../cellarea/)
* class [FormulaParseOptions](../../formulaparseoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetDynamicArrayFormula(string, FormulaParseOptions, object[][], bool, bool, CalculationOptions) {#setdynamicarrayformula_2}

Dinamik dizi formülünü ayarlar ve mümkünse formülün komşu hücrelere yayılmasını sağlar.

```csharp
public CellArea SetDynamicArrayFormula(string arrayFormula, FormulaParseOptions options, 
    object[][] values, bool calculateRange, bool calculateValue, CalculationOptions copts)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arrayFormula | String | formül ifadesi |
| seçenekler | FormulaParseOptions | formülü ayrıştırma seçenekleri. "Parse" seçeneği yoksayılacak ve formül her zaman hemen ayrıştırılacaktır |
| değerler | Object[][] | verilen dinamik dizi formülüne sahip hücreler için değerler (hesaplanmış sonuçlar) |
| calculateRange | Boolean | Bu dinamik dizi formülü için yayılmış aralığı hesaplayıp hesaplamama. "values" parametresi null değil ve bu bayrak false ise, yayılmış aralığın yüksekliği values.Length ve genişliği values[0].Length olacaktır. |
| calculateValue | Boolean | "values" null olduğunda veya bir hücre için "values" içindeki karşılık gelen öğe null olduğunda, bu dinamik dizi formülünü yayılmış aralıktaki hücreler için hesaplayıp hesaplamama. |
| copts | CalculationOptions | Formül hesaplama seçenekleri. Genellikle, performans açısından, [`Recursive`](../../calculationoptions/recursive/) özelliği false olmalıdır. |

### Dönüş Değeri

formülün yayılması gereken aralık.

### Açıklamalar

döndürülen aralık, bu dinamik dizi formülünün yayılacağı gerçek aralıkla aynı olmayabilir. Eğer aralıkta boş olmayan hücreler varsa, formül yalnızca mevcut hücreye ayarlanacak ve "#SPILL!" olarak işaretlenecektir. Ancak bu tür bir durumda bile, bu formülün yayılması gereken tüm aralığı döndürürüz.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetDynamicArrayFormulaWithStringFormulaParseOptionsObjecDemo1
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // A2:B5 hücrelerine örnek veri doldur
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["B2"].PutValue(60);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["B3"].PutValue(55);
            worksheet.Cells["A4"].PutValue(30);
            worksheet.Cells["B4"].PutValue(40);
            worksheet.Cells["A5"].PutValue(40);
            worksheet.Cells["B5"].PutValue(70);

            // Hedef hücre D1'i al
            Cell cellD1 = worksheet.Cells["D1"];

            try
            {
                // SetDynamicArrayFormula için parametreleri hazırla
                string formula = "=FILTER(A2:A5, B2:B5>50)";
                FormulaParseOptions options = new FormulaParseOptions { Parse = true };
                object[][] values = new object[2][] { new object[] { 10 }, new object[] { 40 } };
                bool calculateRange = true;
                bool calculateValue = true;
                CalculationOptions calcOptions = new CalculationOptions { Recursive = true };

                // SetDynamicArrayFormula yöntemini belirli parametrelerle çağırın
                CellArea spillRange = cellD1.SetDynamicArrayFormula(
                    formula,
                    options,
                    values,
                    calculateRange,
                    calculateValue,
                    calcOptions
                );

                Console.WriteLine($"Dynamic array formula set successfully. Spill range: {spillRange}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetDynamicArrayFormula method: {ex.Message}");
            }

            // Sonucu kaydet
            workbook.Save("SetDynamicArrayFormulaDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* struct [CellArea](../../cellarea/)
* class [FormulaParseOptions](../../formulaparseoptions/)
* class [CalculationOptions](../../calculationoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


