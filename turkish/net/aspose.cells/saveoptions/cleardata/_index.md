---
title: "SaveOptions.ClearData"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SaveOptions özelliği. Dosya kaydedildikten sonra çalışma kitabını boş bırakır"
type: docs
url: /tr/net/aspose.cells/saveoptions/cleardata/
---
## SaveOptions.ClearData property

Dosya kaydedildikten sonra çalışma kitabını boş bırak.

```csharp
public bool ClearData { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertyClearDataDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Test verileri ekleyin
            worksheet.Cells["A1"].PutValue("Tabelle1");
            worksheet.Cells["B3"].PutValue(3);

            // ClearData = false ile kaydetme seçeneklerini yapılandırın
            TxtSaveOptions saveOptions = new TxtSaveOptions();
            saveOptions.ClearData = false;
            saveOptions.Separator = ',';

            // Çalışma kitabını kaydedin
            string outputPath = "output_with_cleardata_false.csv";
            workbook.Save(outputPath, saveOptions);

            // Verinin korunduğunu doğrulamak için yeniden yükleyin
            Workbook loadedWorkbook = new Workbook(outputPath);
            Cells cells = loadedWorkbook.Worksheets[0].Cells;
            
            Console.WriteLine("A1 value: " + cells["A1"].StringValue);
            Console.WriteLine("B3 value: " + cells["B3"].IntValue);
        }
    }
}
```

### Ayrıca Bakınız

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


