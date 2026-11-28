---
title: "Cell.Copy"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cell yöntemi. Bir kaynak hücreden verileri kopyalar"
type: docs
url: /tr/net/aspose.cells/cell/copy/
---
## Cell.Copy method

Bir kaynak hücreden verileri kopyalar.

```csharp
public void Copy(Cell cell)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cell | Cell | Kaynak [`Cell`](../) nesnesi. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodCopyWithCellDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Kaynak hücrede değerleri ve stilleri ayarla
            Cell sourceCell = cells["A1"];
            sourceCell.PutValue("Source Value");
            sourceCell.GetStyle().Font.IsBold = true;

            // Hedef hücre oluştur
            Cell destCell = cells["B1"];

            // Kaynaktan hedefe kopyala
            destCell.Copy(sourceCell);

            // Kopyayı doğrula
            Console.WriteLine("Destination cell value: " + destCell.StringValue);
            Console.WriteLine("Destination cell bold status: " + destCell.GetStyle().Font.IsBold);
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


