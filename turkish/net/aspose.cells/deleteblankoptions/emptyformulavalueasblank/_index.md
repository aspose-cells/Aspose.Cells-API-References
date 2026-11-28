---
title: "DeleteBlankOptions.EmptyFormulaValueAsBlank"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DeleteBlankOptions özelliği. Bir hücre formül olduğunda ve hesaplanan sonuç null ya da boş dize olduğunda boş olarak kabul edilip edilmeyeceği. Varsayılan değer false'tur."
type: docs
url: /tr/net/aspose.cells/deleteblankoptions/emptyformulavalueasblank/
---
## DeleteBlankOptions.EmptyFormulaValueAsBlank property

Bir hücrenin formül olduğu ve hesaplanan sonucun null ya da boş dize olduğu durumda boş olarak kabul edilip edilmeyeceği. Varsayılan değer false.

```csharp
public bool EmptyFormulaValueAsBlank { get; set; }
```

### Açıklamalar

Genel olarak, kullanıcı bu özellik true iken silme işleminden önce formüllerin hesaplandığından emin olmalıdır. Aksi takdirde, normal API'ler aracılığıyla yeni oluşturulan ve [`Formula`](../../cell/formula/) gibi formüller boş olarak kabul edilir ve silinebilir, çünkü hesaplamadan önce hesaplanan sonuçları null'dur.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DeleteBlankOptionsPropertyEmptyFormulaValueAsBlankDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;

            // Örnek verileri doldur
            cells["A1"].PutValue("Header");
            cells["A2"].Formula = "=B2";  // Formula returning blank
            cells["A3"].PutValue("Data");
            cells["A4"].Formula = "=1+1"; // Formula with value
            
            // Formül boşluklarını dikkate almadan boş satırları sil
            Console.WriteLine("Before deletion (normal): " + cells.MaxRow + " rows");
            cells.DeleteBlankRows();
            Console.WriteLine("After normal deletion: " + cells.MaxRow + " rows");

            // Verileri sıfırla
            cells.ClearContents(0, 0, cells.MaxRow + 1, cells.MaxColumn + 1);
            cells["A1"].PutValue("Header");
            cells["A2"].Formula = "=B2";
            cells["A3"].PutValue("Data");
            cells["A4"].Formula = "=1+1";

            // Formül boşluklarını boş olarak kabul ederek boş satırları sil
            Console.WriteLine("\nBefore deletion (with EmptyFormulaValueAsBlank): " + cells.MaxRow + " rows");
            cells.DeleteBlankRows(new DeleteBlankOptions() { EmptyFormulaValueAsBlank = true });
            Console.WriteLine("After deletion with EmptyFormulaValueAsBlank: " + cells.MaxRow + " rows");
        }
    }
}
```

### Ayrıca Bakınız

* class [DeleteBlankOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


