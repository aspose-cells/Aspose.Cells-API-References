---
title: "Style.Copy"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Style yöntemi. Başka bir stil nesnesinden verileri kopyalar"
type: docs
url: /tr/net/aspose.cells/style/copy/
---
## Style.Copy method

Başka bir stil nesnesinden verileri kopyalar.

```csharp
public void Copy(Style style)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stil | Stil | Kaynak Style nesnesi |

### Açıklamalar

Bu yöntem stilin adını kopyalamaz. Adı kopyalamak istiyorsanız, stil kopyalandıktan sonra aşağıdaki kodları çağırın: destStyle.Name = style.Name.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleMethodCopyWithStyleDemo
    {
        public static void Run()
        {
            // Örnek veri içeren kaynak çalışma kitabını oluşturun
            Workbook srcWorkbook = new Workbook();
            Worksheet srcSheet = srcWorkbook.Worksheets[0];
            srcSheet.Cells["A1"].PutValue("Sample Text");
            Style srcStyle = srcWorkbook.CreateStyle();
            srcStyle.Font.Name = "Arial";
            srcStyle.Font.Size = 14;
            srcSheet.Cells["A1"].SetStyle(srcStyle);

            // Hedef çalışma kitabı oluştur
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets[0];
            
            // Stili kaynaktan hedefe kopyalayın
            Style destStyle = destWorkbook.CreateStyle();
            destStyle.Copy(srcStyle);
            
            // Kopyalanan stili uygulayın
            destSheet.Cells["B2"].PutValue("Copied Style Text");
            destSheet.Cells["B2"].SetStyle(destStyle);

            // Sonucu kaydet
            destWorkbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


