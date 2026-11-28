---
title: "RowCollection.RemoveAt"
second_title: "Aspose.Cells için .NET API Referansı"
description: "RowCollection yöntemi. Bu koleksiyondaki belirtilen indeks konumundaki satır öğesini kaldır"
type: docs
url: /tr/net/aspose.cells/rowcollection/removeat/
---
## RowCollection.RemoveAt method

Bu koleksiyondaki belirtilen indeks (konum) konumundaki satır öğesini kaldırın.

```csharp
public void RemoveAt(int index)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| index | Int32 | Bu koleksiyondaki mevcut satır öğesinin sıfır tabanlı indeksi (konumu, `[`Index`](../../row/index/)` değil). |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RowCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // İlk birkaç satırdaki hücrelere bazı veriler ekle
            worksheet.Cells["A1"].PutValue("Row 1");
            worksheet.Cells["A2"].PutValue("Row 2");
            worksheet.Cells["A3"].PutValue("Row 3");
            worksheet.Cells["A4"].PutValue("Row 4");

            // İlk satır sayısını göster
            Console.WriteLine($"Initial row count: {worksheet.Cells.Rows.Count}");

            try
            {
                // Satırı indeks 1'de (ikinci satır) kaldırmak için RemoveAt yöntemini çağır
                worksheet.Cells.Rows.RemoveAt(1);

                Console.WriteLine("Method executed successfully. Row at index 1 removed.");

                // Güncellenmiş satır sayısını göster
                Console.WriteLine($"Updated row count: {worksheet.Cells.Rows.Count}");

                // Etkiyi göster - Satır 2 kaldırılmalı, Satır 3 Satır 2 olur
                Console.WriteLine("Cell A1: " + worksheet.Cells["A1"].StringValue);
                Console.WriteLine("Cell A2: " + worksheet.Cells["A2"].StringValue);
                Console.WriteLine("Cell A3: " + worksheet.Cells["A3"].StringValue);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RemoveAt method: {ex.Message}");
            }

            // Sonucu kaydet
            workbook.Save("RowCollectionMethodRemoveAtWithInt32Demo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [RowCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


