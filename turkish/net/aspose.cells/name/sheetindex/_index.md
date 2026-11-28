---
title: "Name.SheetIndex"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Name özelliği. Bu adın Workbook veya Worksheet'a ait olduğunu gösterir. 0  Global ad, aksi takdirde bir‑bazlı sayfa indeksidir"
type: docs
url: /tr/net/aspose.cells/name/sheetindex/
---
## Name.SheetIndex property

Bu adın Workbook'a mı yoksa Worksheet'e mi ait olduğunu gösterir. 0 = Küresel ad, aksi takdirde sayfa indeksi (bir tabanlı).

```csharp
public int SheetIndex { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NamePropertySheetIndexDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Bazı çalışma sayfaları ekle
            workbook.Worksheets.Add("Sheet1");
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Sheet2'de adlandırılmış bir aralık oluştur
            Worksheet sheet2 = workbook.Worksheets["Sheet2"];
            int index = workbook.Worksheets.Names.Add("MyNamedRange");
            Name name = workbook.Worksheets.Names[index];
            name.RefersTo = "=Sheet2!$A$1:$B$10";
            
            // Adlandırılmış aralığın sayfa indeksini göster
            Console.WriteLine("Sheet index of named range: " + name.SheetIndex);
            
            // Çalışma kitabını kaydedin
            workbook.Save("NamedRangeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


