---
title: "WorkbookDesigner.UpdateEmptyStringAsNull"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookDesigner özelliği. Değer TRUE ise Null eklenecektir"
type: docs
url: /tr/net/aspose.cells/workbookdesigner/updateemptystringasnull/
---
## WorkbookDesigner.UpdateEmptyStringAsNull property

Eğer TRUE ise, değer "" olduğunda Null eklenecektir;

```csharp
public bool UpdateEmptyStringAsNull { get; set; }
```

### Örnekler

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerPropertyUpdateEmptyStringAsNullDemo
    {
        public static void Run()
        {
            // Boş dizgeler içeren örnek bir DataSet oluşturun
            DataSet ds = new DataSet();
            DataTable dt = new DataTable("Products");
            dt.Columns.Add("Name");
            dt.Columns.Add("Price");
            dt.Rows.Add("Laptop", "");
            dt.Rows.Add("", "999.99");
            ds.Tables.Add(dt);

            // Tasarımcı işaretçileriyle bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("&=$Products.Name");
            worksheet.Cells["B1"].PutValue("&=$Products.Price");

            // WorkbookDesigner'ı başlatın ve özellikleri ayarlayın
            WorkbookDesigner designer = new WorkbookDesigner();
            designer.Workbook = workbook;
            designer.UpdateEmptyStringAsNull = true; // This is the key property being demonstrated
            
            // Veri kaynağını ayarlayın ve işleyin
            designer.SetDataSource(ds.Tables["Products"]);
            designer.Process();

            // Sonuçları doğrulayın
            Console.WriteLine("A1 value: " + worksheet.Cells["A1"].StringValue); // Should show "Laptop"
            Console.WriteLine("B1 value: " + worksheet.Cells["B1"].StringValue); // Should show empty (null)
        }
    }
}
```

### Ayrıca Bakınız

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


