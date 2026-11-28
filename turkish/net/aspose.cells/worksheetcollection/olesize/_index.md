---
title: "WorksheetCollection.OleSize"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorksheetCollection özelliği. Workbook dosyası Ole nesnesi olarak kullanıldığında görüntülenen boyutu alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/worksheetcollection/olesize/
---
## WorksheetCollection.OleSize property

Workbook dosyası bir Ole nesnesi olarak kullanıldığında görüntülenen boyutu alır ve ayarlar.

```csharp
public object OleSize { get; set; }
```

### Açıklamalar

Null, ole boyut ayarı olmadığını ifade eder.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyOleSizeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Worksheet collection için OLE boyutunu ayarla
            workbook.Worksheets.SetOleSize(0, 10, 0, 10);
            
            // OLE boyut özelliklerine eriş ve görüntüle
            CellArea oleSize = (CellArea)workbook.Worksheets.OleSize;
            Console.WriteLine("OLE Size Range:");
            Console.WriteLine($"StartRow: {oleSize.StartRow}, EndRow: {oleSize.EndRow}");
            Console.WriteLine($"StartColumn: {oleSize.StartColumn}, EndColumn: {oleSize.EndColumn}");
            
            // Çalışma kitabını kaydedin
            workbook.Save("OleSizeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


