---
title: "WorksheetCollection.RefreshPivotTables"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorksheetCollection yöntemi. Excel dosyasındaki tüm PivotTable'ları yeniler"
type: docs
url: /tr/net/aspose.cells/worksheetcollection/refreshpivottables/
---
## RefreshPivotTables() {#refreshpivottables_1}

Excel dosyasındaki tüm PivotTables'ı yeniler.

```csharp
public void RefreshPivotTables()
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodRefreshPivotTablesDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Özet tablo için örnek veri oluştur
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B4"].PutValue(3000);

            // Pivot tablo ekle
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            Aspose.Cells.Pivot.PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(Aspose.Cells.Pivot.PivotFieldType.Data, 1);

            // Kaynak veriyi değiştir
            worksheet.Cells["B2"].PutValue(1500);
            worksheet.Cells["B3"].PutValue(2500);

            // Çalışma kitabındaki tüm pivot tablolarını yenile
            workbook.Worksheets.RefreshPivotTables();

            // Çalışma kitabını kaydedin
            workbook.Save("RefreshPivotTablesDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RefreshPivotTables(PivotTableRefreshOption) {#refreshpivottables}

Excel dosyasındaki tüm PivotTables'ı yeniler.

```csharp
public bool RefreshPivotTables(PivotTableRefreshOption option)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| seçenek | PivotTableRefreshOption | Pivot tablolarının veri kaynağını yenileme seçeneği. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class WorksheetCollectionMethodRefreshPivotTablesWithPivotTableRefreshOptionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            cells["A1"].Value = "Category";
            cells["A2"].Value = "Fruit";
            cells["A3"].Value = "Vegetable";
            cells["B1"].Value = "Sales";
            cells["B2"].Value = 1500;
            cells["B3"].Value = 2300;

            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:B3", "E5", "SalesPivot");
            PivotTable pivotTable = pivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            PivotTableRefreshOption option = new PivotTableRefreshOption();

            workbook.Worksheets.RefreshPivotTables(option);

            Console.WriteLine(cells["F8"].StringValue);

            cells["B2"].Value = 2000;

            workbook.Worksheets.RefreshPivotTables(option);
            Console.WriteLine(cells["F8"].StringValue);
                       


            workbook.Save("WorksheetCollectionMethodRefreshPivotTablesWithPivotTableRefreshOptionDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotTableRefreshOption](../../../aspose.cells.pivot/pivottablerefreshoption/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


