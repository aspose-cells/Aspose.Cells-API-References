---
title: "Workbook.Workbook"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Workbook yapıcı. Workbook sınıfının yeni bir örneğini başlatır"
type: docs
url: /tr/net/aspose.cells/workbook/workbook/
---
## Workbook() {#constructor}

[`Workbook`](../) sınıfının yeni bir örneğini başlatır.

```csharp
public Workbook()
```

### Açıklamalar

Varsayılan dosya formatı Xlsx'tir. Başka dosya türleri oluşturmak istiyorsanız, lütfen Workbook(FileFormatType) kullanın.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCtorDemo
    {
        public static void Run()
        {
            // Yapıcıyı kullanarak yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hücrelere bazı veriler ekleyin
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");
            
            // Çalışma kitabını kaydedin
            workbook.Save("WorkbookCtorDemo.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("Workbook created and saved successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Workbook(FileFormatType) {#constructor_1}

[`Workbook`](../) sınıfının yeni bir örneğini başlatır.

```csharp
public Workbook(FileFormatType fileFormatType)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fileFormatType | FileFormatType | Yeni dosya formatı. |

### Açıklamalar

Varsayılan dosya formatı Excel97To2003'tür.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCtorWithFileFormatTypeDemo
    {
        public static void Run()
        {
            // XLSX dosya formatı ile yeni bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook(FileFormatType.Xlsx);
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // A1 hücresine bazı veriler ekleyin
            worksheet.Cells["A1"].PutValue("Hello World!");
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* enum [FileFormatType](../../fileformattype/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Workbook(LoadOptions) {#constructor_2}

Seçeneklerle [`Workbook`](../) sınıfının yeni boş bir örneğini başlatır

```csharp
public Workbook(LoadOptions loadOptions)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| loadOptions | LoadOptions | Seçenekler. |

### Ayrıca Bakınız

* class [LoadOptions](../../loadoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Workbook(string) {#constructor_5}

Yeni bir [`Workbook`](../) sınıfı örneği başlatır ve bir dosya açar.

```csharp
public Workbook(string file)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dosya | String | Dosya adı. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCtorWithStringDemo
    {
        public static void Run()
        {
            // Belgeler dizinine giden yol.
            string dataDir = "Your Document Directory";

            // Mevcut bir Excel dosyasından bir Workbook oluşturun
            Workbook workbook = new Workbook(dataDir + "example.xlsx");

            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];

            // Bazı çalışma sayfası bilgilerini gösterin
            Console.WriteLine("Worksheet Name: " + worksheet.Name);
            Console.WriteLine("Number of Cells: " + worksheet.Cells.Count);

            // Çalışma kitabını MHTML formatında kaydedin
            workbook.Save(dataDir + "output.mht", SaveFormat.MHtml);

            // Kaydedilen MHTML dosyasından başka bir Workbook oluşturun
            Workbook workbook2 = new Workbook(dataDir + "output.mht");
            Console.WriteLine("Number of Worksheets in MHTML: " + workbook2.Worksheets.Count);
        }
    }
}
```

### Ayrıca Bakınız

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Workbook(Stream) {#constructor_3}

Yeni bir [`Workbook`](../) sınıfı örneği başlatır ve bir akış açar.

```csharp
public Workbook(Stream stream)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| akış | Stream | Akış. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class WorkbookMethodSharpctorWithStreamDemo
    {
        public static void Run()
        {
            // Bellekte örnek bir Excel dosyası oluşturun
            MemoryStream sampleStream = new MemoryStream();
            Workbook sampleWorkbook = new Workbook();
            sampleWorkbook.Worksheets[0].Cells["A1"].Value = "Sample Data";
            sampleWorkbook.Save(sampleStream, SaveFormat.Xlsx);
            sampleStream.Position = 0; // Reset stream position for reading

            try
            {
                // Stream yapıcıyı kullanarak yeni bir Workbook örneği oluşturun
                Workbook workbook = new Workbook(sampleStream);

                // İlk çalışma sayfasına eriş
                Worksheet worksheet = workbook.Worksheets[0];

                // Yüklenen verileri görüntüleyin
                Console.WriteLine($"Loaded data from stream: {worksheet.Cells["A1"].StringValue}");

                // Çalışma kitabını bir dosyaya kaydedin
                workbook.Save("WorkbookFromStream.xlsx");
                Console.WriteLine("Workbook saved successfully from stream.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error loading workbook from stream: {ex.Message}");
            }
            finally
            {
                sampleStream.Dispose();
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Workbook(string, LoadOptions) {#constructor_6}

Yeni bir [`Workbook`](../) sınıfı örneği başlatır ve bir dosya açar.

```csharp
public Workbook(string file, LoadOptions loadOptions)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dosya | String | Dosya adı. |
| loadOptions | LoadOptions | Yükleme seçenekleri |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCtorWithStringLoadOptionsDemo
    {
        public static void Run()
        {
            // LightCellsDataHandler olmadan yükleme seçenekleri oluşturun
            LoadOptions loadOptions = new LoadOptions();

            // Çalışma kitabını dosya yolu ve yükleme seçenekleriyle başlatın
            Workbook workbook = new Workbook("sample.xlsx", loadOptions);

            // Çalışma sayfası sayısına erişerek workbook'un yüklendiğini gösterin
            Console.WriteLine("Number of worksheets: " + workbook.Worksheets.Count);
        }
    }
}
```

### Ayrıca Bakınız

* class [LoadOptions](../../loadoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Workbook(Stream, LoadOptions) {#constructor_4}

Yeni bir [`Workbook`](../) sınıfı örneği başlatır ve akışı açar.

```csharp
public Workbook(Stream stream, LoadOptions loadOptions)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| akış | Stream | Akış. |
| loadOptions | LoadOptions | Yükleme seçenekleri |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class WorkbookMethodSharpctorWithStreamLoadOptionsDemo
    {
        public static void Run()
        {
            try
            {
                // Bellekte örnek bir Excel dosyası oluşturun
                byte[] sampleExcelData = GetSampleExcelData();
                MemoryStream stream = new MemoryStream(sampleExcelData);

                // Belirli ayarlarla LoadOptions oluşturun
                LoadOptions loadOptions = new LoadOptions(LoadFormat.Xlsx);
                loadOptions.MemorySetting = MemorySetting.MemoryPreference;

                // #ctor ile Stream ve LoadOptions kullanarak bir Workbook örneği oluşturun
                Workbook workbook = new Workbook(stream, loadOptions);

                // Yüklenen workbook hakkında temel bilgileri gösterin
                Console.WriteLine("Workbook loaded successfully!");
                Console.WriteLine("Number of worksheets: " + workbook.Worksheets.Count);
                Console.WriteLine("File format: " + workbook.FileFormat);

                // İlk çalışma sayfasına eriş
                Worksheet worksheet = workbook.Worksheets[0];
                Console.WriteLine("First worksheet name: " + worksheet.Name);

                // Mevcutsa bazı hücre içeriğini göster
                if (worksheet.Cells["A1"].Value != null)
                {
                    Console.WriteLine("Cell A1 value: " + worksheet.Cells["A1"].Value.ToString());
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error loading workbook: {ex.Message}");
            }
        }

        private static byte[] GetSampleExcelData()
        {
            // Demonstrasyon için hafızada basit bir Excel dosyası oluştur
            using (MemoryStream ms = new MemoryStream())
            {
                Workbook tempWorkbook = new Workbook();
                tempWorkbook.Worksheets[0].Cells["A1"].PutValue("Sample Data");
                tempWorkbook.Worksheets[0].Cells["B1"].PutValue("Created for demo");
                tempWorkbook.Save(ms, SaveFormat.Xlsx);
                return ms.ToArray();
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [LoadOptions](../../loadoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


