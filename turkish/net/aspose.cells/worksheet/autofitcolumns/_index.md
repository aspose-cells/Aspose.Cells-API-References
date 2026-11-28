---
title: "Worksheet.AutoFitColumns"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet yöntemi. Bu çalışma sayfasındaki tüm sütunları otomatik olarak sığdırır"
type: docs
url: /tr/net/aspose.cells/worksheet/autofitcolumns/
---
## AutoFitColumns() {#autofitcolumns}

Bu çalışma sayfasındaki tüm sütunları otomatik olarak ayarlar.

```csharp
public void AutoFitColumns()
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitColumnsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hücrelere örnek veri ekle
            worksheet.Cells["A1"].PutValue("This is a test string");
            worksheet.Cells["B1"].PutValue("Another longer test string for demonstration");
            worksheet.Cells["C1"].PutValue("Short");
            
            // Çalışma sayfasındaki tüm sütunları otomatik sığdır
            worksheet.AutoFitColumns();
            
            // Çalışma kitabını kaydedin
            workbook.Save("AutoFitColumnsDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitColumns(AutoFitterOptions) {#autofitcolumns_1}

Bu çalışma sayfasındaki tüm sütunları otomatik olarak ayarlar.

```csharp
public void AutoFitColumns(AutoFitterOptions options)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| seçenekler | AutoFitterOptions | Otomatik sığdırma seçenekleri |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitColumnsWithAutoFitterOptionsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hücrelere örnek veri ekle
            worksheet.Cells["A1"].PutValue("Sample Text for AutoFit");
            worksheet.Cells["B1"].PutValue("Longer Sample Text for Testing AutoFitColumns");
            worksheet.Cells["C1"].PutValue(12345.6789);
            
            // Otomatik sığdırıcı seçenekleri oluştur
            AutoFitterOptions options = new AutoFitterOptions();
            options.FormatStrategy = CellValueFormatStrategy.DisplayStyle;
            
            // Seçeneklerle sütunları otomatik sığdır
            worksheet.AutoFitColumns(options);
            
            // Çalışma kitabını kaydedin
            workbook.Save("AutoFitColumnsWithOptions.xlsx");
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

## AutoFitColumns(int, int) {#autofitcolumns_2}

Sütun genişliklerini otomatik olarak ayarlar.

```csharp
public void AutoFitColumns(int firstColumn, int lastColumn)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| firstColumn | Int32 | İlk sütun indeksi. |
| lastColumn | Int32 | Son sütun indeksi. |

### Açıklamalar

AutoFitColumn, kesin olmayan bir işlevdir.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitColumnsWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Otomatik sığdırmayı göstermek için örnek veri ekle
            sheet.Cells["A1"].PutValue("Short");
            sheet.Cells["B1"].PutValue("Medium length text");
            sheet.Cells["C1"].PutValue("Very very long text that needs column width adjustment");
            sheet.Cells["D1"].PutValue("Another example with different length");

            // Sütunları 0'dan 3'e kadar otomatik sığdır
            sheet.AutoFitColumns(0, 3);

            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitColumns(int, int, AutoFitterOptions) {#autofitcolumns_3}

Sütun genişliklerini otomatik olarak ayarlar.

```csharp
public void AutoFitColumns(int firstColumn, int lastColumn, AutoFitterOptions options)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| firstColumn | Int32 | İlk sütun indeksi. |
| lastColumn | Int32 | Son sütun indeksi. |
| seçenekler | AutoFitterOptions | Otomatik sığdırma seçenekleri |

### Açıklamalar

