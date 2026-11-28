---
title: "TableStyleCollection.DefaultTableStyleName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TableStyleCollection özelliği. Tablonun varsayılan stil adını alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.tables/tablestylecollection/defaulttablestylename/
---
## TableStyleCollection.DefaultTableStyleName property

Tablonun varsayılan stil adını alır ve ayarlar.

```csharp
public string DefaultTableStyleName { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class TableStyleCollectionPropertyDefaultTableStyleNameDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Tablo stilleri koleksiyonuna eriş
            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;
            
            // Varsayılan tablo stilinin adını görüntüle
            Console.WriteLine("Default Table Style: " + tableStyles.DefaultTableStyleName);
            
            // Varsayılan tablo stilini değiştir
            tableStyles.DefaultTableStyleName = "TableStyleMedium9";
            Console.WriteLine("New Default Table Style: " + tableStyles.DefaultTableStyleName);
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [TableStyleCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


