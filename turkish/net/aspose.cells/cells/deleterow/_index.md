---
title: "Cells.DeleteRow"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Bir satırı siler"
type: docs
url: /tr/net/aspose.cells/cells/deleterow/
---
## DeleteRow(int) {#deleterow}

Bir satırı siler.

```csharp
public void DeleteRow(int rowIndex)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowIndex | Int32 | Silinecek satırın indeksi. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteRowWithInt32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;

            // Satır 66'da ortak bir formül ayarlayın
            cells[65, 0].SetSharedFormula("=SUM(B10:B66)", 1, 6);

            // Satır 9'u sil (satırları yukarı kaydıracak)
            cells.DeleteRow(9);

            // Satır silme işleminden sonra formülün ayarlandığını doğrulayın
            for (int i = 1; i < 7; i++)
            {
                char columnName = (char)('A' + i);
                Console.WriteLine($"Cell {columnName}66 formula after deletion: {cells[64, i].Formula}");
            }

            // Satır 60-61'i sil (satırları yukarı kaydıracak)
            cells.DeleteRows(59, 2);

            // Satırların silinmesinden sonra formülün ayarlandığını doğrulayın
            for (int i = 1; i < 7; i++)
            {
                char columnName = (char)('A' + i);
                Console.WriteLine($"Cell {columnName}64 formula after deletion: {cells[62, i].Formula}");
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

## DeleteRow(int, bool) {#deleterow_1}

Bir satırı siler.

```csharp
public void DeleteRow(int rowIndex, bool updateReference)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowIndex | Int32 | Silinecek satırın indeksi. |
| updateReference | Boolean | Diğer çalışma sayfalarındaki referansların güncellenip güncellenmeyeceğini gösterir. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteRowWithInt32BooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            sheet.Cells["A1"].PutValue("Item");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["A3"].PutValue("Banana");
            sheet.Cells["A4"].PutValue("Cherry");

            Console.WriteLine("Original Data:");
            for (int i = 1; i <= 4; i++)
            {
                Console.WriteLine(sheet.Cells[$"A{i}"].Value);
            }

            sheet.Cells.DeleteRow(2, true);

            Console.WriteLine("\nData After Deletion:");
            for (int i = 1; i <= 3; i++)
            {
                Console.WriteLine(sheet.Cells[$"A{i}"].Value);
            }

            workbook.Save("DeleteRowExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


