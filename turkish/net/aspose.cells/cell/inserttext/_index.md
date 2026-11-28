---
title: "Cell.InsertText"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cell yöntemi. Hücreye bazı karakterler ekle. Hücre zengin biçimlendirilmişse bu yöntem orijinal biçimlendirmeyi koruyabilir"
type: docs
url: /tr/net/aspose.cells/cell/inserttext/
---
## Cell.InsertText method

Hücreye bazı karakterler ekler. Hücre zengin biçimlendirilmişse, bu yöntem orijinal biçimlendirmeyi koruyabilir.

```csharp
public void InsertText(int index, string text)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| indeks | Int32 | İndeks. |
| metin | String | Eklenmiş metin. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodInsertTextWithInt32StringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // B3 hücresine eriş ve başlangıç değerini ayarla.
            Cell cell = worksheet.Cells["B3"];
            cell.PutValue("OriginalText");
            
            // Metni 6. konuma ekle.
            cell.InsertText(6, "Inserted");
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


