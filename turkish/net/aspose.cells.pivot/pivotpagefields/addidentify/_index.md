---
title: "PivotPageFields.AddIdentify"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotPageFields yöntemi. Her sayfa alanındaki hangi öğe etiketinin veri aralığını tanımlamak için kullanılacağını ayarlar. pageItemIndex.Length, PageFieldCount değerine eşit olmalıdır, bu yüzden lütfen önce sayfa alanını ekleyin."
type: docs
url: /tr/net/aspose.cells.pivot/pivotpagefields/addidentify/
---
## PivotPageFields.AddIdentify method

Her sayfa alanındaki hangi öğe etiketinin veri aralığını tanımlamak için kullanılacağını ayarlar. pageItemIndex.Length, PageFieldCount değerine eşit olmalıdır, bu yüzden önce sayfa alanını ekleyin.

```csharp
public void AddIdentify(int rangeIndex, int[] pageItemIndex)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rangeIndex | Int32 | Konsolidasyon veri aralığı indeksi. |
| pageItemIndex | Int32[] | Her sayfa alanındaki sayfa öğesi indeksi. pageItemIndex[2] = 1, bu aralığı tanımlamak için üçüncü alandaki ikinci öğe anlamına gelir. pageItemIndex[1] = -1, ikinci alanda bu aralığı tanımlamak için öğe olmadığını ve MS'nin ikinci alanda bu aralığı tanımlamak için otomatik olarak "boş" öğe oluşturacağını gösterir. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotPageFieldsMethodAddIdentifyWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue("Data");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["A4"].PutValue(3);
            worksheet.Cells["B1"].PutValue("Category");
            worksheet.Cells["B2"].PutValue("A");
            worksheet.Cells["B3"].PutValue("B");
            worksheet.Cells["B4"].PutValue("C");

            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("A1:B4", "E5", "PivotTable");
            PivotTable pivotTable = pivotTables[pivotIndex];
            
            // PivotTable üzerinden erişmek yerine PivotPageFields'i doğrudan örnekle
            PivotPageFields pageFields = new PivotPageFields();

            try
            {
                pageFields.AddIdentify(0, new int[] { 0, 1 });
                Console.WriteLine("AddIdentify executed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            workbook.Save("PivotPageFieldsMethodAddIdentifyWithInt32Int32Demo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotPageFields](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


