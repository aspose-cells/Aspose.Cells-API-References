---
title: "Workbook.Save"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Workbook yöntemi. Çalışma kitabını diske kaydeder"
type: docs
url: /tr/net/aspose.cells/workbook/save/
---
## Save(string, SaveFormat) {#save_3}

Çalışma kitabını diske kaydeder.

```csharp
public void Save(string fileName, SaveFormat saveFormat)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fileName | String | Dosya adı. |
| saveFormat | SaveFormat | Kaydetme formatı türü. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodSaveWithStringSaveFormatDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına erişin ve bazı örnek veriler ekleyin
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");

            // Çalışma kitabını XLSX formatında kaydedin
            workbook.Save("output.xlsx", SaveFormat.Xlsx);

            // Çalışma kitabını PDF formatında kaydedin
            workbook.Save("output.pdf", SaveFormat.Pdf);
        }
    }
}
```

### Ayrıca Bakınız

* enum [SaveFormat](../../saveformat/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Save(string) {#save_2}

Çalışma kitabını diske kaydeder.

```csharp
public void Save(string fileName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fileName | String |  |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodSaveWithStringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");
            
            // Çalışma kitabını dize parametresi kullanarak farklı formatlarda kaydedin
            workbook.Save("output.xlsx");
            workbook.Save("output.xls");
            workbook.Save("output.xml", SaveFormat.SpreadsheetML);
        }
    }
}
```

### Ayrıca Bakınız

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Save(string, SaveOptions) {#save_4}

Çalışma kitabını diske kaydeder.

```csharp
public void Save(string fileName, SaveOptions saveOptions)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fileName | String | Dosya adı. |
| saveOptions | SaveOptions | Kaydetme seçenekleri. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodSaveWithStringSaveOptionsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına erişin ve bazı veriler ekleyin
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World!");
            
            // HTML kaydetme seçeneklerini oluşturun ve yapılandırın
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExportImagesAsBase64 = true;
            
            // Çalışma kitabını seçeneklerle kaydedin
            workbook.Save("output.html", saveOptions);
            
            Console.WriteLine("Workbook saved successfully with HTML options.");
        }
    }
}
```

### Ayrıca Bakınız

* class [SaveOptions](../../saveoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Save(Stream, SaveFormat) {#save}

Çalışma kitabını akışa kaydeder.

```csharp
public void Save(Stream stream, SaveFormat saveFormat)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| akış | Stream | Dosya akışı. |
| saveFormat | SaveFormat | Kaydetme dosya formatı türü. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class WorkbookMethodSaveWithStreamSaveFormatDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // İlk çalışma sayfasına erişin ve bazı örnek veriler ekleyin
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Stream Save Demo";

            try
            {
                // Çalışma kitabını kaydetmek için bir bellek akışı oluşturun
                using (MemoryStream stream = new MemoryStream())
                {
                    // Çalışma kitabını akışa XLSX formatında kaydedin
                    workbook.Save(stream, SaveFormat.Xlsx);

                    // Başarı mesajını göster
                    Console.WriteLine("Workbook saved to stream successfully in XLSX format.");
                    Console.WriteLine($"Stream length: {stream.Length} bytes");

                    // İlerideki olası işleme için akış konumunu sıfırlayın
                    stream.Position = 0;

                    // Doğrulama için isteğe bağlı olarak dosyaya kaydedin
                    using (FileStream fileStream = File.Create("StreamSaveDemo.xlsx"))
                    {
                        stream.CopyTo(fileStream);
                    }
                    Console.WriteLine("Stream content also saved to file: StreamSaveDemo.xlsx");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error saving workbook to stream: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* enum [SaveFormat](../../saveformat/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Save(Stream, SaveOptions) {#save_1}

Çalışma kitabını akışa kaydeder.

```csharp
public void Save(Stream stream, SaveOptions saveOptions)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| akış | Stream | Dosya akışı. |
| saveOptions | SaveOptions | Kaydetme seçenekleri. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class WorkbookMethodSaveWithStreamSaveOptionsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // İlk çalışma sayfasına erişin ve bazı veriler ekleyin
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Hello, Aspose.Cells!";
            worksheet.Cells["B1"].Value = "Stream Save Demo";

            // Çalışma kitabını kaydetmek için bir MemoryStream oluşturun
            MemoryStream stream = new MemoryStream();

            try
            {
                // PDF formatı için SaveOptions oluşturun
                PdfSaveOptions saveOptions = new PdfSaveOptions();

                // Çalışma kitabını belirtilen seçeneklerle akışa kaydedin
                workbook.Save(stream, saveOptions);

                Console.WriteLine("Workbook saved to stream successfully in PDF format.");
                Console.WriteLine($"Stream length: {stream.Length} bytes");

                // İlerideki olası kullanım için akış konumunu sıfırla
                stream.Position = 0;
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error saving workbook: {ex.Message}");
            }
            finally
            {
                // Kaynakları temizle
                stream?.Dispose();
                workbook?.Dispose();
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [SaveOptions](../../saveoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Save(HttpResponse, string, ContentDisposition, SaveOptions) {#save_5}

Sonuç elektronik tablosunu oluşturur ve istemciye aktarır, ardından tarayıcıda veya MS Workbook'ta açar.

```csharp
public void Save(HttpResponse response, string fileName, ContentDisposition contentDisposition, 
    SaveOptions saveOptions)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| yanıt | HttpResponse | İstemciye elektronik tabloyu döndürmek için yanıt nesnesi. |
| fileName | String | Oluşturulan dosyanın adı. |
| contentDisposition | ContentDisposition | İçerik dağıtım türü. |
| saveOptions | SaveOptions | Kaydetme seçenekleri. |

### Açıklamalar

Bu yöntem yalnızca net4.x sürümleri için kullanılabilir.

### Ayrıca Bakınız

* enum [ContentDisposition](../../contentdisposition/)
* class [SaveOptions](../../saveoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Save(HttpResponse, string, ContentDisposition, SaveOptions, bool) {#save_6}

Sonuç elektronik tablosunu oluşturur ve istemciye aktarır, ardından tarayıcıda veya MS Workbook'ta açar.

```csharp
public void Save(HttpResponse response, string fileName, ContentDisposition contentDisposition, 
    SaveOptions saveOptions, bool enableHttpCompression)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| yanıt | HttpResponse | İstemciye elektronik tabloyu döndürmek için yanıt nesnesi. |
| fileName | String | Oluşturulan dosyanın adı. |
| contentDisposition | ContentDisposition | İçerik dağıtım türü. |
| saveOptions | SaveOptions | Kaydetme seçenekleri. |
| enableHttpCompression | Boolean | http sıkıştırmasının kullanılıp kullanılmayacağı |

### Açıklamalar

Bu yöntem yalnızca net4.x sürümleri için kullanılabilir.

### Ayrıca Bakınız

* enum [ContentDisposition](../../contentdisposition/)
* class [SaveOptions](../../saveoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


