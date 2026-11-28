---
title: "Workbook.MergeNamedStyles"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Workbook yöntemi. Diğer Excel dosyasından adlandırılmış stilleri birleştirir"
type: docs
url: /tr/net/aspose.cells/workbook/mergenamedstyles/
---
## Workbook.MergeNamedStyles method

Diğer Excel dosyasından adlandırılmış stilleri birleştirir.

```csharp
public void MergeNamedStyles(Workbook source)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| kaynak | Çalışma Kitabı | Diğer dosya |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodMergeNamedStylesWithWorkbookDemo
    {
        public static void Run()
        {
            // Hedef çalışma kitabını oluştur (adlandırılmış stilleri alacak olan)
            using (Workbook targetWorkbook = new Workbook())
            {
                // Bağlam için hedef çalışma kitabına bazı veriler ekle
                Worksheet targetSheet = targetWorkbook.Worksheets[0];
                targetSheet.Cells["A1"].PutValue("Target Workbook");

                // Kaynak çalışma kitabını oluştur (birleştirilecek adlandırılmış stilleri içeren)
                using (Workbook sourceWorkbook = new Workbook())
                {
                    // Bağlam için kaynak çalışma kitabına bazı veriler ekle
                    Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
                    sourceSheet.Cells["A1"].PutValue("Source Workbook");

                    try
                    {
                        // sourceWorkbook'dan targetWorkbook'a adlandırılmış stilleri birleştir
                        targetWorkbook.MergeNamedStyles(sourceWorkbook);

                        Console.WriteLine("MergeNamedStyles executed successfully.");

                        // Sonuçta oluşan çalışma kitabını kaydet
                        string outputPath = "MergedNamedStylesDemo.xlsx";
                        targetWorkbook.Save(outputPath, SaveFormat.Xlsx);
                        Console.WriteLine($"Workbook saved to '{outputPath}'.");
                    }
                    catch (Exception ex)
                    {
                        Console.WriteLine($"Error during MergeNamedStyles: {ex.Message}");
                    }
                }
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


