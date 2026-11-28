---
title: "CellsHelper.CellNameToIndex"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CellsHelper yöntemi. Hücrenin adını göre satır ve sütun indekslerini alır."
type: docs
url: /tr/net/aspose.cells/cellshelper/cellnametoindex/
---
## CellsHelper.CellNameToIndex method

Hücre adını temel alarak hücrenin satır ve sütun indekslerini alır.

```csharp
public static void CellNameToIndex(string cellName, out int row, out int column)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cellName | String | Hücre adı. |
| satır | Int32& | Satır indeksi çıktısı |
| sütun | Int32& | Sütun indeksi çıktısı |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsHelperMethodCellNameToIndexWithStringInt32Int32Demo
    {
        public static void Run()
        {
            // Satır ve sütun indekslerini tutacak değişkenleri başlat
            int rowIndex = -1;
            int columnIndex = -1;
            string cellName = "C5";

            try
            {
                // CellNameToIndex yöntemini çağırarak hücre adını satır ve sütun indekslerine dönüştürün
                CellsHelper.CellNameToIndex(cellName, out rowIndex, out columnIndex);

                // Sonuçları görüntüleyin
                Console.WriteLine($"Cell name: {cellName}");
                Console.WriteLine($"Row index: {rowIndex}");
                Console.WriteLine($"Column index: {columnIndex}");

                // Bir çalışma kitabı oluşturun ve indekslerin kullanımını gösterin
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Elde edilen indeksleri kullanarak hücreye erişin
                Cell cell = worksheet.Cells[rowIndex, columnIndex];
                cell.PutValue("Test Value");

                // Çalışma kitabını kaydedin
                workbook.Save("CellNameToIndexDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing CellNameToIndex method: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


