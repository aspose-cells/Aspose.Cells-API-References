---
title: "SplitPartInfo.PartIndex"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SplitPartInfo özelliği. Sıra0 tabanlı geçerli parçanın indeksi. 1, birden fazla parça olmadığını ve sonucun tek olduğunu gösterir"
type: docs
url: /tr/net/aspose.cells.lowcode/splitpartinfo/partindex/
---
## SplitPartInfo.PartIndex property

Sıradaki mevcut parçanın indeksi (0 tabanlı). -1, birden çok parça olmadığını ve sonucun tek olduğunu gösterir.

```csharp
public int PartIndex { get; }
```

### Açıklamalar

Birden fazla sayfanın işlenmesi gerektiğinde ve her sayfa ayrı ayrı (bölünerek) işlendiğinde, parça indeksi her sayfa için her zaman 0'dan başlar. Örneğin, çalışma kitabı görüntülere dönüştürülürken, bu, şu anda işlenen sayfanın çıktı sayfa indeksini temsil eder. Ve -1, mevcut sayfa için yalnızca bir sayfa olduğunu gösterir.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class SplitPartInfoPropertyPartIndexDemo
    {
        public static void Run()
        {
            try
            {
                // Birden fazla sayfaya sahip bir çalışma kitabı oluştur
                Workbook workbook = new Workbook();
                workbook.Worksheets.Add("Sheet1");
                workbook.Worksheets.Add("Sheet2");
                workbook.Worksheets.Add("Sheet3");

                // Bölme işlemiyle kullanmak için çalışma kitabını kaydet
                workbook.Save("sample.xlsx");

                // Yükleme seçenekleri oluştur
                LowCodeLoadOptions loadOptions = new LowCodeLoadOptions();
                loadOptions.InputFile = "sample.xlsx";

                // Özel sağlayıcı ile bölme seçenekleri oluştur
                LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();
                splitOptions.LoadOptions = loadOptions;
                splitOptions.SaveOptionsProvider = new CustomPartIndexProvider();

                // Bölme işlemini işleyin
                SpreadsheetSplitter.Process(splitOptions);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }

    public class CustomPartIndexProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo partInfo)
        {
            if (partInfo == null)
            {
                throw new ArgumentNullException(nameof(partInfo));
            }

            // PartIndex özelliğini okuma örneği göster
            Console.WriteLine($"Current part PartIndex: {partInfo.PartIndex}");
            Console.WriteLine($"Current part SheetIndex: {partInfo.SheetIndex}");
            Console.WriteLine($"Current part SheetName: {partInfo.SheetName}");

            LowCodeSaveOptions options = new LowCodeSaveOptions();
            options.SaveFormat = SaveFormat.Xlsx;
            options.OutputFile = $"Part_{partInfo.PartIndex}_{partInfo.SheetName}.xlsx";
            return options;
        }
    }
}
```

### Ayrıca Bakınız

* class [SplitPartInfo](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


