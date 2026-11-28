---
title: "Worksheet.AutoFitColumn"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet yöntemi. Sütun genişliğini otomatik olarak ayarlar"
type: docs
url: /tr/net/aspose.cells/worksheet/autofitcolumn/
---
## AutoFitColumn(int, int, int) {#autofitcolumn_1}

Sütun genişliğini otomatik olarak ayarlar.

```csharp
public void AutoFitColumn(int columnIndex, int firstRow, int lastRow)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| columnIndex | Int32 | Sütun indeksi. |
| firstRow | Int32 | İlk satır indeksi. |
| lastRow | Int32 | Son satır indeksi. |

### Açıklamalar

Bu yöntem, satır içindeki hücre aralığındaki içeriğe göre bir satırı otomatik ayarlar.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorksheetMethodAutoFitColumnWithInt32Int32Int32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Sütun genişliği ayarlaması gerektirecek örnek veriyle hücreleri doldurun
            worksheet.Cells["A1"].PutValue("Short text");
            worksheet.Cells["A2"].PutValue("This is a much longer piece of text that will require column width adjustment");
            worksheet.Cells["A3"].PutValue("Another long text entry to demonstrate AutoFitColumn");
            
            try
            {

                Console.WriteLine($"Column width before: {worksheet.Cells.GetColumnWidth(0)}");
                // Satır 0'dan 2'ye (sıfır tabanlı) kadar sütun A (indeks 0) üzerinde AutoFitColumn çağırın
                worksheet.AutoFitColumn(0, 0, 2);
                
                Console.WriteLine("AutoFitColumn method executed successfully on column A for rows 1-3");
                
                // Sütun genişliğini önce ve sonra göstererek etkiyi görüntüleyin                
                Console.WriteLine($"Column width after: {worksheet.Cells.GetColumnWidth(0)}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AutoFitColumn method: {ex.Message}");
            }
            
            // Sonucu kaydet
            workbook.Save("AutoFitColumnWithInt32Int32Int32Demo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitColumn(int) {#autofitcolumn}

Sütun genişliğini otomatik olarak ayarlar.

```csharp
public void AutoFitColumn(int columnIndex)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| columnIndex | Int32 | Sütun indeksi. |

### Açıklamalar

AutoFitColumn, kesin olmayan bir işlevdir.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitColumnWithInt32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Sütun 4'teki hücrelere örnek veri ekleyin (0 tabanlı indeks)
            worksheet.Cells["D1"].PutValue("This is a test");
            worksheet.Cells["D2"].PutValue("AutoFitColumn demonstration");
            worksheet.Cells["D3"].PutValue("Aspose.Cells for .NET");
            
            // Sütun 4'ü otomatik sığdır (0 tabanlı indeks)
            worksheet.AutoFitColumn(3);
            
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


