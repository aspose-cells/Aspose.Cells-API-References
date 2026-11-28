---
title: "FileFormatUtil.DetectFileFormat"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FileFormatUtil yöntemi. Bir akışta depolanan Excel'in formatı hakkında bilgiyi algılar ve döndürür"
type: docs
url: /tr/net/aspose.cells/fileformatutil/detectfileformat/
---
## DetectFileFormat(Stream) {#detectfileformat}

Bir akışta depolanan Excel'in formatı hakkında bilgiyi algılar ve döndürür.

```csharp
public static FileFormatInfo DetectFileFormat(Stream stream)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| akış | Stream |  |

### Dönüş Değeri

Algılanan bilgileri içeren bir [`FileFormatInfo`](../../fileformatinfo/) nesnesi.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class FileFormatUtilMethodDetectFileFormatWithStreamDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Çalışma kitabı verileriyle bir MemoryStream hazırlayın
            using (MemoryStream stream = new MemoryStream())
            {
                // Çalışma kitabını XLSX biçiminde akışa kaydedin
                workbook.Save(stream, SaveFormat.Xlsx);
                stream.Seek(0, SeekOrigin.Begin); // Reset stream position

                try
                {
                    // Akıştan dosya biçimini algıla
                    FileFormatInfo fileFormatInfo = FileFormatUtil.DetectFileFormat(stream);
                    
                    // Algılama sonuçlarını göster
                    Console.WriteLine($"Detected File Format Type: {fileFormatInfo.FileFormatType}");
                    Console.WriteLine($"Is Encrypted: {fileFormatInfo.IsEncrypted}");
                }
                catch (Exception ex)
                {
                    Console.WriteLine($"Error detecting file format: {ex.Message}");
                }
            }

            // Doğrulama için orijinal çalışma kitabını kaydedin
            workbook.Save("DetectFileFormatWithStreamDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [FileFormatInfo](../../fileformatinfo/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DetectFileFormat(Stream, string) {#detectfileformat_1}

Bir akışta depolanan Excel'in formatı hakkında bilgiyi algılar ve döndürür.

```csharp
public static FileFormatInfo DetectFileFormat(Stream stream, string password)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| akış | Stream |  |
| parola | String | Şifreli ooxml dosyaları için parola. |

### Dönüş Değeri

Algılanan bilgileri içeren bir [`FileFormatInfo`](../../fileformatinfo/) nesnesi.

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFormatUtilMethodDetectFileFormatWithStreamStringDemo
    {
        public static void Run()
        {
            string sourcePath = "example.xlsx";
            
            using (Stream stream = File.OpenRead(sourcePath))
            {
                FileFormatInfo info = FileFormatUtil.DetectFileFormat(stream, "test");
                Console.WriteLine("File format: " + info.FileFormatType);
                Console.WriteLine("Is encrypted: " + info.IsEncrypted);
                Console.WriteLine("Is password valid: " + FileFormatUtil.VerifyPassword(stream, "test"));
            }

            using (Stream stream = File.OpenRead(sourcePath))
            {
                FileFormatInfo info = FileFormatUtil.DetectFileFormat(stream, "1234");
                Console.WriteLine("File format: " + info.FileFormatType);
                Console.WriteLine("Is encrypted: " + info.IsEncrypted);
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [FileFormatInfo](../../fileformatinfo/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DetectFileFormat(string) {#detectfileformat_2}

Bir dosyada depolanan Excel'in formatı hakkında bilgiyi algılar ve döndürür.

```csharp
public static FileFormatInfo DetectFileFormat(string filePath)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| filePath | String | Dosya yolu. |

### Dönüş Değeri

Algılanan bilgileri içeren bir [`FileFormatInfo`](../../fileformatinfo/) nesnesi.

### Açıklamalar

Yalnızca sihirli imzaya sahip bazı dosyaları kontrol etmeyi destekler. Eğer sihirli imza yoksa, dosya biçimini kesin olarak tespit edemeyiz.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFormatUtilMethodDetectFileFormatWithStringDemo
    {
        public static void Run()
        {
            string filePath = "example.xlsx";
            FileFormatInfo info = FileFormatUtil.DetectFileFormat(filePath);
            
            Console.WriteLine("Load Format: " + info.LoadFormat);
            Console.WriteLine("File Format Type: " + info.FileFormatType);
            
            SaveFormat saveFormat = FileFormatUtil.FileFormatToSaveFormat(info.FileFormatType);
            LoadFormat loadFormat = FileFormatUtil.SaveFormatToLoadFormat(saveFormat);
            
            Console.WriteLine("Save Format: " + saveFormat);
            Console.WriteLine("Load Format (converted): " + loadFormat);
        }
    }
}
```

### Ayrıca Bakınız

* class [FileFormatInfo](../../fileformatinfo/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DetectFileFormat(string, string) {#detectfileformat_3}

Bir dosyada depolanan Excel'in formatı hakkında bilgiyi algılar ve döndürür.

```csharp
public static FileFormatInfo DetectFileFormat(string filePath, string password)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| filePath | String | Dosya yolu. |
| parola | String | Şifreli ooxml dosyaları için parola. |

### Dönüş Değeri

Algılanan bilgileri içeren bir [`FileFormatInfo`](../../fileformatinfo/) nesnesi.

### Açıklamalar

Yalnızca sihirli imzaya sahip bazı dosyaları kontrol etmeyi destekler. Eğer sihirli imza yoksa, dosya biçimini kesin olarak tespit edemeyiz.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFormatUtilMethodDetectFileFormatWithStringStringDemo
    {
        public static void Run()
        {
            string sourcePath = @"..\..\..\Data\";
            
            // XLSX dosya biçimini algıla
            FileFormatInfo xlsxInfo = FileFormatUtil.DetectFileFormat(sourcePath + "example.xlsx", "password");
            Console.WriteLine("XLSX format: " + xlsxInfo.FileFormatType);

            // DOCX dosya biçimini algıla
            FileFormatInfo docxInfo = FileFormatUtil.DetectFileFormat(sourcePath + "example.docx", "password");
            Console.WriteLine("DOCX format: " + docxInfo.FileFormatType);
        }
    }
}
```

### Ayrıca Bakınız

* class [FileFormatInfo](../../fileformatinfo/)
* class [FileFormatUtil](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


