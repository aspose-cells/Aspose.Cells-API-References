---
title: "TableStyleCollection.DefaultPivotStyleName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TableStyleCollection özelliği. Pivot tablonun varsayılan stil adını alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.tables/tablestylecollection/defaultpivotstylename/
---
## TableStyleCollection.DefaultPivotStyleName property

Özet tablonun varsayılan stil adını alır ve ayarlar.

```csharp
public string DefaultPivotStyleName { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class TableStyleCollectionPropertyDefaultPivotStyleNameDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Tablo stilleri koleksiyonuna eriş
            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;
            
            // Varsayılan pivot stil adını göster
            Console.WriteLine("Default Pivot Style: " + tableStyles.DefaultPivotStyleName);
            
            // Varsayılan pivot stilini değiştir
            tableStyles.DefaultPivotStyleName = "PivotStyleDark2";
            
            // Değişikliği doğrulayın
            Console.WriteLine("Updated Default Pivot Style: " + tableStyles.DefaultPivotStyleName);
            
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


