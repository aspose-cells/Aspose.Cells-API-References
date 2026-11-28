---
title: "Cell.IsCheckBoxStyle"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cell özelliği. Bu hücrenin bir onay kutusu olarak ayarlanıp ayarlanmadığını gösterir"
type: docs
url: /tr/net/aspose.cells/cell/ischeckboxstyle/
---
## Cell.IsCheckBoxStyle property

Bu hücrenin bir onay kutusu olarak ayarlanıp ayarlanmadığını gösterir.

```csharp
public bool IsCheckBoxStyle { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsCheckBoxStyleDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // B1 hücresine erişin ve onay kutusu stiline ayarlayın
            Cell cell = worksheet.Cells["B1"];
            cell.IsCheckBoxStyle = true;
            cell.PutValue(true);
            
            // A1 hücresine erişin ve bir değerle onay kutusu stiline ayarlayın
            cell = worksheet.Cells["A1"];
            cell.IsCheckBoxStyle = true;
            cell.PutValue(false);
            
            // Çalışma kitabını kaydedin
            workbook.Save("CheckBoxStyleDemo.xlsx");
            
            // Kaydedilmiş çalışma kitabını yükleyerek özellikleri doğrulayın
            Workbook loadedWorkbook = new Workbook("CheckBoxStyleDemo.xlsx");
            worksheet = loadedWorkbook.Worksheets[0];
            
            // B1'in onay kutusu stili olduğunu doğrulayın
            cell = worksheet.Cells["B1"];
            Console.WriteLine("Cell B1 IsCheckBoxStyle: " + cell.IsCheckBoxStyle);
            
            // B1'i onay kutusu olmayan stile değiştirin ve kaydedin
            cell.IsCheckBoxStyle = false;
            loadedWorkbook.Save("CheckBoxStyleDemo_Modified.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


