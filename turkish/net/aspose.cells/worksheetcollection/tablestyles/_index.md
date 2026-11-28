---
title: "WorksheetCollection.TableStyles"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorksheetCollection özelliği. TableStyles nesnesini alır"
type: docs
url: /tr/net/aspose.cells/worksheetcollection/tablestyles/
---
## WorksheetCollection.TableStyles property

`TableStyles` nesnesini alır.

```csharp
public TableStyleCollection TableStyles { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyTableStylesDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Bazı çalışma sayfaları ekle
            workbook.Worksheets.Add("Sheet1");
            workbook.Worksheets.Add("Sheet2");
            
            // Tablo stilleri oluştur ve ekle
            int styleIndex1 = workbook.Worksheets.TableStyles.AddTableStyle("Style1");
            TableStyle style1 = workbook.Worksheets.TableStyles[styleIndex1];
            
            int styleIndex2 = workbook.Worksheets.TableStyles.AddTableStyle("Style2");
            TableStyle style2 = workbook.Worksheets.TableStyles[styleIndex2];
            
            // Tablo stillerinin sayısını göster
            Console.WriteLine("Table styles count: " + workbook.Worksheets.TableStyles.Count);
            
            // Bir stili kaldır
            workbook.Worksheets.TableStyles.RemoveAt(0);
            
            // Güncellenmiş sayıyı göster
            Console.WriteLine("Table styles count after removal: " + workbook.Worksheets.TableStyles.Count);
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [TableStyleCollection](../../../aspose.cells.tables/tablestylecollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


