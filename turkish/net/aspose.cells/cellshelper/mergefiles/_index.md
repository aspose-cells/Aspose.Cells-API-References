---
title: "CellsHelper.MergeFiles"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CellsHelper yöntemi. Bazı büyük xls dosyalarını bir xls dosyasına birleştirir"
type: docs
url: /tr/net/aspose.cells/cellshelper/mergefiles/
---
## CellsHelper.MergeFiles method

Bazı büyük xls dosyalarını tek bir xls dosyasına birleştirir.

```csharp
public static void MergeFiles(string[] files, string cachedFile, string destFile)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dosyalar | String[] | Dosyalar. |
| cachedFile | String | Önbellek dosyası. |
| destFile | String | Hedef dosya. |

### Açıklamalar

Bu yöntem yalnızca veri, stil ve formüllerin yeni dosyaya birleştirilmesini destekler. Önbellek dosyası bazı geçici verileri depolamak için kullanılır.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class CellsHelperMethodMergeFilesWithStringStringDemo
    {
        public static void Run()
        {
            // Geçici Excel dosyaları oluştur
            string[] filesToMerge = new string[2];
            filesToMerge[0] = "File1.xlsx";
            filesToMerge[1] = "File2.xlsx";

            // Örnek çalışma kitapları oluştur
            Workbook workbook1 = new Workbook();
            workbook1.Worksheets[0].Cells["A1"].PutValue("File 1 Content");
            workbook1.Save(filesToMerge[0]);

            Workbook workbook2 = new Workbook();
            workbook2.Worksheets[0].Cells["A1"].PutValue("File 2 Content");
            workbook2.Save(filesToMerge[1]);

            string cachedFile = "CacheFile.tmp";
            string outputFile = "MergedOutput.xlsx";

            try
            {
                // MergeFiles'i String[], String, String parametreleriyle çağır
                CellsHelper.MergeFiles(filesToMerge, cachedFile, outputFile);

                Console.WriteLine("Files merged successfully. Output saved to: " + outputFile);

                // Birleştirilmiş dosyayı doğrula
                Workbook mergedWorkbook = new Workbook(outputFile);
                Console.WriteLine("Merged content:");
                Console.WriteLine(mergedWorkbook.Worksheets[0].Cells["A1"].StringValue);
                Console.WriteLine(mergedWorkbook.Worksheets[1].Cells["A1"].StringValue);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error merging files: {ex.Message}");
            }
            finally
            {
                // Geçici dosyaları temizleyin
                if (File.Exists(filesToMerge[0])) File.Delete(filesToMerge[0]);
                if (File.Exists(filesToMerge[1])) File.Delete(filesToMerge[1]);
                if (File.Exists(cachedFile)) File.Delete(cachedFile);
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


