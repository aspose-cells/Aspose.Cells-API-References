---
title: "Cells.GetRow"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells metodu. Belirtilen hücre satır indeksindeki Row öğesini alır"
type: docs
url: /tr/net/aspose.cells/cells/getrow/
---
## Cells.GetRow method

Belirtilen hücre satır indeksindeki [`Row`](../../row/) öğesini alır.

```csharp
[Obsolete("Use Cells.CheckRow(int row) instead.")]
public Row GetRow(int row)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | Int32 | Satır indeksi |

### Dönüş Değeri

Satır nesnesi mevcutsa Row nesnesini döndür, aksi takdirde null döndür.

### Açıklamalar

NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine lütfen Cells.CheckRow(int row) metodunu kullanın. Bu metod Şubat 2024'ten itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodGetRowWithInt32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Satırın mevcut olduğundan emin olmak için 5. satırda hücreler oluşturun
            worksheet.Cells["A5"].PutValue("Row 5 Data");
            worksheet.Cells["B5"].PutValue(12345);

            try
            {
                // Int32 parametresiyle GetRow metodunu çağırın
                Row resultRow = worksheet.Cells.GetRow(5);

                if (resultRow != null)
                {
                    // Satır manipülasyonunu gösterin
                    resultRow.Height = 20;
                    Console.WriteLine($"Retrieved row 5 successfully. Current height: {resultRow.Height} points");
                    
                    // Satırdaki hücreleri sayın
                    int cellCount = 0;
                    foreach (Cell cell in resultRow)
                    {
                        cellCount++;
                    }
                    Console.WriteLine($"Row 5 contains {cellCount} cells");
                }
                else
                {
                    Console.WriteLine("Row 5 not found in worksheet");
                }
            }
            catch (ArgumentOutOfRangeException ex)
            {
                Console.WriteLine($"Invalid row index: {ex.Message}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetRow: {ex.Message}");
            }

            // Değiştirilmiş çalışma kitabını kaydet
            workbook.Save("CellsMethodGetRowWithInt32Demo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Row](../../row/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


