---
title: "Cell.GetHtmlString"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cell yöntemi. Bu hücredeki veri ve bazı biçimlendirmeleri içeren html dizesini alır"
type: docs
url: /tr/net/aspose.cells/cell/gethtmlstring/
---
## Cell.GetHtmlString method

Bu hücredeki veri ve bazı biçimleri içeren html dizesini al.

```csharp
public string GetHtmlString(bool html5)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| html5 | Boolean | Değerin html5 ile uyumlu olup olmadığını gösterir |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetHtmlStringWithBooleanDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Biçimlendirme ile örnek hücre değerini ayarlayın
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text");
            Style style = cell.GetStyle();
            style.Font.Name = "Calibri";
            style.Font.Size = 11;
            style.Font.Color = System.Drawing.Color.Red;
            cell.SetStyle(style);

            // Boolean parametresiyle GetHtmlString yöntemini gösterin
            string htmlWithoutDiv = cell.GetHtmlString(false);
            string htmlWithDiv = cell.GetHtmlString(true);
            
            Console.WriteLine("HTML without div wrapper:");
            Console.WriteLine(htmlWithoutDiv);
            Console.WriteLine("\nHTML with div wrapper:");
            Console.WriteLine(htmlWithDiv);
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


