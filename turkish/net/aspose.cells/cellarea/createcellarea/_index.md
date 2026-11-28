---
title: "CellArea.CreateCellArea"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CellArea yöntemi. Bir hücre alanı oluşturur"
type: docs
url: /tr/net/aspose.cells/cellarea/createcellarea/
---
## CreateCellArea(int, int, int, int) {#createcellarea}

Bir hücre alanı oluşturur.

```csharp
public static CellArea CreateCellArea(int startRow, int startColumn, int endRow, int endColumn)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startRow | Int32 | Başlangıç satırı. |
| startColumn | Int32 | Başlangıç sütunu. |
| endRow | Int32 | Bitiş satırı. |
| endColumn | Int32 | Bitiş sütunu. |

### Dönüş Değeri

Bir [`CellArea`](../) döndürün.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellAreaMethodCreateCellAreaWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            
            // Hücreleri örnek veriyle doldurun
            int[] values = { 1, 3, 2, 6, 4, 5, 8, 9, 7 };
            for (int i = 0; i < values.Length; i++)
            {
                cells[i, i / 3].PutValue(values[i]);
            }

            // Veri sıralayıcıyı oluşturun ve yapılandırın
            DataSorter sorter = wb.DataSorter;
            sorter.Clear();
            sorter.Order1 = SortOrder.Ascending;
            sorter.Key1 = 2;
            sorter.Order2 = SortOrder.Ascending;
            sorter.Key2 = 1;
            sorter.Order3 = SortOrder.Ascending;
            sorter.Key3 = 0;

            // Int32 parametreleriyle CreateCellArea kullanarak sıralayın
            sorter.Sort(cells, CellArea.CreateCellArea(0, 0, 8, 2));

            // Sıralanmış değerleri çıktıla
            Console.WriteLine("Sorted values:");
            for (int i = 0; i < 9; i++)
            {
                Console.WriteLine(cells[i, 2 - i / 3].IntValue);
            }
        }
    }
}
```

### Ayrıca Bakınız

* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CreateCellArea(string, string) {#createcellarea_1}

Bir hücre alanı oluşturur.

```csharp
public static CellArea CreateCellArea(string startCellName, string endCellName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startCellName | String | Aralığın sol üst hücresi. |
| endCellName | String | Aralığın sağ alt hücresi. |

### Dönüş Değeri

Bir [`CellArea`](../) döndürün.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellAreaMethodCreateCellAreaWithStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // A sütununa bazı veriler ekleyin
            for (int i = 0; i < 10; i++)
            {
                cells[i, 0].PutValue($"Data {i}");
            }

            // B1'den B10'a kadar hücre alanı oluşturun
            CellArea area = CellArea.CreateCellArea("B1", "B10");
            
            // Hücreleri aşağı kaydırarak aralığı ekleyin
            cells.InsertRange(area, ShiftType.Down);
            
            // Hücre değerlerini kontrol ederek işlemi doğrulayın
            Console.WriteLine("Inserted range from B1 to B10. Total rows: " + cells.Rows.Count);
        }
    }
}
```

### Ayrıca Bakınız

* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


