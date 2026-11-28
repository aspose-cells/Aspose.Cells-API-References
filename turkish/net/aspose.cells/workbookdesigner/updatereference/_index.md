---
title: "WorkbookDesigner.UpdateReference"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookDesigner özelliği. Diğer çalışma sayfalarındaki referansların güncellenip güncellenmeyeceğini gösterir"
type: docs
url: /tr/net/aspose.cells/workbookdesigner/updatereference/
---
## WorkbookDesigner.UpdateReference property

Diğer çalışma sayfalarındaki referansların güncellenip güncellenmeyeceğini gösterir.

```csharp
public bool UpdateReference { get; set; }
```

### Örnekler

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerPropertyUpdateReferenceDemo
    {
        public static void Run()
        {
            // Örnek bir veri kümesi oluştur
            DataSet ds = new DataSet();
            DataTable dt = new DataTable("Products");
            dt.Columns.Add("ID", typeof(int));
            dt.Columns.Add("Name", typeof(string));
            dt.Columns.Add("Price", typeof(decimal));
            
            dt.Rows.Add(1, "Product A", 19.99);
            dt.Rows.Add(2, "Product B", 29.99);
            dt.Rows.Add(3, "Product C", 39.99);
            
            ds.Tables.Add(dt);

            // Bir çalışma kitabı tasarımcısı oluşturun
            WorkbookDesigner designer = new WorkbookDesigner();
            
            // UpdateReference özelliğini true olarak ayarlayın
            designer.UpdateReference = true;
            
            // Şablonlu yeni bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Akıllı işaretçiler ekleyin
            worksheet.Cells["A1"].PutValue("&=Products.ID");
            worksheet.Cells["B1"].PutValue("&=Products.Name");
            worksheet.Cells["C1"].PutValue("&=Products.Price");
            
            designer.Workbook = workbook;
            designer.SetDataSource("Products", dt);
            
            // Tasarımcıyı işleyin
            designer.Process();
            
            // Sonucu kaydet
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


