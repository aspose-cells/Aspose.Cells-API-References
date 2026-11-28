---
title: "DocxSaveOptions.SaveAsEditableShaps"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DocxSaveOptions özelliği. Tüm çizim nesnelerini word dosyasında düzenlenebilir şekiller olarak kaydeder. Böylece Word'de düzenleyebilirsiniz"
type: docs
url: /tr/net/aspose.cells/docxsaveoptions/saveaseditableshaps/
---
## DocxSaveOptions.SaveAsEditableShaps property

Tüm çizim nesnelerini word dosyasında düzenlenebilir şekiller olarak kaydet. Böylece Word'de düzenleyebilirsiniz.

```csharp
[Obsolete("Use SaveFormat.SaveAsEditableShapes instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool SaveAsEditableShaps { get; set; }
```

### Açıklamalar

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen [`SaveAsEditableShapes`](../saveaseditableshapes/) özelliğini kullanın. Bu özellik Mayıs 2025'ten itibaren 6 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DocxSaveOptionsPropertySaveAsEditableShapsDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı nesnesi oluşturun ve şablon Excel dosyasını açın
            Workbook workbook = new Workbook("example.xlsx");

            // DocxSaveOptions'ı başlatın
            DocxSaveOptions saveOptions = new DocxSaveOptions();
            
            // SaveAsEditableShaps özelliğini true olarak ayarlayın
            saveOptions.SaveAsEditableShaps = true;

            // Çalışma kitabını belirtilen seçeneklerle DOCX olarak kaydedin
            workbook.Save("example.docx", saveOptions);
        }
    }
}
```

### Ayrıca Bakınız

* class [DocxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