AutoFitColumn, kesin olmayan bir işlevdir.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorksheetMethodAutoFitColumnsWithInt32Int32AutoFitterOptionsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Hücrelere örnek veri ekle
            worksheet.Cells["A1"].PutValue("Short text");
            worksheet.Cells["B1"].PutValue("This is a much longer text that needs column autofitting");
            worksheet.Cells["C1"].PutValue("Another example with different length");

            // Belirli ayarlarla AutoFitterOptions oluştur
            AutoFitterOptions options = new AutoFitterOptions();
            options.AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine;
            options.IgnoreHidden = false;
            options.OnlyAuto = false;

            try
            {
                // AutoFitColumns'ı (firstColumn, lastColumn, options) parametreleriyle çağır
                worksheet.AutoFitColumns(0, 2, options);
                
                Console.WriteLine("AutoFitColumns method executed successfully with parameters (Int32, Int32, AutoFitterOptions)");
                
                // Sütun genişliklerini göstererek etkiyi görüntüle
                Console.WriteLine($"Column A width: {worksheet.Cells.GetColumnWidth(0)}");
                Console.WriteLine($"Column B width: {worksheet.Cells.GetColumnWidth(1)}");
                Console.WriteLine($"Column C width: {worksheet.Cells.GetColumnWidth(2)}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AutoFitColumns method: {ex.Message}");
            }
            
            // Sonucu kaydet
            workbook.Save("AutoFitColumnsWithOptionsDemo.xlsx");
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

## AutoFitColumns(int, int, int, int) {#autofitcolumns_4}

Sütun genişliklerini otomatik olarak ayarlar.

```csharp
public void AutoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| firstRow | Int32 | İlk satır indeksi. |
| firstColumn | Int32 | İlk sütun indeksi. |
| lastRow | Int32 | Son satır indeksi. |
| lastColumn | Int32 | Son sütun indeksi. |

### Açıklamalar

AutoFitColumn, kesin olmayan bir işlevdir.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitColumnsWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Gösterim için bazı verileri doldur
            worksheet.Cells["A1"].PutValue("Short");
            worksheet.Cells["B1"].PutValue("Medium length text");
            worksheet.Cells["C1"].PutValue("Very very long text that needs more column width");
            
            // Sütunları 0 (A) ile 2 (C) arasında, ilk satır 0 ve son satır 0 ile otomatik sığdır
            worksheet.AutoFitColumns(0, 2, 0, 0);
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitColumns(int, int, int, int, AutoFitterOptions) {#autofitcolumns_5}

Sütun genişliklerini otomatik olarak ayarlar.

```csharp
public void AutoFitColumns(int firstRow, int firstColumn, int lastRow, int lastColumn, 
    AutoFitterOptions options)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| firstRow | Int32 | İlk satır indeksi. |
| firstColumn | Int32 | İlk sütun indeksi. |
| lastRow | Int32 | Son satır indeksi. |
| lastColumn | Int32 | Son sütun indeksi. |
| seçenekler | AutoFitterOptions | Otomatik sığdırma seçenekleri |

### Açıklamalar

AutoFitColumn, kesin olmayan bir işlevdir.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorksheetMethodAutoFitColumnsWithInt32Int32Int32Int32AutoFitterDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Sütun genişliği ayarı gerektiren örnek veriyle hücreleri doldur
            worksheet.Cells["A1"].PutValue("This is a long text that needs column autofit");
            worksheet.Cells["B1"].PutValue("Another lengthy text string for demonstration");
            worksheet.Cells["C1"].PutValue("Short");
            worksheet.Cells["A2"].PutValue(12345.6789);
            worksheet.Cells["B2"].PutValue("Multi-line\ntext\nsample");
            worksheet.Cells["C2"].PutValue(true);

            // Belirli ayarlarla AutoFitterOptions oluştur
            AutoFitterOptions options = new AutoFitterOptions();
            options.AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine;
            options.IgnoreHidden = false;
            options.OnlyAuto = false;

            try
            {
                // AutoFitColumns'ı (firstRow, firstColumn, lastRow, lastColumn, options) belirli parametrelerle çağır
                worksheet.AutoFitColumns(0, 0, 1, 2, options);
                
                Console.WriteLine("AutoFitColumns method executed successfully with parameters (Int32, Int32, Int32, Int32, AutoFitterOptions)");
                
                // Otomatik sığdırmadan sonra sütun genişliklerini göster
                Console.WriteLine($"Column A width after autofit: {worksheet.Cells.GetColumnWidth(0)}");
                Console.WriteLine($"Column B width after autofit: {worksheet.Cells.GetColumnWidth(1)}");
                Console.WriteLine($"Column C width after autofit: {worksheet.Cells.GetColumnWidth(2)}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AutoFitColumns method: {ex.Message}");
            }
            
            // Sonucu kaydet
            workbook.Save("AutoFitColumnsWithOptionsDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [AutoFitterOptions](../../autofitteroptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


