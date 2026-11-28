---
title: "Cells.ImportGridView"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Bir grid görünümünü bu hücrelere aktarır"
type: docs
url: /tr/net/aspose.cells/cells/importgridview/
---
## Cells.ImportGridView method

Bu hücrelere bir ızgara görünümü aktarır.

```csharp
public int ImportGridView(GridView gridView, int firstRow, int firstColumn, 
    ImportTableOptions options)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| gridView | GridView | Grid view nesnesi. |
| firstRow | Int32 | İçe aktarılacak ilk hücrenin satır numarası. |
| firstColumn | Int32 | İçe aktarılacak ilk hücrenin sütun numarası. |
| seçenekler | ImportTableOptions | İçe aktarma seçenekleri. |

### Dönüş Değeri

Satır numarası.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Data;

    public class CellsMethodImportGridViewWithGridViewInt32Int32ImportTableOptiDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // GridView verilerini taklit etmek için bir DataTable oluşturun
            DataTable dataTable = new DataTable();
            dataTable.Columns.Add("Name");
            dataTable.Columns.Add("Price");
            dataTable.Columns.Add("Stock");

            dataTable.Rows.Add("Product A", 100.5, 50);
            dataTable.Rows.Add("Product B", 200.75, 30);
            dataTable.Rows.Add("Product C", 150.25, 75);

            try
            {
                // ImportTableOptions oluşturun
                ImportTableOptions options = new ImportTableOptions();
                options.IsFieldNameShown = true;
                options.InsertRows = true;

                // DataTable verilerini, B3 hücresinden (satır 2, sütun 1) başlayarak aktarın
                worksheet.Cells.ImportData(dataTable, 2, 1, options);

                Console.WriteLine("Data imported successfully starting at cell B3");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error importing data: {ex.Message}");
            }

            // Çalışma kitabını kaydedin
            workbook.Save("CellsMethodImportGridViewWithGridViewInt32Int32ImportTableOptiDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ImportTableOptions](../../importtableoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


