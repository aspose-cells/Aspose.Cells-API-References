---
title: "Workbook.SaveToStream"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Workbook yöntemi. Excel dosyasını bir MemoryStream nesnesine Excel97-2003 xls dosyası olarak kaydeder ve döndürür"
type: docs
url: /tr/net/aspose.cells/workbook/savetostream/
---
## Workbook.SaveToStream method

Excel dosyasını bir MemoryStream nesnesine Excel97-2003 xls dosyası olarak kaydeder ve döndürür.

```csharp
public MemoryStream SaveToStream()
```

### Dönüş Değeri

Bir xls Excel dosyası içeren MemoryStream nesnesi.

### Açıklamalar

Bu yöntem, Save yönteminin aynı işlevini sağlar ve çalışma kitabını yalnızca Excel97-2003 xls dosyası olarak kaydeder. Daha çok COM istemcilerinden çağırmak için kullanılır.

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodSaveToStreamDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook start = new Workbook();
            
            // İlk çalışma sayfasına eriş ve bazı örnek veriler ekle
            Worksheet worksheet = start.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);

            // Çalışma kitabını bellek akışına kaydet
            MemoryStream stream = start.SaveToStream();

            // Akıştan yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook(stream);

            // Yeni çalışma kitabını değiştir
            Worksheet newWorksheet = workbook.Worksheets[0];
            var area = CellArea.CreateCellArea(3, 0, 3, 1);
            newWorksheet.Cells.InsertRange(area, 3, ShiftType.Down, true);

            newWorksheet.Cells["A4"].PutValue("D");
            newWorksheet.Cells["B4"].PutValue(40);
            newWorksheet.Cells["A5"].PutValue("E");
            newWorksheet.Cells["B5"].PutValue(50);
            newWorksheet.Cells["A6"].PutValue("F");
            newWorksheet.Cells["B6"].PutValue(60);

            // Değiştirilmiş çalışma kitabını kaydet
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


