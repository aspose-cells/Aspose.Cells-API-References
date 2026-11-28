---
title: "Cells.Subtotal"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Aralık için alt toplamlar oluşturur"
type: docs
url: /tr/net/aspose.cells/cells/subtotal/
---
## Subtotal(CellArea, int, ConsolidationFunction, int[]) {#subtotal}

Aralık için alt toplamlar oluşturur.

```csharp
public void Subtotal(CellArea ca, int groupBy, ConsolidationFunction function, int[] totalList)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ca | CellArea | Aralık |
| groupBy | Int32 | Gruplamak için alan, sıfır‑tabanlı bir tam sayı ofseti olarak |
| fonksiyon | ConsolidationFunction | Alt toplam işlevi. |
| totalList | Int32[] | Alt toplamların eklendiği alanları gösteren, sıfır tabanlı alan ofsetlerinden oluşan bir dizi. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodSubtotalWithCellAreaInt32ConsolidationFuncDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Alt toplam için örnek verileri doldur
            CreateSampleData(worksheet);

            // Veri içeren hücre alanını tanımla (A1:C6)
            CellArea cellArea = CellArea.CreateCellArea(0, 0, 5, 2);

            try
            {
                // Subtotal yöntemini şu parametrelerle çağır:
                // - Sütun 0'a göre grupla (Region)
                // - SUM işlevini kullan
                // - Sütun 2'ye uygula (Sales)
                worksheet.Cells.Subtotal(
                    cellArea,
                    0,
                    ConsolidationFunction.Sum,
                    new int[] { 2 }
                );

                Console.WriteLine("Subtotal added successfully for parameters (CellArea, 0, Sum, [2])");
                
                // Derleme hatalarını düzeltmek için ExpandColumnLevel ve ExpandRowLevel yöntemleri kaldırıldı.
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Subtotal method: {ex.Message}");
            }

            // Sonucu kaydet
            workbook.Save("CellsMethodSubtotalWithCellAreaInt32ConsolidationFuncDemo.xlsx");
        }

        private static void CreateSampleData(Worksheet worksheet)
        {
            // Başlık satırı oluştur
            worksheet.Cells["A1"].PutValue("Region");
            worksheet.Cells["B1"].PutValue("Product");
            worksheet.Cells["C1"].PutValue("Sales");

            // Veri satırları oluştur
            object[,] data = new object[,] {
                {"North", "Widget", 5000},
                {"North", "Gadget", 3000},
                {"South", "Widget", 6000},
                {"South", "Gadget", 4000},
                {"West", "Widget", 4500}
            };

            // Verileri 2. satırdan (sıfır tabanlı indeks 1) itibaren doldur
            for (int i = 0; i < data.GetLength(0); i++)
            {
                worksheet.Cells[i + 1, 0].PutValue(data[i, 0]);
                worksheet.Cells[i + 1, 1].PutValue(data[i, 1]);
                worksheet.Cells[i + 1, 2].PutValue(data[i, 2]);
            }
        }
    }
}
```

### Ayrıca Bakınız

* struct [CellArea](../../cellarea/)
* enum [ConsolidationFunction](../../consolidationfunction/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Subtotal(CellArea, int, ConsolidationFunction, int[], bool, bool, bool) {#subtotal_1}

Aralık için alt toplamlar oluşturur.

```csharp
public void Subtotal(CellArea ca, int groupBy, ConsolidationFunction function, int[] totalList, 
    bool replace, bool pageBreaks, bool summaryBelowData)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ca | CellArea | Aralık |
| groupBy | Int32 | Gruplamak için alan, sıfır‑tabanlı bir tam sayı ofseti olarak |
| fonksiyon | ConsolidationFunction | Alt toplam işlevi. |
| totalList | Int32[] | Alt toplamların eklendiği alanları gösteren, sıfır tabanlı alan ofsetlerinden oluşan bir dizi. |
| değiştir | Boolean | Mevcut ara toplamların değiştirilip değiştirilmeyeceğini gösterir |
| sayfaKesintileri | Boolean | Gruplar arasında sayfa kesintisi eklenip eklenmeyeceğini gösterir |
| summaryBelowData | Boolean | Verilerin altında özet eklenip eklenmeyeceğini gösterir. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodSubtotalWithCellAreaInt32ConsolidationFuncDemo1
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Ara toplam için örnek veri oluştur
            cells["A1"].PutValue("Category");
            cells["B1"].PutValue("Product");
            cells["C1"].PutValue("Sales");
            
            object[,] data = new object[,] {
                { "Fruits", "Apple", 1500 },
                { "Fruits", "Orange", 2500 },
                { "Vegetables", "Carrot", 1800 },
                { "Vegetables", "Potato", 3000 },
                { "Fruits", "Banana", 2000 }
            };

            for (int row = 0; row < 5; row++)
            {
                for (int col = 0; col < 3; col++)
                {
                    cells[row + 1, col].PutValue(data[row, col]);
                }
            }

            try
            {
                // Ara toplam için hücre alanını tanımla (A1:C6)
                CellArea area = new CellArea();
                area.StartRow = 0;
                area.StartColumn = 0;
                area.EndRow = 5;
                area.EndColumn = 2;

                // Parametrelerle Subtotal'ı çağır:
                // - İlk sütuna göre grupla (sıfır tabanlı indeks 0)
                // - Toplam fonksiyonunu kullan
                // - Üçüncü sütuna uygula (sıfır tabanlı indeks 2)
                // - Mevcut ara toplamları değiştir, gruplar arasında sayfa kesintileri, veri altında özet
                cells.Subtotal(
                    area,
                    0,
                    ConsolidationFunction.Sum,
                    new int[] { 2 },
                    true,
                    true,
                    true
                );

                Console.WriteLine("Subtotal added successfully for parameters: (CellArea, Int32, ConsolidationFunction, Int32[], Boolean, Boolean, Boolean)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating subtotal: {ex.Message}");
            }

            workbook.Save("SubtotalDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* struct [CellArea](../../cellarea/)
* enum [ConsolidationFunction](../../consolidationfunction/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


