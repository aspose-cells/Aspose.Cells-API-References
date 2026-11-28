---
title: "Cell.Characters"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cell yöntemi. Hücre metni içindeki bir karakter aralığını temsil eden bir Characters nesnesi döndürür"
type: docs
url: /tr/net/aspose.cells/cell/characters/
---
## Cell.Characters method

Hücre metni içindeki bir karakter aralığını temsil eden bir Characters nesnesi döndürür.

```csharp
public FontSetting Characters(int startIndex, int length)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startIndex | Int32 | Karakterin başlangıç indeksidir. |
| uzunluk | Int32 | Karakter sayısı. |

### Dönüş Değeri

Karakterler nesnesi.

### Açıklamalar

Bu yöntem yalnızca dize değeri olan hücrelerde çalışır.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class CellMethodCharactersWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            cells["A1"].PutValue("Helloworld");
            cells["A1"].Characters(5, 5).Font.IsBold = true;
            cells["A1"].Characters(5, 5).Font.Color = Color.Blue;
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [FontSetting](../../fontsetting/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


