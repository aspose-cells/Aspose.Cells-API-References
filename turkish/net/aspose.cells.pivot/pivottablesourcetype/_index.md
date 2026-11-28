---
title: "Enum PivotTableSourceType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Pivot.PivotTableSourceType enum. Pivot tablonun veri kaynağı türünü temsil eder"
type: docs
url: /tr/net/aspose.cells.pivot/pivottablesourcetype/
---
## PivotTableSourceType enumeration

PivotTable veri kaynağı türünü temsil eder.

```csharp
public enum PivotTableSourceType : byte
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Sheet | `1` | Kaynak verinin bir aralık olduğunu belirtir. |
| External | `2` | Harici kaynak verisinin kullanıldığını belirtir. |
| Consolidation | `4` | Birden çok konsolidasyon aralığının kaynak veri olarak kullanıldığını belirtir. |
| Scenario | `8` | Kaynak veri geçici bir iç yapıyıdan doldurulur. |
| Unknown | `9` | Bilinmeyen veri kaynağı. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotClassPivotTableSourceTypeDemo
    {
        public static void Run()
        {
            // Demonstrasyon için yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Çalışma sayfasına örnek veri ekle
                worksheet.Cells["A1"].PutValue("Category");
                worksheet.Cells["B1"].PutValue("Value");
                worksheet.Cells["A2"].PutValue("A");
                worksheet.Cells["B2"].PutValue(10);
                worksheet.Cells["A3"].PutValue("B");
                worksheet.Cells["B3"].PutValue(20);
                worksheet.Cells["A4"].PutValue("C");
                worksheet.Cells["B4"].PutValue(30);

                // Bir pivot tablo koleksiyonu oluştur
                PivotTableCollection pivotTables = worksheet.PivotTables;

                // Kaynak türü olarak Sheet kullanan bir pivot tablo ekle
                int index = pivotTables.Add("=A1:B4", "D3", "SheetPivotTable");
                PivotTable pivotTable = pivotTables[index];

                // Kaynak türünü göster
                Console.WriteLine("Pivot Table Source Type: " + pivotTable.SourceType);

                // Farklı kaynak türlerini göster
                Console.WriteLine("Available PivotTableSourceType values:");
                Console.WriteLine("Sheet: " + PivotTableSourceType.Sheet);
                Console.WriteLine("External: " + PivotTableSourceType.External);
                Console.WriteLine("Consolidation: " + PivotTableSourceType.Consolidation);
                Console.WriteLine("Scenario: " + PivotTableSourceType.Scenario);
                Console.WriteLine("Unknown: " + PivotTableSourceType.Unknown);

                // Çalışma kitabını kaydedin
                workbook.Save("PivotTableSourceTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with PivotTableSourceType: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


