---
title: "Cells.InsertRows"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Çalışma sayfasına birden fazla satır ekler"
type: docs
url: /tr/net/aspose.cells/cells/insertrows/
---
## InsertRows(int, int, bool) {#insertrows_2}

Çalışma sayfasına birden fazla satır ekler.

```csharp
public void InsertRows(int rowIndex, int totalRows, bool updateReference)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowIndex | Int32 | Satır indeksi. |
| totalRows | Int32 | Eklenecek satır sayısı. |
| updateReference | Boolean | Diğer çalışma sayfalarındaki referansların güncellenip güncellenmeyeceğini gösterir. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertRowsWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Data 1");
            worksheet.Cells["A3"].PutValue("Data 2");
            worksheet.Cells["A4"].PutValue("Data 3");
            
            // 2. indekste bir satır ekle (yeni 3. satır olur)
            worksheet.Cells.InsertRows(2, 1, true);
            
            // Eklenen satıra veri ekle
            worksheet.Cells["A3"].PutValue("Inserted Data");
            
            // Çalışma kitabını kaydedin
            workbook.Save("InsertRowsDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## InsertRows(int, int, InsertOptions) {#insertrows_1}

Çalışma sayfasına birden fazla satır ekler.

```csharp
public void InsertRows(int rowIndex, int totalRows, InsertOptions options)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowIndex | Int32 | Satır indeksi. |
| totalRows | Int32 | Eklenecek satır sayısı. |
| seçenekler | InsertOptions | Ekleme işlemi için seçenekler. |

### Örnekler

```csharp
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertRowsWithInt32Int32InsertOptionsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Biraz örnek veri doldurun
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].Value = "Row " + (i + 1);
            }

            InsertOptions insertOptions = new InsertOptions
            {
                CopyFormatType = CopyFormatType.SameAsAbove,
                UpdateReference = true
            };

            // Belirtilen seçeneklerle 5. satır indeksinde 3 satır ekle
            worksheet.Cells.InsertRows(5, 3, insertOptions);

            workbook.Save("InsertRowsWithOptions.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [InsertOptions](../../insertoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## InsertRows(int, int) {#insertrows}

Çalışma sayfasına birden fazla satır ekler.

```csharp
public void InsertRows(int rowIndex, int totalRows)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowIndex | Int32 | Satır indeksi. |
| totalRows | Int32 | Eklenecek satır sayısı. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertRowsWithInt32Int32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Örnek veri ekleyin
            cells["A1"].PutValue("Header1");
            cells["B1"].PutValue("Header2");
            cells["A2"].PutValue("Data1");
            cells["B2"].PutValue("Data2");
            cells["A3"].PutValue("Data3");
            cells["B3"].PutValue("Data4");

            // 2. satır indeksinde 2 satır ekle
            cells.InsertRows(2, 2);

            // Eklenen satırların boş olduğunu doğrula
            Console.WriteLine("Cell A2 value: " + cells[1, 0].Value); // Should be "Data1"
            Console.WriteLine("Cell A3 value: " + cells[2, 0].Value); // Should be null (empty)
            Console.WriteLine("Cell A4 value: " + cells[3, 0].Value); // Should be null (empty)
            Console.WriteLine("Cell A5 value: " + cells[4, 0].Value); // Should be "Data3"

            // Çalışma kitabını kaydedin
            workbook.Save("InsertRowsDemo_out.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


