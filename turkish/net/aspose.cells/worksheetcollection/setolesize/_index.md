---
title: "WorksheetCollection.SetOleSize"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorksheetCollection yöntemi. Workbook dosyası Ole nesnesi olarak kullanıldığında görüntülenen boyutu ayarlar"
type: docs
url: /tr/net/aspose.cells/worksheetcollection/setolesize/
---
## WorksheetCollection.SetOleSize method

Workbook dosyası Ole nesnesi olarak kullanıldığında görüntülenen boyutu ayarlar.

```csharp
public void SetOleSize(int startRow, int endRow, int startColumn, int endColumn)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startRow | Int32 | Başlangıç satır indeksi. |
| endRow | Int32 | Bitiş satır indeksi. |
| startColumn | Int32 | Başlangıç sütun indeksi. |
| endColumn | Int32 | Bitiş sütun indeksi. |

### Açıklamalar

Bu yöntem genellikle ppt dosyasında veya doc dosyasında görüntü boyutunu ayarlamak için kullanılır.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodSetOleSizeWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Çalışma sayfaları için OLE boyutunu ayarla
            workbook.Worksheets.SetOleSize(0, 10, 0, 10);
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
            
            // OLE boyutunu doğrula
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            CellArea oleSize = (CellArea)loadedWorkbook.Worksheets.OleSize;
            Console.WriteLine("OLE Size - StartRow: {0}, EndRow: {1}, StartColumn: {2}, EndColumn: {3}", 
                oleSize.StartRow, oleSize.EndRow, oleSize.StartColumn, oleSize.EndColumn);
        }
    }
}
```

### Ayrıca Bakınız

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


