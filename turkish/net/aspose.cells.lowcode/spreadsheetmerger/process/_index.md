---
title: "SpreadsheetMerger.Process"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SpreadsheetMerger yöntemi. Verilen şablon dosyalarını birleştir"
type: docs
url: /tr/net/aspose.cells.lowcode/spreadsheetmerger/process/
---
## Process(string[], string) {#process_1}

Verilen şablon dosyalarını birleştir.

```csharp
public static void Process(string[] templateFiles, string resultFile)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| templateFiles | String[] | Birleştirilecek şablon dosyaları |
| resultFile | String | Ortaya çıkan dosya |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class SpreadsheetMergerMethodProcessWithStringArrayStringDemo
    {
        public static void Run()
        {
            // Örnek şablon dosyaları oluştur
            CreateTemplateFile("template1.xlsx", "Data from Template 1");
            CreateTemplateFile("template2.xlsx", "Data from Template 2");

            string[] templateFiles = { "template1.xlsx", "template2.xlsx" };
            string resultFile = "merged_output.xlsx";

            try
            {
                SpreadsheetMerger.Process(templateFiles, resultFile);

                Console.WriteLine($"Process method merged {templateFiles.Length} files into {resultFile}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Process method: {ex.Message}");
            }
        }

        private static void CreateTemplateFile(string fileName, string cellValue)
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].PutValue(cellValue);
            workbook.Save(fileName);
        }
    }
}
```

### Ayrıca Bakınız

* class [SpreadsheetMerger](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)

---

## Process(LowCodeMergeOptions) {#process}

Birden fazla şablon dosyasını tek bir dosyada birleştirir.

```csharp
public static void Process(LowCodeMergeOptions options)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| seçenekler | LowCodeMergeOptions | Dosyaları birleştirme seçenekleri |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class SpreadsheetMergerMethodProcessWithLowCodeMergeOptDemo
    {
        public static void Run()
        {
            // Birleştirilecek iki basit şablon dosyası hazırla.
            CreateTemplateFile("TemplateA.xlsx", "Data from Template A");
            CreateTemplateFile("TemplateB.xlsx", "Data from Template B");

            try
            {
                // Seçenek sınıfının bir örneğini oluştur.
                // LowCodeMergeOptions sınıfı Aspose.Cells.LowCode'un bir parçasıdır.
                // Bu demo için varsayılan yapıcıyı kullanıyoruz.
                LowCodeMergeOptions options = new LowCodeMergeOptions();

                // LowCodeMergeOptions kabul eden Process metodunu çağırın.
                SpreadsheetMerger.Process(options);

                Console.WriteLine("Process method invoked successfully with LowCodeMergeOptions.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Process: {ex.Message}");
            }
        }

        private static void CreateTemplateFile(string fileName, string cellValue)
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].PutValue(cellValue);
            workbook.Save(fileName);
        }
    }
}
```

### Ayrıca Bakınız

* class [LowCodeMergeOptions](../../lowcodemergeoptions/)
* class [SpreadsheetMerger](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


