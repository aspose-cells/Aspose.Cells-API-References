---
title: "Cells.RemoveFormulas"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Tüm formülleri kaldırır ve formülün değeriyle değiştirir"
type: docs
url: /tr/net/aspose.cells/cells/removeformulas/
---
## Cells.RemoveFormulas method

Tüm formülleri kaldırır ve formülün değeriyle değiştirir.

```csharp
public void RemoveFormulas()
```

### Örnekler

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodRemoveFormulasDemo
    {
        public static void Run()
        {
            // Örnek bir veri kümesi oluştur
            DataSet ds = new DataSet();

            // Master tablosunu oluştur ve doldur
            DataTable dtMaster = new DataTable("Master");
            dtMaster.Columns.Add("ACCOUNT", typeof(string));
            dtMaster.Columns.Add("ACCOUNT_CREATEDBY_NAME", typeof(string));
            dtMaster.Rows.Add("Test_Account", "Test_user");
            ds.Tables.Add(dtMaster);

            // OppLineItems tablosunu oluştur ve doldur
            DataTable lineItems = new DataTable("OppLineItems");
            lineItems.Columns.Add("Id", typeof(int));
            lineItems.Columns.Add("Name", typeof(string));
            lineItems.Columns.Add("SALESPRICE", typeof(int));
            lineItems.Rows.Add(1, "lineItem1", 10);
            lineItems.Rows.Add(2, "lineItem2", 20);
            ds.Tables.Add(lineItems);

            // Yeni bir çalışma kitabı oluştur
            Workbook wkb = new Workbook();
            
            // Veri bağlamak için WorkbookDesigner'ı kullan
            WorkbookDesigner designer = new WorkbookDesigner { Workbook = wkb };
            designer.SetDataSource(ds);
            designer.Process(false);

            // Kaldırmayı göstermek için bir formül ekle
            wkb.Worksheets[0].Cells["A10"].Formula = "=SUM(C2:C3)";
            
            // Önce formülleri hesapla
            wkb.CalculateFormula();

            // Çalışma sayfasındaki tüm formülleri kaldır
            wkb.Worksheets[0].Cells.RemoveFormulas();

            // Çalışma kitabını kaydedin
            wkb.Save("output.xlsx");
            
            Console.WriteLine("Formulas removed and workbook saved successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


