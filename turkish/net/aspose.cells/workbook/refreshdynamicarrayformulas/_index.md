---
title: "Workbook.RefreshDynamicArrayFormulas"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Workbook yöntemi. Dinamik dizi formüllerinin yayılımını mevcut verilere göre komşu hücrelerin yeni aralığına genişletir. Çalışma kitabındaki diğer formüller, dinamik dizi formülleri tarafından kullanılmış olsa bile, özyinelemeli olarak hesaplanmayacaktır."
type: docs
url: /tr/net/aspose.cells/workbook/refreshdynamicarrayformulas/
---
## RefreshDynamicArrayFormulas(bool) {#refreshdynamicarrayformulas}

Dinamik dizi formüllerini (mevcut verilere göre komşu hücrelerin yeni bir aralığına yayılır) yeniler. Çalışma kitabındaki diğer formüller, dinamik dizi formülleri tarafından kullanılsa bile, yinelemeli olarak hesaplanmayacaktır.

```csharp
public void RefreshDynamicArrayFormulas(bool calculate)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| hesapla | Boolean | Bu dinamik dizi formülleri için hücre değerlerini hesaplayıp güncelleyip güncellemeyeceği |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodRefreshDynamicArrayFormulasWithBooleanDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet1 = wb.Worksheets[0];
            Worksheet sheet2 = wb.Worksheets.Add("Sheet2");

            // İlk verileri ve dinamik dizi formüllerini ayarlayın
            sheet1.Cells["A1"].PutValue("B1:B3");
            sheet1.Cells["A2"].SetDynamicArrayFormula("=INDIRECT(A1)", new FormulaParseOptions(), true);
            sheet2.Cells["B1"].SetDynamicArrayFormula("=TRANSPOSE(Sheet1!A2#)", new FormulaParseOptions(), true);

            Console.WriteLine("Before refresh:");
            PrintSpillStatus(sheet1, sheet2);

            // Aralığı değiştirin ve formülleri yenileyin
            sheet1.Cells["A1"].PutValue("B1:B5");
            wb.RefreshDynamicArrayFormulas(true);

            Console.WriteLine("\nAfter refresh:");
            PrintSpillStatus(sheet1, sheet2);
        }

        private static void PrintSpillStatus(Worksheet sheet1, Worksheet sheet2)
        {
            Console.WriteLine("Sheet1 spill range:");
            for (int i = 1; i <= 6; i++)
            {
                Cell cell = sheet1.Cells.CheckCell(i, 0);
                Console.WriteLine($"Row {i}: {(cell != null && cell.IsFormula ? "Formula" : "Empty")}");
            }

            Console.WriteLine("\nSheet2 spill range:");
            for (int i = 1; i <= 6; i++)
            {
                Cell cell = sheet2.Cells.CheckCell(0, i);
                Console.WriteLine($"Column {i}: {(cell != null && cell.IsFormula ? "Formula" : "Empty")}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RefreshDynamicArrayFormulas(bool, CalculationOptions) {#refreshdynamicarrayformulas_1}

Dinamik dizi formüllerini (mevcut verilere göre komşu hücrelerin yeni bir aralığına yayılır) yeniler.

```csharp
public void RefreshDynamicArrayFormulas(bool calculate, CalculationOptions copts)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| hesapla | Boolean | Bu dinamik dizi formülleri için hücre değerlerini hesaplayıp güncelleyip güncellemeyeceği |
| copts | CalculationOptions | Formülleri hesaplamak için seçenekler |

### Açıklamalar

Performans göz önüne alındığında, formül kendisi veya başvurduğu veri değiştiğinde tüm dinamik dizi formüllerini otomatik olarak yenilemeyiz. Bu nedenle kullanıcı, hücre değerlerini içe aktarma/ayarlama, satır/sütun/aralık ekleme/silme gibi dinamik dizi formüllerini etkileyebilecek işlemlerden sonra bu yöntemi manuel olarak çağırmalıdır. Çoğu fonksiyon içeren formül için, yayılım aralığını hesaplamak da formülün hesaplanmasını gerektirir; bu yüzden genellikle "calculate" bayrağı için true değeri tercih edilir. Formül basit bir aralık referansı veya dizi ise (örneğin "=C1:E5", "={1,2;3,4}", ...), bir aralık veya dizi üzerindeki basit bir fonksiyon ise (örneğin "=ABS(C1:E5)", "=1+{1,2;3,4}", ...) ve tüm formüller daha sonra (örneğin [`CalculateFormula`](../calculateformula/) ile) hesaplanacaksa, "calculate" bayrağı için false değeri kullanmak, performans açısından yinelenen hesaplamayı önleyebilir.

### Örnekler

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodRefreshDynamicArrayFormulasWithBooleanCalculationOptionsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek dinamik dizi formülü ekle
            worksheet.Cells["A1"].Formula = "=SEQUENCE(5)";
            
            // Hesaplama seçenekleri oluştur
            CalculationOptions opts = new CalculationOptions();
            opts.CalcStackSize = 100;
            
            // Hesaplama seçenekleriyle dinamik dizi formüllerini yenile
            workbook.RefreshDynamicArrayFormulas(true, opts);
            
            // Çalışma kitabı formüllerini hesapla
            workbook.CalculateFormula(opts);
            
            // A1:A5 aralığından sonucu çıktı al
            for (int i = 0; i < 5; i++)
            {
                Console.WriteLine(worksheet.Cells["A" + (i + 1)].Value);
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [CalculationOptions](../../calculationoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


