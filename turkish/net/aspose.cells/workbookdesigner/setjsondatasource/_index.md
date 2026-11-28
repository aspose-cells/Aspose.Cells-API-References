---
title: "WorkbookDesigner.SetJsonDataSource"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookDesigner yöntemi. json dize değerini akıllı işaretçilerin veri kaynağı olarak ayarlar"
type: docs
url: /tr/net/aspose.cells/workbookdesigner/setjsondatasource/
---
## WorkbookDesigner.SetJsonDataSource method

JSON dize değerini akıllı işaretçilerin veri kaynağı olarak ayarla.

```csharp
public void SetJsonDataSource(string name, string json)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| name | String | Tablonun adı. JSON değerinin bir nesneyi temsil etmesi durumunda, null olabilir. |
| json | String | Json dizesinin değeri. |

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerMethodSetJsonDataSourceWithStringStringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // A1 hücresine örnek işaretçi ekleyin
            worksheet.Cells["A1"].PutValue("&=$DataSource.Name");
            
            // Çalışma kitabı tasarımcısı oluştur
            WorkbookDesigner designer = new WorkbookDesigner();
            designer.Workbook = workbook;
            
            // Örnek JSON verisi
            string jsonData = "{\"Name\":\"John Doe\",\"Age\":30,\"City\":\"New York\"}";
            
            // JSON veri kaynağını ayarlayın
            designer.SetJsonDataSource("DataSource", jsonData);
            
            // İşaretçileri işleyin
            designer.Process();
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


