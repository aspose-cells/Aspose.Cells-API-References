---
title: "Worksheet.AutoFitRow"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet yöntemi. Bir dikdörtgen aralıkta satır yüksekliğini otomatik ayarlar"
type: docs
url: /tr/net/aspose.cells/worksheet/autofitrow/
---
## AutoFitRow(int, int, int, int) {#autofitrow_3}

Dikdörtgen bir aralıktaki satır yüksekliğini otomatik olarak ayarlar.

```csharp
public void AutoFitRow(int startRow, int endRow, int startColumn, int endColumn)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startRow | Int32 | Başlangıç satır indeksi. |
| endRow | Int32 | Bitiş satır indeksi. |
| startColumn | Int32 | Başlangıç sütun indeksi. |
| endColumn | Int32 | Bitiş sütun indeksi. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorksheetMethodAutoFitRowWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            RowCollection rows = worksheet.Cells.Rows;
            rows[0].Height = 20;
            rows[1].Height = 20;
            // Satır otomatik ayarını göstermek için hücrelere örnek veri ekle
            worksheet.Cells["A1"].PutValue("This is a long text that will demonstrate row autofit");
            worksheet.Cells["B1"].PutValue("Additional column with text");
            worksheet.Cells["A2"].PutValue("Shorter text");
            worksheet.Cells["B2"].PutValue("More text");
            
            try
            {
                Console.WriteLine($"Row 1 height before autofit: {worksheet.Cells.Rows[0].Height}");
                Console.WriteLine($"Row 2 height before autofit: {worksheet.Cells.Rows[1].Height}");

                // AutoFitRow yöntemini şu parametrelerle çağır: startRow, endRow, startColumn, endColumn
                worksheet.AutoFitRow(0, 1, 0, 1);
                
                Console.WriteLine("AutoFitRow method executed successfully with parameters (0, 1, 0, 1)");
                
                // Satır yüksekliklerini göstererek etkiyi görüntüle
                Console.WriteLine($"Row 1 height after autofit: {worksheet.Cells.Rows[0].Height}");
                Console.WriteLine($"Row 2 height after autofit: {worksheet.Cells.Rows[1].Height}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AutoFitRow method: {ex.Message}");
            }
            
            // Sonucu kaydet
            workbook.Save("AutoFitRowWithInt32Int32Int32Int32Demo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitRow(int) {#autofitrow}

Satır yüksekliğini otomatik olarak ayarlar.

```csharp
public void AutoFitRow(int rowIndex)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowIndex | Int32 | Satır indeksi. |

### Açıklamalar

AutoFitRow kesin olmayan bir işlevdir.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitRowWithInt32Demo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // A1 hücresine metin kaydırma ile uzun metin ayarla
            worksheet.Cells["A1"].Value = "LOOOOOOOOOOOOOOOOOONG TEEEEEEEEEEXT";
            Style style = worksheet.Cells["A1"].GetStyle();
            style.IsTextWrapped = true;
            worksheet.Cells["A1"].SetStyle(style);

            // İlk satırı otomatik ayarla
            worksheet.AutoFitRow(0);

            // Çalışma kitabını kaydedin
            workbook.Save("AutoFitRowDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitRow(int, int, int) {#autofitrow_1}

Satır yüksekliğini otomatik olarak ayarlar.

```csharp
public void AutoFitRow(int rowIndex, int firstColumn, int lastColumn)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowIndex | Int32 | Satır indeksi. |
| firstColumn | Int32 | İlk sütun indeksi. |
| lastColumn | Int32 | Son sütun indeksi. |

### Açıklamalar

Bu yöntem, satır içindeki hücre aralığındaki içeriğe göre bir satırı otomatik ayarlar.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitRowWithInt32Int32Int32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Satır yüksekliğini etkileyecek hücrelere örnek veri ekle
            worksheet.Cells["A2"].PutValue("This is a long text that will demonstrate AutoFitRow functionality");
            worksheet.Cells["B2"].PutValue("Additional text in another column");
            
            // Satırı (satır 2) 0 ve 1 (A'dan B'ye) sütunları arasında otomatik ayarla
            worksheet.AutoFitRow(1, 0, 1);
            
            // Çalışma kitabını kaydedin
            workbook.Save("AutoFitRowDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitRow(int, int, int, AutoFitterOptions) {#autofitrow_2}

Satır yüksekliğini otomatik olarak ayarlar.

```csharp
public void AutoFitRow(int rowIndex, int firstColumn, int lastColumn, AutoFitterOptions options)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowIndex | Int32 | Satır indeksi. |
| firstColumn | Int32 | İlk sütun indeksi. |
| lastColumn | Int32 | Son sütun indeksi. |
| seçenekler | AutoFitterOptions | Otomatik ayarlayıcı seçenekleri |

### Açıklamalar

Bu yöntem, satır içindeki hücre aralığındaki içeriğe göre bir satırı otomatik ayarlar.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitRowWithInt32Int32Int32AutoFitterOptioDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Hücrelere örnek veri ekle
            worksheet.Cells["A1"].PutValue("This is a test string for autofit");
            worksheet.Cells["B1"].PutValue("Another test string in column B");
            
            // AutoFitterOptions oluştur
            AutoFitterOptions options = new AutoFitterOptions
            {
                AutoFitMergedCells = true,
                IgnoreHidden = false,
                OnlyAuto = false
            };

            // Orijinal satır yüksekliğini al
            double originalHeight = worksheet.Cells.GetRowHeight(0);
            Console.WriteLine($"Original row height: {originalHeight}");

            // İlk satırı otomatik ayarla
            worksheet.AutoFitRow(0, 0, 2, options);

            // Yeni satır yüksekliğini al
            double newHeight = worksheet.Cells.GetRowHeight(0);
            Console.WriteLine($"New row height after AutoFit: {newHeight}");

            // Çalışma kitabını kaydedin
            workbook.Save("AutoFitRowExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [AutoFitterOptions](../../autofitteroptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


