---
title: "Cell.SetSharedFormula"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Hücre yöntemi. Bir formülü hücre aralığına ayarlar"
type: docs
url: /tr/net/aspose.cells/cell/setsharedformula/
---
## SetSharedFormula(string, int, int, bool, bool) {#setsharedformula_3}

Bir formülü hücre aralığına ayarlar.

```csharp
[Obsolete("Use FormulaParseOptions for more options instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void SetSharedFormula(string sharedFormula, int rowNumber, int columnNumber, bool isR1C1, 
    bool isLocal)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sharedFormula | String | Paylaşılan formül. |
| rowNumber | Int32 | Formülü doldurmak için satır sayısı. |
| columnNumber | Int32 | Formülü doldurmak için sütun sayısı. |
| isR1C1 | Boolean | formülün R1C1 formülü olup olmadığı |
| isLocal | Boolean | formülün yerel biçimde olup olmadığı |

### Açıklamalar

NOT: Bu sınıf artık kullanımdan kaldırıldı. Bunun yerine lütfen Cell.SetSharedFormula(string,int,int,FormulaParseOptions) metodunu kullanın. Bu özellik Aralık 2019'dan itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetSharedFormulaWithStringInt32Int32BooleanBooleanDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluşturun ve ilk çalışma sayfasına erişin
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            // A sütununa örnek veri doldurun
            for (int row = 0; row < 5; row++)
            {
                cells[row, 0].Value = row + 1; // A1-A5: 1-5
            }

            // Paylaşılan formülü ayarlamak için hedef hücre B1'i alın
            Cell targetCell = cells[0, 1]; // B1

            try
            {
                // A sütunundaki değerlerin karesini hesaplamak için paylaşılan formülü ayarlayın
                // Parametreler: (formula, rowCount=5, columnCount=1, isR1C1=false, isLocal=false)
#pragma warning disable 0618 // Disable obsolete warning for demonstration
                targetCell.SetSharedFormula("=A1^2", 5, 1, false, false);
#pragma warning restore 0618

                // Formül yayılımını doğrulayın
                Console.WriteLine($"B1 formula: {targetCell.Formula}");
                Console.WriteLine($"B5 formula: {cells[4, 1].Formula}");

                // Formül sonuçlarını yenilemek için çalışma kitabını hesaplayın
                workbook.CalculateFormula();

                Console.WriteLine($"A1 value: {cells["A1"].Value}");
                Console.WriteLine($"A5 value: {cells["A5"].Value}");
                Console.WriteLine($"B1 value: {targetCell.Value}");
                Console.WriteLine($"B5 value: {cells[4, 1].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting shared formula: {ex.Message}");
                return;
            }

            // Değiştirilmiş çalışma kitabını kaydet
            workbook.Save("SetSharedFormulaDemo.xlsx");
            Console.WriteLine("Spreadsheet saved successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetSharedFormula(string, int, int) {#setsharedformula}

Paylaşılan formülleri hücre aralığına ayarlar.

```csharp
public void SetSharedFormula(string sharedFormula, int rowNumber, int columnNumber)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sharedFormula | String | Paylaşılan formül. |
| rowNumber | Int32 | Formülü doldurmak için satır sayısı. |
| columnNumber | Int32 | Formülü doldurmak için sütun sayısı. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodSetSharedFormulaWithStringInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // B1'den B20'ye kadar B sütununda bir paylaşılan formül ayarlayın
            cells["B1"].SetSharedFormula("=C1*2", 20, 1);

            // Formül hesaplamasını göstermek için C sütununda bazı değerler ayarlayın
            for (int i = 0; i < 20; i++)
            {
                cells[i, 2].PutValue(i + 1); // Column C values (C1=1, C2=2...)
            }

            // Formülleri hesapla
            workbook.CalculateFormula();

            // Doğrulama için sonuçları çıktı alın
            for (int i = 0; i < 5; i++) // Display first 5 results
            {
                Console.WriteLine($"B{i+1} value: {cells[i, 1].Value}");
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

## SetSharedFormula(string, int, int, FormulaParseOptions) {#setsharedformula_1}

Paylaşılan formülleri hücre aralığına ayarlar.

```csharp
public void SetSharedFormula(string sharedFormula, int rowNumber, int columnNumber, 
    FormulaParseOptions options)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sharedFormula | String | Paylaşılan formül. |
| rowNumber | Int32 | Formülü doldurmak için satır sayısı. |
| columnNumber | Int32 | Formülü doldurmak için sütun sayısı. |
| seçenekler | FormulaParseOptions | Formül ayrıştırma seçenekleri. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodSetSharedFormulaWithStringInt32Int32FormulaParseOpDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluşturun ve ilk çalışma sayfasına erişin
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // A sütununa örnek veri doldurun
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);

            // Paylaşılan formülü ayarlayacağımız hedef hücreyi alın
            Cell targetCell = worksheet.Cells["B1"];

            try
            {
                // Varsayılan ayarlarla formül ayrıştırma seçenekleri oluşturun
                FormulaParseOptions options = new FormulaParseOptions();

                // B1'den başlayarak 3 satır ve 2 sütun için paylaşılan formül ayarlayın
                targetCell.SetSharedFormula("=A1*2", 3, 2, options);

                Console.WriteLine("Shared formula set successfully for B1:C3 range");
                Console.WriteLine("B1 formula: " + worksheet.Cells["B1"].Formula);
                Console.WriteLine("C3 formula: " + worksheet.Cells["C3"].Formula);

                workbook.CalculateFormula();
                Console.WriteLine("B3 value: " + worksheet.Cells["B3"].Value);
                Console.WriteLine("B1 value: " + worksheet.Cells["B1"].Value);
                Console.WriteLine("C3 value: " + worksheet.Cells["C3"].Value);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting shared formula: {ex.Message}");
            }

            // Değiştirilmiş çalışma kitabını kaydet
            workbook.Save("SetSharedFormulaDemo.xlsx");
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

## SetSharedFormula(string, int, int, FormulaParseOptions, object[][]) {#setsharedformula_2}

Paylaşılan formülleri hücre aralığına ayarlar.

```csharp
public void SetSharedFormula(string sharedFormula, int rowNumber, int columnNumber, 
    FormulaParseOptions options, object[][] values)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sharedFormula | String | Paylaşılan formül. |
| rowNumber | Int32 | Formülü doldurmak için satır sayısı. |
| columnNumber | Int32 | Formülü doldurmak için sütun sayısı. |
| seçenekler | FormulaParseOptions | Formül ayrıştırma seçenekleri. |
| değerler | Object[][] | verilen paylaşılan formülle o hücreler için değerler |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class CellMethodSetSharedFormulaWithStringInt32Int32FormulaParseOpDemo1
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluşturun ve ilk çalışma sayfasına erişin
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // A1 hücresine örnek değer ayarla
            worksheet.Cells["A1"].PutValue(5);

            // Paylaşılan formülün ayarlanacağı hedef hücre B2'yi al
            Cell cell = worksheet.Cells["B2"];

            try
            {
                // Paylaşılan formül parametrelerini tanımla
                string formula = "=A1*2";
                int totalRows = 2;
                int totalColumns = 2;
                FormulaParseOptions parseOptions = new FormulaParseOptions();
                object[][] presetValues = new object[2][]
                {
                    new object[] { 10, 10 },
                    new object[] { 10, 10 }
                };

                // B2'den başlayan 2x2 aralık için önceden ayarlanmış değerlerle paylaşılan formülü ayarla
                cell.SetSharedFormula(formula, totalRows, totalColumns, parseOptions, presetValues);

                Console.WriteLine("Shared formula set successfully. Cells B2:C3 contain values 10");
                workbook.CalculateFormula();
                Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2", "C3");
                IEnumerator iter = range.GetEnumerator();
                while(iter.MoveNext()) 
                {
                    Cell temp = (Cell)iter.Current;
                    Console.WriteLine(temp.Name + "  " + temp.Value);
                }

            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error setting shared formula: {ex.Message}");
            }

            // Değiştirilmiş çalışma kitabını kaydet
            workbook.Save("SetSharedFormulaDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [FormulaParseOptions](../../formulaparseoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


