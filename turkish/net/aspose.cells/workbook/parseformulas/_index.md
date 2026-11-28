---
title: "Workbook.ParseFormulas"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Workbook yöntemi. Şablon dosyasından yüklendiğinde veya bir hücreye ayarlandığında henüz ayrıştırılmamış tüm formülleri ayrıştırır"
type: docs
url: /tr/net/aspose.cells/workbook/parseformulas/
---
## Workbook.ParseFormulas method

Şablon dosyasından yüklendiğinde veya bir hücreye ayarlandığında ayrılmamış tüm formülleri ayrıştırır.

```csharp
public void ParseFormulas(bool ignoreError)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ignoreError | Boolean | Geçersiz formül için hatanın göz ardı edilip edilmeyeceği. Tek bir geçersiz formül için, hata göz ardı edilirse bu formül atlanır ve işlem diğer formülleri ayrıştırmaya devam eder, aksi takdirde istisna fırlatılır. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodParseFormulasWithBooleanDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook wb = new Workbook();
            Worksheet worksheet = wb.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Formülleri ayrıştırmadan ayarla (Parse = false)
            for (int i = 1; i < 10; i++)
            {
                cells[i, 0].SetFormula($"=SUM(A{i}:B{i})", new FormulaParseOptions() { Parse = false }, null);
            }

            Console.WriteLine("Formulas set without parsing. Now parsing them all at once...");

            // Tüm formülleri bir kerede ayrıştır
            wb.ParseFormulas(false);

            // Formülleri doğrula
            for (int i = 1; i < 10; i++)
            {
                Console.WriteLine($"Cell A{i} formula: {cells[i, 0].Formula}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


