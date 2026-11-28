---
title: "SplitPartInfo sınıfı"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.LowCode.SplitPartInfo sınıfı. Çalışma sayfasını görüntüye dönüştürürken işlenecek mevcut sayfa gibi birden çok giriş/çıkış için bir giriş/çıkış bilgisini temsil eder."
type: docs
url: /tr/net/aspose.cells.lowcode/splitpartinfo/
---
## SplitPartInfo class

Birden fazla giriş/çıkış için bir giriş/çıkış bilgisini temsil eder, örneğin elektronik tabloyu görüntüye dönüştürürken işlenecek mevcut sayfa.

```csharp
public class SplitPartInfo
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [PartIndex](../../aspose.cells.lowcode/splitpartinfo/partindex/) { get; } | Sıradaki mevcut parçanın indeksi (0 tabanlı). -1, birden çok parça olmadığını ve sonucun tek olduğunu gösterir. |
| [SheetIndex](../../aspose.cells.lowcode/splitpartinfo/sheetindex/) { get; } | Mevcut parçanın bulunduğu sayfanın indeksi. -1, yalnızca bir sayfa olduğunu gösterir. |
| [SheetName](../../aspose.cells.lowcode/splitpartinfo/sheetname/) { get; } | Mevcut parçanın bulunduğu sayfanın adı. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeClassSplitPartInfoDemo
    {
        public static void Run()
        {
            try
            {
                // Demonstrasyon için birden çok sayfaya sahip bir çalışma kitabı oluşturun
                Workbook workbook = new Workbook();
                workbook.Worksheets.Add("Sheet1");
                workbook.Worksheets.Add("Sheet2");
                workbook.Worksheets.Add("Sheet3");

                // LowCodeLoadOptions ve LowCodeSplitOptions oluşturun
                LowCodeLoadOptions loadOptions = new LowCodeLoadOptions();
                loadOptions.InputFile = "sample.xlsx";

                LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();
                splitOptions.LoadOptions = loadOptions;

                // SplitPartInfo kullanımını göstermek için özel bir sağlayıcı oluşturun
                splitOptions.SaveOptionsProvider = new CustomSplitOptionsProvider();

                // Bölme işlemini işleyin
                SpreadsheetSplitter.Process(splitOptions);

                Console.WriteLine("Split operation completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }

    public class CustomSplitOptionsProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo partInfo)
        {
            if (partInfo == null)
            {
                throw new ArgumentNullException(nameof(partInfo));
            }

            // SplitPartInfo özelliklerine erişimi gösterin
            Console.WriteLine($"Processing part: Index={partInfo.PartIndex}, SheetIndex={partInfo.SheetIndex}, SheetName={partInfo.SheetName}");

            LowCodeSaveOptions options = new LowCodeSaveOptions();
            options.SaveFormat = SaveFormat.Xlsx;
            options.OutputFile = $"Part_{partInfo.PartIndex}_{partInfo.SheetName}.xlsx";
            return options;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


