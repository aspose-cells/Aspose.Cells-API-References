---
title: "CellsHelper.ColumnNameToIndex"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CellsHelper yöntemi. Sütun adına göre sütun indeksini alır"
type: docs
url: /tr/net/aspose.cells/cellshelper/columnnametoindex/
---
## CellsHelper.ColumnNameToIndex method

Sütun adına göre sütun indeksini alır.

```csharp
public static int ColumnNameToIndex(string columnName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| columnName | String | Sütun adı. |

### Dönüş Değeri

Sütun indeksi.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodColumnNameToIndexWithStringDemo
    {
        public static void Run()
        {
            int columnIndex = CellsHelper.ColumnNameToIndex("BAA");
            string columnName = CellsHelper.ColumnIndexToName(columnIndex);
            
            Console.WriteLine("Column Name: " + columnName);
            Console.WriteLine("Column Index: " + columnIndex);
        }
    }
}
```

### Ayrıca Bakınız

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


