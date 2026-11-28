---
title: "Cells.ExportArray"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Cells koleksiyonundaki verileri iki boyutlu dizi nesnesine dışa aktarır"
type: docs
url: /tr/net/aspose.cells/cells/exportarray/
---
## Cells.ExportArray method

[`Cells`](../) koleksiyonundaki verileri iki boyutlu dizi nesnesine dışa aktarır.

```csharp
public object[] ExportArray(int firstRow, int firstColumn, int totalRows, int totalColumns)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| firstRow | Int32 | Dışa aktarılacak ilk hücrenin satır numarası. |
| firstColumn | Int32 | Dışa aktarılacak ilk hücrenin sütun numarası. |
| totalRows | Int32 | Dışa aktarılacak satır sayısı |
| totalColumns | Int32 | Dışa aktarılacak sütun sayısı |

### Dönüş Değeri

Dışa aktarılan hücre değeri dizi nesnesi.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodExportArrayWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Biraz örnek veri doldurun
            cells[0, 0].PutValue("A");
            cells[0, 1].PutValue("B");
            cells[1, 0].PutValue(10);
            cells[1, 1].PutValue(20);

            try
            {
                // Verileri diziye dışa aktar
                object[,] dataArray = cells.ExportArray(0, 0, 2, 2);
                
                // Dışa aktarılan diziyi göster
                for (int i = 0; i < 2; i++)
                {
                    for (int j = 0; j < 2; j++)
                    {
                        Console.Write(dataArray[i, j] + "\t");
                    }
                    Console.WriteLine();
                }
            }
            catch (CellsException ex)
            {
                Console.WriteLine("Error exporting array: " + ex.Message);
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


