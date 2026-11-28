---
title: "Cells.MinDataRow"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells özelliği. Veri içeren hücrenin minimum satır indeksi"
type: docs
url: /tr/net/aspose.cells/cells/mindatarow/
---
## Cells.MinDataRow property

Veri içeren hücrenin minimum satır indeksi.

```csharp
public int MinDataRow { get; }
```

### Açıklamalar

Veri içeren hücre yoksa -1 döndürür. Bu özellik hücreleri ve satırları dinamik olarak yinelemek ve kontrol etmek gerektiğinden zaman alıcı bir işlemdir ve bir döngüde doğrudan koşul olarak kullanmak gibi tekrarlı çağrılmamalıdır.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyMinDataRowDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Bazı verileri doldurun
            sheet.Cells[0, 0].Value = "Header1";
            sheet.Cells[0, 1].Value = "Header2";
            sheet.Cells[1, 0].Value = "Data1";
            sheet.Cells[1, 1].Value = "Data2";
            sheet.Cells[2, 0].Value = "Data3";
            sheet.Cells[2, 1].Value = "Data4";

            // MinDataRow kullanımını göster
            Console.WriteLine("Minimum data row index: " + sheet.Cells.MinDataRow);
            Console.WriteLine("Maximum data row index: " + sheet.Cells.MaxDataRow);

            // Çalışma kitabını kaydedin
            workbook.Save("MinDataRowExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


