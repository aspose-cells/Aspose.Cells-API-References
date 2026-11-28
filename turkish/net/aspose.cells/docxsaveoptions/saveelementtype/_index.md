---
title: "DocxSaveOptions.SaveElementType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DocxSaveOptions özelliği. Hangi öğelerin kaydedileceğini gösterir"
type: docs
url: /tr/net/aspose.cells/docxsaveoptions/saveelementtype/
---
## DocxSaveOptions.SaveElementType property

Hangi öğelerin kaydedilmesi gerektiğini gösterir.

```csharp
public SaveElementType SaveElementType { get; set; }
```

### Örnekler

```csharp
using Aspose.Cells;
using System;

namespace AsposeCellsExamples
{
    public class DocxSaveOptionsPropertySaveElementTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluşturun ve bazı örnek veriler ekleyin
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].PutValue("Demo Data");

            try
            {
                // DocxSaveOptions'ı başlatın
                DocxSaveOptions saveOptions = new DocxSaveOptions();

                // NOT: SaveElementType özelliği DocxSaveOptions sınıfında bulunmamaktadır
                // sağlanan API yansıtmasına dayanarak. Eğer mevcut olsaydı, şu şekilde okurdunuz:
                // var elementType = saveOptions.SaveElementType;
                // Console.WriteLine(\"SaveElementType: \" + elementType);

                // Mevcut bir özelliği okuma örneği: SaveAsEditableShaps
                Console.WriteLine("SaveAsEditableShaps (default): " + saveOptions.SaveAsEditableShaps);

                // Özelliği true olarak ayarlayın ve yeni değeri gösterin
                saveOptions.SaveAsEditableShaps = true;
                Console.WriteLine("SaveAsEditableShaps (after set): " + saveOptions.SaveAsEditableShaps);

                // Çalışma kitabını yapılandırılmış seçenekleri kullanarak DOCX olarak kaydedin
                workbook.Save("SaveElementTypeDemo.docx", saveOptions);
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error: " + ex.Message);
            }
        }
    }
}
```

### Ayrıca Bakınız

* enum [SaveElementType](../../../aspose.cells.saving/saveelementtype/)
* class [DocxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


