---
title: "Cells.ImportCSV"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Bir CSV dosyasını hücrelere içe aktarır"
type: docs
url: /tr/net/aspose.cells/cells/importcsv/
---
## ImportCSV(string, string, bool, int, int) {#importcsv_3}

CSV dosyasını hücrelere içe aktar.

```csharp
public void ImportCSV(string fileName, string splitter, bool convertNumericData, int firstRow, 
    int firstColumn)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fileName | String | CSV dosya adı. |
| bölücü | String | Bölücü |
| convertNumericData | Boolean | Metin dosyasındaki dizenin sayısal veriye dönüştürülüp dönüştürülmediği. |
| firstRow | Int32 | İçe aktarılacak ilk hücrenin satır numarası. |
| firstColumn | Int32 | İçe aktarılacak ilk hücrenin sütun numarası. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodImportCSVWithStringStringBooleanInt32Int32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // CSV dosyasının yolu
            string csvPath = "example.csv";
            
            // CSV verilerini A1 hücresinden (satır 0, sütun 0) itibaren içe aktar
            // Ayırıcı olarak noktalı virgül kullanarak ve sayısal verileri dönüştürerek
            cells.ImportCSV(csvPath, ";", true, 0, 0);

            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportCSV(Stream, string, bool, int, int) {#importcsv_1}

CSV dosyasını hücrelere içe aktar.

```csharp
public void ImportCSV(Stream stream, string splitter, bool convertNumericData, int firstRow, 
    int firstColumn)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| akış | Stream | CSV dosya akışı. |
| bölücü | String | Bölücü |
| convertNumericData | Boolean | Metin dosyasındaki dizenin sayısal veriye dönüştürülüp dönüştürülmediği. |
| firstRow | Int32 | İçe aktarılacak ilk hücrenin satır numarası. |
| firstColumn | Int32 | İçe aktarılacak ilk hücrenin sütun numarası. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class CellsMethodImportCSVWithStreamStringBooleanInt32Int32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Bellekte örnek CSV verisi oluştur
            string csvData = "Name,Age,City\nJohn,30,New York\nAlice,25,London\nBob,35,Paris";
            byte[] byteArray = System.Text.Encoding.UTF8.GetBytes(csvData);
            MemoryStream csvStream = new MemoryStream(byteArray);

            try
            {
                // Stream, String, Boolean, Int32, Int32 parametreleriyle ImportCSV yöntemini çağır
                cells.ImportCSV(csvStream, ",", true, 0, 0);

                Console.WriteLine("CSV data imported successfully to worksheet.");
                Console.WriteLine($"Data range: A1 to {cells.MaxDisplayRange}");

                // Çalışma kitabını kaydedin
                workbook.Save("ImportCSVFromStreamDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error importing CSV: {ex.Message}");
            }
            finally
            {
                csvStream?.Dispose();
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportCSV(string, TxtLoadOptions, int, int) {#importcsv_2}

CSV dosyasını hücrelere içe aktar.

```csharp
public void ImportCSV(string fileName, TxtLoadOptions options, int firstRow, int firstColumn)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fileName | String | CSV dosya adı. |
| seçenekler | TxtLoadOptions | Metin dosyasını okuma için yükleme seçenekleri |
| firstRow | Int32 | İçe aktarılacak ilk hücrenin satır numarası. |
| firstColumn | Int32 | İçe aktarılacak ilk hücrenin sütun numarası. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodImportCSVWithStringTxtLoadOptionsInt32Int32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // CSV yükleme seçeneklerini oluştur
            TxtLoadOptions loadOptions = new TxtLoadOptions();
            loadOptions.Separator = ',';
            loadOptions.ConvertDateTimeData = true;
            loadOptions.ConvertNumericData = true;
            loadOptions.ParsingFormulaOnOpen = true;

            // Örnek CSV dosya yolu (ortamınızdaki gerçek yol ile değiştirin)
            string csvFilePath = "example.csv";
            
            // CSV verilerini A1 hücresinden (satır 0, sütun 0) itibaren içe aktar
            worksheet.Cells.ImportCSV(csvFilePath, loadOptions, 0, 0);

            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* class [TxtLoadOptions](../../txtloadoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportCSV(Stream, TxtLoadOptions, int, int) {#importcsv}

CSV dosyasını hücrelere içe aktar.

```csharp
public void ImportCSV(Stream stream, TxtLoadOptions options, int firstRow, int firstColumn)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| akış | Stream | CSV dosya akışı. |
| seçenekler | TxtLoadOptions | Metin dosyasını okuma için yükleme seçenekleri |
| firstRow | Int32 | İçe aktarılacak ilk hücrenin satır numarası. |
| firstColumn | Int32 | İçe aktarılacak ilk hücrenin sütun numarası. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class CellsMethodImportCSVWithStreamTxtLoadOptionsInt32Int32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];

            // Cells koleksiyonunu al
            Cells cells = worksheet.Cells;

            // Örnek CSV verisi oluştur
            string csvData = "Name,Age,City\nJohn,30,New York\nJane,25,Los Angeles\nBob,35,Chicago";

            // CSV verisiyle bir bellek akışı oluştur
            MemoryStream csvStream = new MemoryStream(System.Text.Encoding.UTF8.GetBytes(csvData));

            try
            {
                // CSV içe aktarma için TxtLoadOptions oluştur
                TxtLoadOptions loadOptions = new TxtLoadOptions();
                loadOptions.Separator = ',';
                loadOptions.ConvertNumericData = true;

                // CSV verisini satır 0, sütun 0'dan başlayarak içe aktar
                cells.ImportCSV(csvStream, loadOptions, 0, 0);

                // Çalışma kitabını kaydedin
                workbook.Save("ImportCSVDemo.xlsx");

                Console.WriteLine("CSV data imported successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error importing CSV: {ex.Message}");
            }
            finally
            {
                // Akışı serbest bırak
                csvStream.Dispose();
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [TxtLoadOptions](../../txtloadoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


