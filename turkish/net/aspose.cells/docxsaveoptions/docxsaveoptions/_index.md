---
title: "DocxSaveOptions.DocxSaveOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DocxSaveOptions yapıcı. .docx dosyasını kaydetme seçeneklerini temsil eder"
type: docs
url: /tr/net/aspose.cells/docxsaveoptions/docxsaveoptions/
---
## DocxSaveOptions() {#constructor}

.docx dosyasını kaydetme seçeneklerini temsil eder.

```csharp
public DocxSaveOptions()
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DocxSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına erişin ve örnek veri ekleyin
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");
            
            // Yapıcıyı kullanarak DocxSaveOptions'ı başlatın
            DocxSaveOptions saveOptions = new DocxSaveOptions();
            saveOptions.SaveAsEditableShaps = true;
            
            // Çalışma kitabını seçeneklerle DOCX olarak kaydedin
            workbook.Save("output.docx", saveOptions);
            
            Console.WriteLine("Document saved successfully with DocxSaveOptions.");
        }
    }
}
```

### Ayrıca Bakınız

* class [DocxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DocxSaveOptions(bool) {#constructor_1}

.docx dosyasını kaydetme seçeneklerini temsil eder.

```csharp
public DocxSaveOptions(bool saveAsImage)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| saveAsImage | Boolean | Eğer True ise, çalışma kitabı .docx dosyasının bazı resimlerine dönüştürülecek. Eğer False ise, çalışma kitabı .docx dosyasının bazı tablolarına dönüştürülecek. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DocxSaveOptionsMethodCtorWithBooleanDemo
    {
        public static void Run()
        {
            // Örnek verilerle yeni bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World!");
            
            // DOCX olarak varsayılan seçeneklerle kaydet
            workbook.Save("output_default.docx");
            
            // DOCX olarak DocxSaveOptions(true) ile kaydet - MS Word için optimize edilmiştir
            workbook.Save("output_optimized.docx", new DocxSaveOptions(true));
        }
    }
}
```

### Ayrıca Bakınız

* class [DocxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


