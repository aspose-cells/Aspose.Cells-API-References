---
title: "Cell.SetArrayFormula"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cell yöntemi. Bir dizi formülünü hücre aralığına ayarlar"
type: docs
url: /tr/net/aspose.cells/cell/setarrayformula/
---
## SetArrayFormula(string, int, int, bool, bool) {#setarrayformula_3}

Bir dizi formülünü hücre aralığına ayarlar.

```csharp
[Obsolete("Use FormulaParseOptions for more options instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void SetArrayFormula(string arrayFormula, int rowNumber, int columnNumber, bool isR1C1, 
    bool isLocal)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arrayFormula | String | Dizi formülü. |
| rowNumber | Int32 | Dizi formülünün sonucunu dolduracak satır sayısı. |
| columnNumber | Int32 | Dizi formülünün sonucunu dolduracak sütun sayısı. |
| isR1C1 | Boolean | formülün R1C1 formülü olup olmadığı |
| isLocal | Boolean | formülün yerel biçimde olup olmadığı |

### Açıklamalar

NOT: Bu sınıf artık kullanımdan kaldırılmıştır. Bunun yerine lütfen Cell.SetArrayFormula(string,int,int,FormulaParseOptions) kullanın. Bu özellik Aralık 2019'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetArrayFormulaWithStringInt32Int32BooleanBooleanDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["A2"].Value = 20;
            worksheet.Cells["A3"].Value = 30;

            try
            {
                // Dizi formülünü ayarlamak istediğimiz hedef hücreyi al
                Cell targetCell = worksheet.Cells["B1"];

                // A1:A3 aralığındaki değerleri 2 ile çarpan bir dizi formülü ayarla
                // Parametreler: (formula, rowNumber=3, columnNumber=1, isR1C1=false, isLocal=false)
                targetCell.SetArrayFormula("=A1:A3*2", 3, 1, false, false);

                // Sonuçları görmek için çalışma kitabını hesapla
                workbook.CalculateFormula();

                // Sonuçları görüntüleyin
                Console.WriteLine($"B1 value: {targetCell.Value}");
                Console.WriteLine($"B2 value: {worksheet.Cells["B2"].Value}");
                Console.WriteLine($"B3 value: {worksheet.Cells["B3"].Value}");

                // Çalışma kitabını kaydedin
                workbook.Save("SetArrayFormulaDemo.xlsx");
                Console.WriteLine("Array formula set successfully and workbook saved.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting array formula: {ex.Message}");
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

## SetArrayFormula(string, int, int) {#setarrayformula}

Bir dizi formülünü (CTRL+SHIFT+ENTER ile MS Excel'de girilen eski dizi formülü) hücre aralığına ayarlar.

```csharp
public void SetArrayFormula(string arrayFormula, int rowNumber, int columnNumber)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arrayFormula | String | Dizi formülü. |
| rowNumber | Int32 | Dizi formülünün sonucunu dolduracak satır sayısı. |
| columnNumber | Int32 | Dizi formülünün sonucunu dolduracak sütun sayısı. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodSetArrayFormulaWithStringInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            Cell cell = cells["A1"];
            cell.SetArrayFormula("=FREQUENCY({\"79\",\"85\",\"78\",\"85\",\"50\",\"81\",\"95\",\"88\",\"97\"},{70,79,89})", 4, 1);

            workbook.CalculateFormula();

            for (int i = 0; i < 4; i++)
            {
                Console.WriteLine($"Cell A{i+1} value: {cells[i, 0].IntValue}");
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

## SetArrayFormula(string, int, int, FormulaParseOptions) {#setarrayformula_1}

Bir dizi formülünü hücre aralığına ayarlar.

```csharp
public void SetArrayFormula(string arrayFormula, int rowNumber, int columnNumber, 
    FormulaParseOptions options)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arrayFormula | String | Dizi formülü. |
| rowNumber | Int32 | Dizi formülünün sonucunu dolduracak satır sayısı. |
| columnNumber | Int32 | Dizi formülünün sonucunu dolduracak sütun sayısı. |
| seçenekler | FormulaParseOptions | Formül ayrıştırma seçenekleri. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodSetArrayFormulaWithStringInt32Int32FormulaParseOpDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // C1:E1 hücrelerine örnek veri koy
            cells["C1"].PutValue(10);
            cells["D1"].PutValue(20);
            cells["E1"].PutValue(30);

            // A1 hücresine 2 satır ve 3 sütuna yayılacak bir dizi formülü ayarla
            cells["A1"].SetArrayFormula("=TRANSPOSE(C1:E1)", 2, 1, new FormulaParseOptions());

            // Formülleri hesapla
            workbook.CalculateFormula();

            // Sonuçları çıktı olarak ver.
            Console.WriteLine("Array formula results:");
            for (int row = 0; row < 2; row++)
            {
                for (int col = 0; col < 3; col++)
                {
                    Cell cell = cells[row, col];
                    Console.WriteLine($"Cell {cell.Name}: {cell.Value}");
                }
            }
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

## SetArrayFormula(string, int, int, FormulaParseOptions, object[][]) {#setarrayformula_2}

Bir dizi formülünü hücre aralığına ayarlar.

```csharp
public void SetArrayFormula(string arrayFormula, int rowNumber, int columnNumber, 
    FormulaParseOptions options, object[][] values)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arrayFormula | String | Dizi formülü. |
| rowNumber | Int32 | Dizi formülünün sonucunu dolduracak satır sayısı. |
| columnNumber | Int32 | Dizi formülünün sonucunu dolduracak sütun sayısı. |
| seçenekler | FormulaParseOptions | Formül ayrıştırma seçenekleri. |
| değerler | Object[][] | verilen dizi formülüyle o hücrelerin değerleri |

### Ayrıca Bakınız

* class [FormulaParseOptions](../../formulaparseoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


