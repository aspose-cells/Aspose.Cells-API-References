---
title: "CellsFactory.CreateStyle"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CellsFactory yöntemi. Yeni bir stil oluşturur"
type: docs
url: /tr/net/aspose.cells/cellsfactory/createstyle/
---
## CellsFactory.CreateStyle method

Yeni bir stil oluşturur.

```csharp
public Style CreateStyle()
```

### Dönüş Değeri

Bir stil nesnesi döndürür.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class CellsFactoryMethodCreateStyleDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // CellsFactory kullanarak bir stil oluştur
            Style style = new CellsFactory().CreateStyle();
            
            // Stil için kenarlık özelliklerini ayarla
            style.SetBorder(BorderType.BottomBorder, CellBorderType.Thick, Color.Black);
            
            // Stili bir hücreye uygula
            workbook.Worksheets[0].Cells["A1"].Value = "Hello World";
            workbook.Worksheets[0].Cells["A1"].SetStyle(style);
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Style](../../style/)
* class [CellsFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


