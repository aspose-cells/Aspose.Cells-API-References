---
title: "Cell.IsTableFormula"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cell özelliği. Bu hücrenin tablo formülünün bir parçası olup olmadığını gösterir"
type: docs
url: /tr/net/aspose.cells/cell/istableformula/
---
## Cell.IsTableFormula property

Bu hücrenin tablo formülünün bir parçası olup olmadığını gösterir.

```csharp
public bool IsTableFormula { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class CellPropertyIsTableFormulaDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Bir tablo oluştur
            int index = worksheet.ListObjects.Add(0, 0, 5, 3, true);
            ListObject table = worksheet.ListObjects[index];
            
            // D2 hücresine tablo formülü ekle
            Cell cell = worksheet.Cells["D2"];
            cell.Formula = "=SUM(Table1[[#This Row],[Column1]:[Column3]])";
            
            // Hücrenin tablo formülü içerip içermediğini kontrol et
            Console.WriteLine("Is table formula: " + cell.IsTableFormula);
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


