---
title: "Cells.ExportTypeArray"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Cells koleksiyonundaki hücre değer türünü iki boyutlu bir dizi nesnesine dışa aktarır"
type: docs
url: /tr/net/aspose.cells/cells/exporttypearray/
---
## Cells.ExportTypeArray method

[`Cells`](../) koleksiyonundaki hücre değer türünü iki boyutlu bir dizi nesnesine dışa aktarır.

```csharp
public CellValueType[] ExportTypeArray(int firstRow, int firstColumn, int totalRows, 
    int totalColumns)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| firstRow | Int32 | Dışa aktarılacak ilk hücrenin satır numarası. |
| firstColumn | Int32 | Dışa aktarılacak ilk hücrenin sütun numarası. |
| totalRows | Int32 | Dışa aktarılacak satır sayısı. |
| totalColumns | Int32 | Dışa aktarılacak sütun sayısı. |

### Dönüş Değeri

Hücre değer türlerini temsil eden dışa aktarılmış dizi nesnesi.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodExportTypeArrayWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Hücrelerdeki değerleri ayarla
            cells["A1"].PutValue(10);
            cells["B1"].PutValue("Hello");
            cells["A2"].PutValue(true);
            cells["B2"].PutValue(DateTime.Now);

            // Hücre türlerini 2D diziye dışa aktar
            CellValueType[,] typeArray = cells.ExportTypeArray(0, 0, 2, 2);

            // Sonuçları görüntüleyin
            for (int i = 0; i < 2; i++)
            {
                for (int j = 0; j < 2; j++)
                {
                    Console.WriteLine($"Cell[{i},{j}] Type: {typeArray[i, j]}");
                }
            }

            // İstisna durumunu göster
            try
            {
                CellValueType[,] invalidArray = cells.ExportTypeArray(-1, 0, 2, 2);
            }
            catch (CellsException ex)
            {
                Console.WriteLine("Exception caught as expected: " + ex.Message);
            }
        }
    }
}
```

### Ayrıca Bakınız

* enum [CellValueType](../../cellvaluetype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


