---
title: "Worksheet.AutoFitRows"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet yöntemi. Bu çalışma sayfasındaki tüm satırları otomatik olarak sığdırır"
type: docs
url: /tr/net/aspose.cells/worksheet/autofitrows/
---
## AutoFitRows(AutoFitterOptions) {#autofitrows_1}

Bu çalışma sayfasındaki tüm satırları otomatik olarak ayarlar.

```csharp
public void AutoFitRows(AutoFitterOptions options)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| seçenekler | AutoFitterOptions | Otomatik ayarlayıcı seçenekleri |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitRowsWithAutoFitterOptionsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ve biçimlendirmeyi ayarla
            worksheet.Cells["A1"].PutValue("This is a long text that will need auto-fitting");
            worksheet.Cells["A2"].PutValue("Another long text\nwith multiple lines\nfor demonstration");
            
            // Birleştirilmiş hücre otomatik sığdırmayı göstermek için hücreleri birleştir
            worksheet.Cells.Merge(3, 0, 2, 1);
            worksheet.Cells["A3"].PutValue("Merged cells text that needs to fit");

            // Satırları belirli seçeneklerle otomatik sığdır
            worksheet.AutoFitRows(new AutoFitterOptions
            {
                AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine,
                AutoFitWrappedTextType = AutoFitWrappedTextType.Paragraph,
                MaxRowHeight = 100,  // Set reasonable max height
                OnlyAuto = true
            });

            // Çalışma kitabını kaydedin
            workbook.Save("AutoFitRowsDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [AutoFitterOptions](../../autofitteroptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitRows(int, int) {#autofitrows_3}

Bir aralıktaki satır yüksekliğini otomatik olarak ayarlar.

```csharp
public void AutoFitRows(int startRow, int endRow)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startRow | Int32 | Başlangıç satır indeksi. |
| endRow | Int32 | Bitiş satır indeksi. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitRowsWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            Cells cells = sheet.Cells;

            // Hücreleri örnek veri ve stillerle doldur
            for (int i = 0; i <= 8; i++)
            {
                Cell cell = cells[i, i];
                cell.Value = "Sample text for row " + i;
                
                if (i % 2 == 0)
                {
                    Style style = cell.GetStyle();
                    style.SetBorder(BorderType.BottomBorder, CellBorderType.Thin, System.Drawing.Color.Black);
                    cell.SetStyle(style);
                }
            }

            // Satırları indeks 0'dan 8'e kadar otomatik sığdır
            sheet.AutoFitRows(0, 8);

            // Ortaya çıkan satır yüksekliklerini çıktı olarak ver
            for (int i = 0; i <= 8; i++)
            {
                Console.WriteLine($"Row {i} height: {cells.GetRowHeightPixel(i)} pixels");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitRows(int, int, AutoFitterOptions) {#autofitrows_4}

Bir aralıktaki satır yüksekliğini otomatik olarak ayarlar.

```csharp
public void AutoFitRows(int startRow, int endRow, AutoFitterOptions options)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startRow | Int32 | Başlangıç satır indeksi. |
| endRow | Int32 | Bitiş satır indeksi. |
| seçenekler | AutoFitterOptions | Otomatik sığdırıcının seçenekleri. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitRowsWithInt32Int32AutoFitterOptionsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hücrelere örnek veri ekle
            worksheet.Cells["A1"].PutValue("This is a test string for auto-fit row height demonstration");
            worksheet.Cells["A2"].PutValue("Another line\nwith multiple lines\nof text");
            
            // Otomatik sığdırıcı seçenekleri oluştur
            AutoFitterOptions options = new AutoFitterOptions();
            options.OnlyAuto = true;
            
            // Satırları 0'dan 1'e kadar seçeneklerle otomatik sığdır
            worksheet.AutoFitRows(0, 1, options);
            
            // Çalışma kitabını kaydedin
            workbook.Save("AutoFitRowsDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [AutoFitterOptions](../../autofitteroptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitRows() {#autofitrows}

Bu çalışma sayfasındaki tüm satırları otomatik olarak ayarlar.

```csharp
public void AutoFitRows()
```

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitRowsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hücrelere örnek veri ekle
            worksheet.Cells["A1"].PutValue("This is a test string for AutoFitRows demonstration");
            worksheet.Cells["A2"].PutValue("Another line of text\nwith line break to show row height adjustment");
            worksheet.Cells["B1"].PutValue("Column B content");
            
            // Satırları otomatik sığdır
            worksheet.AutoFitRows();
            
            // Daha iyi görünürlük için sütunları otomatik sığdır
            worksheet.AutoFitColumns();
            
            // Çalışma kitabını kaydedin
            string outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "AutoFitRowsDemo.xlsx");
            workbook.Save(outputPath, SaveFormat.Xlsx);
            
            Console.WriteLine("Worksheet with AutoFitRows saved to: " + outputPath);
        }
    }
}
```

### Ayrıca Bakınız

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitRows(bool) {#autofitrows_2}

Bu çalışma sayfasındaki tüm satırları otomatik olarak ayarlar.

```csharp
public void AutoFitRows(bool onlyAuto)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| onlyAuto | Boolean | True, sadece satır yüksekliği özelleştirilmediğinde satır yüksekliğini otomatik sığdırır. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitRowsWithBooleanDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Satır otomatik sığdırmayı göstermek için hücrelere örnek metin ekle
            worksheet.Cells["A1"].PutValue("This is a sample text that will demonstrate AutoFitRows functionality");
            worksheet.Cells["A2"].PutValue("Another line of text\nwith line breaks\nto show multi-line row adjustment");
            
            // Otomatik birleştirme dikkate alınarak satırları otomatik sığdır
            worksheet.AutoFitRows(true);
            
            // Çalışma kitabını kaydedin
            workbook.Save("AutoFitRowsDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


