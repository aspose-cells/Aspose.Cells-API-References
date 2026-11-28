---
title: "Cell.SetFormula"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cell yöntemi. Formülü ve formülün hesaplanan sonucunu ayarla"
type: docs
url: /tr/net/aspose.cells/cell/setformula/
---
## SetFormula(string, object) {#setformula_3}

Formülü ve formülün değerini (hesaplanan sonuç) ayarlar.

```csharp
public void SetFormula(string formula, object value)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| formül | String | Formül. |
| değer | Object | Formülün değeri (hesaplanan sonuç). |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodSetFormulaWithStringObjectDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Formülü dize ve nesne parametreleriyle ayarla
            cells["A1"].SetFormula("=SUM(1,2)", 4); // Will display 4 until calculation
            cells["A2"].SetFormula("=AVERAGE(5,10)", 7.5); // Will display 7.5 until calculation

            // Hesaplamadan önceki değerleri göster
            Console.WriteLine("Before Calculation:");
            Console.WriteLine("A1: " + cells["A1"].StringValue);
            Console.WriteLine("A2: " + cells["A2"].StringValue);

            // Formülleri hesapla
            workbook.CalculateFormula();

            // Hesaplamadan sonraki değerleri göster
            Console.WriteLine("\nAfter Calculation:");
            Console.WriteLine("A1: " + cells["A1"].IntValue); // Should show 3
            Console.WriteLine("A2: " + cells["A2"].DoubleValue); // Should show 7.5
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetFormula(string, FormulaParseOptions) {#setformula}

Formülü ve formülün değerini (hesaplanan sonuç) ayarlar.

```csharp
public void SetFormula(string formula, FormulaParseOptions options)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| formül | String | Formül. |
| seçenekler | FormulaParseOptions | Formül ayrıştırma seçenekleri. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodSetFormulaWithStringFormulaParseOptionsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Belirli bir hücre al (bu durumda B2)
            Cell cell = worksheet.Cells["B2"];
            
            // Gösterim için bazı başlangıç değerleri ayarla
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["B1"].PutValue(30);
            
            // Örnek 1: Varsayılan ayrıştırma seçenekleriyle basit bir formül ayarla
            cell.SetFormula("=SUM(A1:A2)", new FormulaParseOptions());
            Console.WriteLine("Formula with default options: " + cell.Formula);
            
            // Örnek 2: FormulaParseOptions kullanarak R1C1 stilinde formül ayarla
            FormulaParseOptions options = new FormulaParseOptions();
            options.Parse = true;
            options.R1C1Style = true;
            
            cell.SetFormula("=SUM(R[-1]C[-1]:R[0]C[-1])", options);
            Console.WriteLine("Formula with R1C1 style: " + cell.Formula);
            
            // Örnek 3: R1C1 formatını koruyan ayrıştırma seçenekleriyle formül ayarla
            options = new FormulaParseOptions();
            options.Parse = true;
            options.R1C1Style = true;
            cell.SetFormula("=R1C1+R2C2", options);
            Console.WriteLine("Formula preserved as R1C1: " + cell.Formula);
            
            // Sonuçları görmek için çalışma kitabını hesaplayın
            workbook.CalculateFormula();
            Console.WriteLine("Calculated value: " + cell.Value);
        }
    }
}
```

### Ayrıca Bakınız

* class [FormulaParseOptions](../../formulaparseoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetFormula(string, bool, bool, object) {#setformula_2}

Formülü ve formülün değerini ayarlayın.

```csharp
[Obsolete("Use FormulaParseOptions for more options instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void SetFormula(string formula, bool isR1C1, bool isLocal, object value)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| formül | String | Formül. |
| isR1C1 | Boolean | Formülün R1C1 formülü olup olmadığı. |
| isLocal | Boolean | Formülün yerel biçimlendirilip biçimlendirilmediği. |
| değer | Object | Formülün değeri. |

### Açıklamalar

NOT: Bu sınıf artık kullanımdan kaldırıldı. Bunun yerine lütfen Cell.SetFormula(string,FormulaParseOptions,object) yöntemini kullanın. Bu özellik Aralık 2019'dan itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetFormulaWithStringBooleanBooleanObjectDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["B1"].PutValue(30);
            worksheet.Cells["B2"].PutValue(40);

            // Formülü ayarlayacağımız hedef hücreyi alın
            Cell cell = worksheet.Cells["C1"];

            try
            {
                // Tüm parametrelerle bir formül ayarlayın
                // Parametreler: formül dizesi, isR1C1, isLocal, değer
                cell.SetFormula("=SUM(A1:B2)", false, false, null);

                // Formülü hesapla
                workbook.CalculateFormula();

                // Sonucu göster
                Console.WriteLine($"Formula set successfully. Result: {cell.Value}");

                // Çalışma kitabını kaydedin
                workbook.Save("SetFormulaDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting formula: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetFormula(string, FormulaParseOptions, object) {#setformula_1}

Formülü ve formülün değerini (hesaplanan sonuç) ayarlar.

```csharp
public void SetFormula(string formula, FormulaParseOptions options, object value)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| formül | String | Formül. |
| seçenekler | FormulaParseOptions | Formül ayrıştırma seçenekleri. |
| değer | Object | Formülün değeri (hesaplanan sonuç). |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodSetFormulaWithStringFormulaParseOptionsObjecDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];

            // Eklenti referansı ile başlangıç formülünü ayarla
            sheet.Cells[0, 0].Formula = "'externalDS.xlam'!dsfun(B1)";
            Console.WriteLine("Initial formula: " + sheet.Cells[0, 0].Formula);

            // Eklentiyi kontrol etmeden geçersiz kılmak için SetFormula kullanın
            sheet.Cells[0, 0].SetFormula("=dsfun(B1)", new FormulaParseOptions() { CheckAddIn = false }, null);
            Console.WriteLine("After SetFormula: " + sheet.Cells[0, 0].Formula);

            // Eklenti formülüne sıfırla
            sheet.Cells[0, 0].Formula = "'externalDS.xlam'!dsfun(B1)";
            Console.WriteLine("Reset to add-in formula: " + sheet.Cells[0, 0].Formula);

            // Yeni bir çalışma kitabı oluşturun ve sayfayı kopyalayın
            Workbook wb2 = new Workbook();
            wb2.Worksheets[0].Cells[0, 0].Formula = "'externalDS.xlam'!dsfunnew(C1)";
            wb2.Worksheets[0].Copy(sheet);
            Console.WriteLine("After copy: " + wb2.Worksheets[0].Cells[0, 0].Formula);
        }
    }
}
```

### Ayrıca Bakınız

* class [FormulaParseOptions](../../formulaparseoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


