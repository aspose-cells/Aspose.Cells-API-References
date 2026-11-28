---
title: "Cell.IsRichText"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cell yöntemi. Bu hücrenin string değerinin zengin biçimlendirilmiş bir metin olup olmadığını gösterir"
type: docs
url: /tr/net/aspose.cells/cell/isrichtext/
---
## Cell.IsRichText method

Bu hücrenin dize değerinin zengin biçimlendirilmiş bir metin olup olmadığını gösterir.

```csharp
public bool IsRichText()
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodIsRichTextDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Zengin metin biçimlendirmeli bir hücre oluşturun
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Hello World");
            
            // Zengin metin biçimlendirmesini uygulayın
            FontSetting boldFont = cell.GetCharacters()[0];
            boldFont.Font.IsBold = true;
            
            FontSetting normalFont = cell.GetCharacters()[6];
            normalFont.Font.IsBold = false;
            
            // Hücrenin zengin metin içerip içermediğini kontrol edin
            bool isRichText = cell.IsRichText();
            Console.WriteLine("Is cell A1 rich text? " + isRichText);
            
            // Çalışma kitabını kaydedin
            workbook.Save("RichTextDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


