---
title: "DocxSaveOptions.SaveAsEditableShapes"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DocxSaveOptions özelliği. Tüm çizim nesnelerini Word dosyasında düzenlenebilir şekiller olarak kaydeder, böylece Word'de düzenleyebilirsiniz"
type: docs
url: /tr/net/aspose.cells/docxsaveoptions/saveaseditableshapes/
---
## DocxSaveOptions.SaveAsEditableShapes property

Tüm çizim nesnelerini Word dosyasında düzenlenebilir şekiller olarak kaydedin, böylece Word'de düzenleyebilirsiniz.

```csharp
public bool SaveAsEditableShapes { get; set; }
```

### Açıklamalar

Yalnızca grafikler için.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DocxSaveOptionsPropertySaveAsEditableShapesDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // İlk çalışma sayfasına erişin ve örnek veri ekleyin
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Editable Shapes Demo";

            try
            {
                // DocxSaveOptions'ı başlatın
                DocxSaveOptions saveOptions = new DocxSaveOptions();

                // SaveAsEditableShapes özelliğinin varsayılan değerini göster
                Console.WriteLine("Default SaveAsEditableShapes value: " + saveOptions.SaveAsEditableShapes);

                // Kullanımını göstermek için SaveAsEditableShapes'ı true olarak ayarla
                saveOptions.SaveAsEditableShapes = true;
                Console.WriteLine("SaveAsEditableShapes set to: " + saveOptions.SaveAsEditableShapes);

                // Çalışma kitabını yapılandırılmış seçeneklerle DOCX olarak kaydedin
                workbook.Save("SaveAsEditableShapesDemo.docx", saveOptions);
                Console.WriteLine("Document saved successfully with SaveAsEditableShapes option.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [DocxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


