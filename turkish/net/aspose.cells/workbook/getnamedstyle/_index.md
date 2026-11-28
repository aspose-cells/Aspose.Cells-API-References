---
title: "Workbook.GetNamedStyle"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Workbook yöntemi. Stil havuzundaki adlandırılmış stili alır"
type: docs
url: /tr/net/aspose.cells/workbook/getnamedstyle/
---
## Workbook.GetNamedStyle method

Stil havuzundaki adlandırılmış stili alır.

```csharp
public Style GetNamedStyle(string name)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| name | String | stilin adı |

### Dönüş Değeri

adlandırılmış stil, null olabilir.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using System.Data;

namespace AsposeCellsExamples
{
    public class WorkbookMethodGetNamedStyleWithStringDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Bazı adlandırılmış stiller ekle
            Style style1 = workbook.CreateStyle();
            style1.Name = "Number7";
            style1.Custom = "#,##0.00";
            
            Style style2 = workbook.CreateStyle();
            style2.Name = "Center";
            style2.HorizontalAlignment = TextAlignmentType.Center;
            
            // Örnek veri oluştur
            DataTable dt = new DataTable();
            dt.Columns.Add("ProductID", typeof(int));
            dt.Columns.Add("ProductName", typeof(string));
            dt.Columns.Add("Quantity", typeof(int));
            dt.Columns.Add("UnitPrice", typeof(decimal));
            dt.Columns.Add("Discount", typeof(float));
            
            dt.Rows.Add(1, "Product A", 10, 19.99m, 0.1f);
            dt.Rows.Add(2, "Product B", 5, 29.99m, 0.15f);
            
            // Çalışma sayfasını ve hücreleri al
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Adlandırılmış stilleri al
            Style numberStyle = workbook.GetNamedStyle("Number7");
            Style centerStyle = workbook.GetNamedStyle("Center");
            
            // Stilleri veriye uygula
            for(int i = 0; i < dt.Rows.Count; i++)
            {
                cells[i, 0].PutValue((int)dt.Rows[i]["ProductID"]);
                cells[i, 0].SetStyle(centerStyle);
                
                cells[i, 1].PutValue((string)dt.Rows[i]["ProductName"]);
                
                cells[i, 3].PutValue((decimal)dt.Rows[i]["UnitPrice"]);
                cells[i, 3].SetStyle(numberStyle);
            }
            
            // Çalışma kitabını kaydedin
            workbook.Save("GetNamedStyleDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Style](../../style/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


