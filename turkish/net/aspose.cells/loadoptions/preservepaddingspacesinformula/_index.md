---
title: "LoadOptions.PreservePaddingSpacesInFormula"
second_title: "Aspose.Cells için .NET API Referansı"
description: "LoadOptions özelliği. Formülleri alırken ve ayarlarken formül tokenları arasında doldurulan boşlukları ve satır sonlarını koruyup korumayacağını gösterir. Varsayılan değer false'tur"
type: docs
url: /tr/net/aspose.cells/loadoptions/preservepaddingspacesinformula/
---
## LoadOptions.PreservePaddingSpacesInFormula property

Formülleri alırken ve ayarlarken formül tokenları arasında eklenen boşluk ve satır sonlarının korunup korunmayacağını gösterir. Varsayılan değer yanlıştır.

```csharp
public bool PreservePaddingSpacesInFormula { get; set; }
```

### Açıklamalar

Bu seçenekle şablon dosyasından çalışma kitabı yüklendikten sonra, [`PreservePaddingSpaces`](../../formulasettings/preservepaddingspaces/) aynı değerle bu özellik ile ayarlanacaktır.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyPreservePaddingSpacesInFormulaDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Formüllerde doldurma boşluklarını korumayı etkinleştir
            workbook.Settings.FormulaSettings.PreservePaddingSpaces = true;
            
            // İlk çalışma sayfasına eriş ve doldurma boşlukları içeren bir formül ayarla
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            string formulaWithSpaces = "= IF(1 <>2, 2, 1)";
            cell.Formula = formulaWithSpaces;
            
            // Çalışma kitabını PreservePaddingSpacesInFormula seçeneğiyle kaydet ve yeniden yükle
            string outputPath = "output.xlsx";
            workbook.Save(outputPath, SaveFormat.Xlsx);
            
            LoadOptions loadOptions = new LoadOptions(LoadFormat.Xlsx)
            {
                PreservePaddingSpacesInFormula = true
            };
            
            Workbook reloadedWorkbook = new Workbook(outputPath, loadOptions);
            Worksheet reloadedWorksheet = reloadedWorkbook.Worksheets[0];
            
            // Yeniden yükledikten sonra formülün boşlukları koruduğunu doğrula
            Console.WriteLine("Original formula: " + formulaWithSpaces);
            Console.WriteLine("Reloaded formula: " + reloadedWorksheet.Cells["A1"].Formula);
        }
    }
}
```

### Ayrıca Bakınız

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


