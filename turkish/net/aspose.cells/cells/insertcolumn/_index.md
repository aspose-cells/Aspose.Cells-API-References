---
title: "Cells.InsertColumn"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Çalışma sayfasına yeni bir sütun ekler"
type: docs
url: /tr/net/aspose.cells/cells/insertcolumn/
---
## InsertColumn(int, bool) {#insertcolumn_1}

Çalışma sayfasına yeni bir sütun ekler.

```csharp
public void InsertColumn(int columnIndex, bool updateReference)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| columnIndex | Int32 | Sütun indeksi. |
| updateReference | Boolean | Diğer çalışma sayfalarındaki referansların güncellenip güncellenmeyeceğini gösterir. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertColumnWithInt32BooleanDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Sütun 0'a bazı örnek veriler doldurun
            Cells cells = sheet.Cells;
            for (int i = 0; i < 5; i++)
            {
                cells[i, 0].PutValue($"Original {i}");
            }

            // İndeks 1'de yeni bir sütun ekleyin ve sütunları sağa kaydırın
            cells.InsertColumn(1, true);

            // Verileri sütun 0'dan yeni sütun 1'e kopyalayın
            cells.CopyColumn(cells, 0, 1);

            // Çalışma kitabını kaydedin
            workbook.Save("InsertColumnDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## InsertColumn(int) {#insertcolumn}

Çalışma sayfasına yeni bir sütun ekler.

```csharp
public void InsertColumn(int columnIndex)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| columnIndex | Int32 | Sütun indeksi. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertColumnWithInt32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet sheet = workbook.Worksheets[0];
            
            // Hücre koleksiyonunu alın
            Cells cells = sheet.Cells;
            
            // Gösterim için hücrelere veri ekleyin
            cells["A1"].PutValue("Column A");
            cells["B1"].PutValue("Column B");
            cells["C1"].PutValue("Column C");
            
            // İndeks 1'de yeni bir sütun ekleyin (yeni sütun B olacaktır)
            cells.InsertColumn(1);
            
            // Yeni sütuna veri ekleyerek doğrulayın
            cells["B1"].PutValue("New Column");
            
            // Çalışma kitabını kaydedin
            workbook.Save("InsertColumnDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


