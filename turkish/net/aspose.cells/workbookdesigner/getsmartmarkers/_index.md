---
title: "WorkbookDesigner.GetSmartMarkers"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookDesigner yöntemi. Bir elektronik tabloda akıllı işaretçilerin bir koleksiyonunu döndürür"
type: docs
url: /tr/net/aspose.cells/workbookdesigner/getsmartmarkers/
---
## WorkbookDesigner.GetSmartMarkers method

Bir elektronik tabloda akıllı işaretçilerin bir koleksiyonunu döndürür.

```csharp
public string[] GetSmartMarkers()
```

### Dönüş Değeri

Akıllı işaretçilerin bir koleksiyonu

### Açıklamalar

Her çağrıda bir dize dizisi oluşturulur. Dizi sıralanır ve yinelenen değerler kaldırılır.

### Örnekler

```csharp
using System;
using System.Data;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerMethodGetSmartMarkersDemo
    {
        public static void Run()
        {
            // Bellekte örnek bir şablon dosyası oluşturun
            Workbook templateWorkbook = new Workbook();
            Cells cells = templateWorkbook.Worksheets[0].Cells;
            
            // Şablona akıllı işaretçiler ekleyin
            cells["A1"].PutValue("&=COLORS_TIMES.COLORS");
            cells["B1"].PutValue("&=COLORS_TIMES.TIMES");
            
            // Şablonu bellek akışına kaydet
            MemoryStream templateStream = new MemoryStream();
            templateWorkbook.Save(templateStream, SaveFormat.Xlsx);
            
            // WorkbookDesigner'ı şablonla başlat
            WorkbookDesigner designer = new WorkbookDesigner();
            designer.Workbook = new Workbook(templateStream);
            
            // Akıllı işaretçileri al ve göster
            string[] smartMarkers = designer.GetSmartMarkers();
            Console.WriteLine("Found smart markers:");
            foreach (string marker in smartMarkers)
            {
                Console.WriteLine(marker);
            }
            
            // Veri kaynağını hazırla
            DataTable data = new DataTable("COLORS_TIMES");
            data.Columns.Add("COLORS", typeof(string));
            data.Columns.Add("TIMES", typeof(DateTime));
            data.Rows.Add("red", DateTime.Now.AddDays(-1));
            data.Rows.Add("yellow", DateTime.Now);
            data.Rows.Add("green", DateTime.Now.AddDays(1));
            
            // Veri kaynağını ayarlayın ve işleyin
            designer.SetDataSource(data);
            designer.Process();
            
            // Sonucu kaydedin
            designer.Workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


