---
title: "Cells.DeleteBlankRows"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Veri veya başka bir nesne içermeyen tüm boş satırları siler"
type: docs
url: /tr/net/aspose.cells/cells/deleteblankrows/
---
## DeleteBlankRows() {#deleteblankrows}

Veri veya başka bir nesne içermeyen tüm boş satırları sil.

```csharp
public void DeleteBlankRows()
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteBlankRowsDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Boş satırlarla birlikte bazı veriler ekleyin
            cells["A1"].PutValue("Header");
            cells["A2"].PutValue("Data1");
            cells["A4"].PutValue("Data2"); // Blank row at A3
            cells["A6"].PutValue("Data3"); // Blank row at A5

            Console.WriteLine("Before deleting blank rows:");
            for (int i = 0; i < 7; i++)
            {
                Console.WriteLine($"Row {i + 1}: {cells[i, 0].StringValue}");
            }

            // Boş satırları sil
            cells.DeleteBlankRows();

            Console.WriteLine("\nAfter deleting blank rows:");
            for (int i = 0; i < cells.MaxDataRow + 1; i++)
            {
                Console.WriteLine($"Row {i + 1}: {cells[i, 0].StringValue}");
            }

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

## DeleteBlankRows(DeleteOptions) {#deleteblankrows_1}

Veri veya görünür yorum, pivot tablo gibi bazı özel nesneler içermeyen tüm boş satırları sil.

```csharp
public void DeleteBlankRows(DeleteOptions options)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| seçenekler | DeleteOptions | Silme aralığının seçenekleri. |

### Açıklamalar

Silinecek boş satırlar için, sadece [`IsBlank`](../../row/isblank/) değerinin true olması yeterli değildir; aynı zamanda bu satırlardaki hiçbir hücreye tanımlı görünür bir yorum olmamalı ve bu satırlarla kesişen bir özet tablo (pivot table) bulunmamalıdır.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteBlankRowsWithDeleteOptionsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet sheet = workbook.Worksheets[0];
            
            // Boş satırlarla birlikte bazı test verileri ekleyin
            sheet.Cells["A1"].PutValue("Data1");
            sheet.Cells["A3"].PutValue("Data2");
            sheet.Cells["A5"].PutValue("Data3");
            
            // Silme seçenekleri oluşturun
            DeleteOptions options = new DeleteOptions();
            options.UpdateReference = true;
            
            // Boş satırları sil
            sheet.Cells.DeleteBlankRows(options);
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [DeleteOptions](../../deleteoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


