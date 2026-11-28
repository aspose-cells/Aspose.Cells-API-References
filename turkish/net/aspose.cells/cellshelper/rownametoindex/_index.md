---
title: "CellsHelper.RowNameToIndex"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CellsHelper yöntemi. Satır adına göre satır indeksini alır"
type: docs
url: /tr/net/aspose.cells/cellshelper/rownametoindex/
---
## CellsHelper.RowNameToIndex method

Satır adına göre satır indeksini alır.

```csharp
public static int RowNameToIndex(string rowName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowName | String | Satır adı. |

### Dönüş Değeri

Satır indeksi.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodRowNameToIndexWithStringDemo
    {
        public static void Run()
        {
            string rowName = "11";
            int rowIndex = CellsHelper.RowNameToIndex(rowName);
            Console.WriteLine("Row name '{0}' converted to index: {1}", rowName, rowIndex);
        }
    }
}
```

### Ayrıca Bakınız

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


