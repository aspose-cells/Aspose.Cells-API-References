---
title: "Workbook.CalculateFormula"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Workbook yöntemi. Formüllerin sonucunu hesaplar."
type: docs
url: /tr/net/aspose.cells/workbook/calculateformula/
---
## CalculateFormula() {#calculateformula}

Formüllerin sonucunu hesaplar.

```csharp
public void CalculateFormula()
```

### Açıklamalar

Desteklenen tüm formüller için lütfen https://docs.aspose.com/display/cellsnet/Supported+Formula+Functions adresindeki listeye bakın.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCalculateFormulaDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Değerleri ve formülleri ayarla.
            cells["A1"].PutValue(5);
            cells["B1"].Formula = "=A1*2";
            cells["C1"].Formula = "=B1+10";
            
            // Formülleri hesapla
            workbook.CalculateFormula();
            
            // Sonuçları göster
            Console.WriteLine("A1 value: " + cells["A1"].IntValue);
            Console.WriteLine("B1 formula result: " + cells["B1"].IntValue);
            Console.WriteLine("C1 formula result: " + cells["C1"].IntValue);
        }
    }
}
```

### Ayrıca Bakınız

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CalculateFormula(bool) {#calculateformula_2}

Formüllerin sonucunu hesaplar.

```csharp
public void CalculateFormula(bool ignoreError)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ignoreError | Boolean | Formüller hesaplanırken hatanın gizlenip gizlenmeyeceğini gösterir. Hata, desteklenmeyen işlev, dış bağlantılar vb. olabilir. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCalculateFormulaWithBooleanDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook wb = new Workbook();
            
            // İlk çalışma sayfasına ve hücrelerine erişin.
            Worksheet worksheet = wb.Worksheets[0];
            Cells cells = worksheet.Cells;

            // İlk satıra (A1:E1) değerleri koyun.
            for (int i = 0; i < 5; i++)
            {
                cells[0, i].PutValue(i + 1); // Values 1-5
            }

            // İkinci satıra (A2:E2) değerleri koyun.
            for (int i = 0; i < 5; i++)
            {
                cells[1, i].PutValue((i + 1) * 10); // Values 10,20,30,40,50
            }

            // Dördüncü satıra (A4:E4) ortak bir HLOOKUP formülü ayarlayın.
            cells[3, 0].SetSharedFormula("=HLOOKUP(A1,$A$1:$E$2,2,FALSE)", 1, 5);

            // Formülleri özyinelemeli hesaplama olmadan hesaplayın.
            wb.CalculateFormula(false);

            // Sonuçları görüntüleyin
            Console.WriteLine("Formula calculation results:");
            for (int i = 0; i < 5; i++)
            {
                Console.WriteLine($"Cell {((char)('A' + i))}4 value: {cells[3, i].StringValue}");
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

## CalculateFormula(CalculationOptions) {#calculateformula_1}

Bu çalışma kitabındaki formüller hesaplanıyor.

```csharp
public void CalculateFormula(CalculationOptions options)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| seçenekler | CalculationOptions | Hesaplama seçenekleri |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCalculateFormulaWithCalculationOptionsDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Bir tablo oluşturun ve sütun adlarını ayarlayın.
            sheet.Cells["A1"].PutValue("A");
            sheet.Cells["B1"].PutValue("B");
            sheet.Cells["A2"].PutValue(1);
            sheet.Cells["B2"].PutValue(2);
            
            // Formülleri ayarlayın ve hesaplayın.
            Cells cells = sheet.Cells;
            cells["C1"].PutValue("InvalidColumn");
            cells["D1"].Formula = "=INDIRECT(\"A\"&ROW())";
            cells["E1"].Formula = "=IFERROR(INDIRECT(\"B\"&ROW()),\"OK\")";
            
            // Seçeneklerle formülleri hesaplayın.
            wb.CalculateFormula(new CalculationOptions());
            
            // Sonuçları çıktı olarak ver
            Console.WriteLine("D1 result: " + cells["D1"].StringValue);
            Console.WriteLine("E1 result: " + cells["E1"].StringValue);
        }
    }
}
```

### Ayrıca Bakınız

* class [CalculationOptions](../../calculationoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


