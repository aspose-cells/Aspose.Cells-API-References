---
title: "HtmlSaveOptions.CellNameAttribute"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HtmlSaveOptions özelliği. Yazılacak CellName'i belirten özniteliği tanımlar. Örneğin, değer id ise A1 hücresi için çıktı td idA1 olur. Varsayılan değer null'dur"
type: docs
url: /tr/net/aspose.cells/htmlsaveoptions/cellnameattribute/
---
## HtmlSaveOptions.CellNameAttribute property

Yazılacak CellName'i belirten özniteliği belirtir. (ör. Değer "id" ise, "A1" hücresi için çıktı &lt;td id='A1'&gt; olur). Varsayılan değer null'dur.

```csharp
public string CellNameAttribute { get; set; }
```

### Örnekler

```csharp
using System;
using System.IO;
using System.Text.RegularExpressions;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyCellNameAttributeDemo
    {
        public static void Run()
        {
            // Bazı verilerle örnek bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Data");
            worksheet.Cells["B2"].PutValue(123);

            // CellNameAttribute özelliği ile HTML kaydetme seçeneklerini ayarlayın
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.CellNameAttribute = "id";
            saveOptions.ExportImagesAsBase64 = true;
            saveOptions.ExportActiveWorksheetOnly = true;

            // HTML dosyasına kaydedin
            string outputPath = "output.html";
            workbook.Save(outputPath, saveOptions);

            // HTML çıktısının hücre kimliklerini içerdiğini doğrulayın
            string htmlContent = File.ReadAllText(outputPath);
            Console.WriteLine("HTML contains A1 cell with ID: " + Regex.IsMatch(htmlContent, @"<td\s+id='A1'"));
            Console.WriteLine("HTML contains B2 cell with ID: " + Regex.IsMatch(htmlContent, @"<td\s+id='B2'"));
        }
    }
}
```

### Ayrıca Bakınız

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


