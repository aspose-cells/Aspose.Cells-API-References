---
title: "WorkbookDesigner.SortDataSource"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookDesigner özelliği. Veri kaynağının sıralanıp sıralanmayacağını gösterir"
type: docs
url: /tr/net/aspose.cells/workbookdesigner/sortdatasource/
---
## WorkbookDesigner.SortDataSource property

Veri kaynağının sıralanıp sıralanmadığını gösterir.

```csharp
[EditorBrowsable(EditorBrowsableState.Never)]
public bool SortDataSource { get; set; }
```

### Açıklamalar

NOT: Bu özellik artık kullanımdan kaldırıldı. Bu özellik, Ekim 2026'dan itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler. Akıllı işaretçi artan ve azalan parametreler içeriyorsa Json veri kaynağı sıralanmış olur.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Data;

    public class WorkbookDesignerPropertySortDataSourceDemo
    {
        public static void Run()
        {
            // Sıralanmamış verilerle örnek bir DataTable oluştur
            DataTable dataTable = new DataTable("Products");
            dataTable.Columns.Add("ProductID", typeof(int));
            dataTable.Columns.Add("ProductName", typeof(string));
            dataTable.Columns.Add("Price", typeof(decimal));

            // Örnek verileri sıralanmamış sırayla ekle
            dataTable.Rows.Add(3, "Product C", 15.99m);
            dataTable.Rows.Add(1, "Product A", 10.50m);
            dataTable.Rows.Add(2, "Product B", 12.75m);

            // Akıllı işaretçilerle bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasında akıllı işaretçileri ayarlayın
            worksheet.Cells["A1"].PutValue("&=$ProductID");
            worksheet.Cells["B1"].PutValue("&=$ProductName");
            worksheet.Cells["C1"].PutValue("&=$Price");

            try
            {
                // WorkbookDesigner örneği oluştur
                WorkbookDesigner designer = new WorkbookDesigner(workbook);

                // İlk SortDataSource değerini göster
                Console.WriteLine($"Initial SortDataSource value: {designer.SortDataSource}");

                // Veri kaynağını sıralama olmadan ayarla
                designer.SortDataSource = false;
                designer.SetDataSource(dataTable);
                designer.Process();

                // Sıralanmamış sonucu kaydet
                workbook.Save("UnsortedOutput.xlsx");
                Console.WriteLine("Unsorted data saved to UnsortedOutput.xlsx");

                // Sıralı gösterim için yeni bir çalışma kitabı oluştur
                Workbook sortedWorkbook = new Workbook();
                Worksheet sortedSheet = sortedWorkbook.Worksheets[0];
                sortedSheet.Cells["A1"].PutValue("&=$ProductID");
                sortedSheet.Cells["B1"].PutValue("&=$ProductName");
                sortedSheet.Cells["C1"].PutValue("&=$Price");

                // Sıralama etkinleştirilmiş yeni bir tasarımcı oluştur
                WorkbookDesigner sortedDesigner = new WorkbookDesigner(sortedWorkbook);
                sortedDesigner.SortDataSource = true;
                sortedDesigner.SetDataSource(dataTable);
                sortedDesigner.Process();

                // Sıralı sonucu kaydet
                sortedWorkbook.Save("SortedOutput.xlsx");
                Console.WriteLine("Sorted data saved to SortedOutput.xlsx");
                Console.WriteLine($"Final SortDataSource value: {sortedDesigner.SortDataSource}");
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

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


