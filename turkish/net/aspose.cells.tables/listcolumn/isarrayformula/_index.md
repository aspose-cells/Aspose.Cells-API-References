---
title: "ListColumn.IsArrayFormula"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ListColumn özelliği. Formülün dizi formülü olup olmadığını gösterir"
type: docs
url: /tr/net/aspose.cells.tables/listcolumn/isarrayformula/
---
## ListColumn.IsArrayFormula property

Formülün dizi formülü olup olmadığını gösterir.

```csharp
public bool IsArrayFormula { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class ListColumnPropertyIsArrayFormulaDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir tablo oluşturmak için örnek veri ekle
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue(20);

            // Bir tablo/list nesnesi oluştur
            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject listObject = worksheet.ListObjects[tableIndex];

            // İkinci sütuna bir dizi formülü ekle
            listObject.ListColumns[1].Formula = "{=SUM(A2:A3*B2:B3)}";

            try
            {
                // IsArrayFormula özelliğine eriş (yalnızca okunabilir)
                bool isArrayFormula = listObject.ListColumns[1].IsArrayFormula;

                // Değeri göster
                Console.WriteLine("IsArrayFormula value: " + isArrayFormula);

                // Çalışma kitabını kaydedin
                workbook.Save("IsArrayFormulaDemo.xlsx");
                Console.WriteLine("Demo completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


