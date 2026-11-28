---
title: "Cells.DeleteColumn"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Bir sütunu siler"
type: docs
url: /tr/net/aspose.cells/cells/deletecolumn/
---
## DeleteColumn(int, bool) {#deletecolumn_1}

Bir sütunu siler.

```csharp
public void DeleteColumn(int columnIndex, bool updateReference)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| columnIndex | Int32 | Silinecek sütunun indeksi. |
| updateReference | Boolean | Diğer çalışma sayfalarındaki referansların güncellenip güncellenmeyeceğini gösterir. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteColumnWithInt32BooleanDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet sheet = workbook.Worksheets[0];
            
            // Hücrelere örnek veri doldurun
            for (int i = 0; i < 5; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    sheet.Cells[i, j].PutValue($"Data {i},{j}");
                }
            }
            
            Console.WriteLine("Before deleting column:");
            PrintCellValues(sheet);
            
            // İlk sütunu sil ve kalan sütunları sola kaydır
            sheet.Cells.DeleteColumn(0, true);
            
            Console.WriteLine("\nAfter deleting column 0:");
            PrintCellValues(sheet);
            
            // Çalışma kitabını kaydedin
            workbook.Save("DeleteColumnDemo.xlsx");
        }
        
        private static void PrintCellValues(Worksheet sheet)
        {
            for (int i = 0; i < 5; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    Console.Write(sheet.Cells[i, j].Value + "\t");
                }
                Console.WriteLine();
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

## DeleteColumn(int) {#deletecolumn}

Bir sütunu siler.

```csharp
public void DeleteColumn(int columnIndex)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| columnIndex | Int32 | Silinecek sütunun indeksi. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteColumnWithInt32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet sheet = workbook.Worksheets[0];
            
            // Sütunlara örnek veri doldurun
            Cells cells = sheet.Cells;
            cells["A1"].PutValue("Column A");
            cells["B1"].PutValue("Column B");
            cells["C1"].PutValue("Column C");
            
            // 1. indeksteki sütunu sil (Sütun B)
            cells.DeleteColumn(1);
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
            
            Console.WriteLine("Column deleted successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


