---
title: "CellsHelper.RowIndexToName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CellsHelper yöntemi. Satır indeksine göre satır adını alır"
type: docs
url: /tr/net/aspose.cells/cellshelper/rowindextoname/
---
## CellsHelper.RowIndexToName method

Satır indeksine göre satır adını alır.

```csharp
public static string RowIndexToName(int row)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | Int32 | Satır indeksi. |

### Dönüş Değeri

Satır adı.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodRowIndexToNameWithInt32Demo
    {
        public static void Run()
        {
            int rowIndex = 10;
            string rowName = CellsHelper.RowIndexToName(rowIndex);
            Console.WriteLine("Row index {0} corresponds to row name: {1}", rowIndex, rowName);
            
            int convertedBackIndex = CellsHelper.RowNameToIndex(rowName);
            Console.WriteLine("Row name {0} converted back to index: {1}", rowName, convertedBackIndex);
        }
    }
}
```

### Ayrıca Bakınız

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


