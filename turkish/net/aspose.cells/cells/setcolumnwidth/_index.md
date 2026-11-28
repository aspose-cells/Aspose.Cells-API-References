---
title: "Cells.SetColumnWidth"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Belirtilen sütunun genişliğini normal görünümde ayarlar"
type: docs
url: /tr/net/aspose.cells/cells/setcolumnwidth/
---
## Cells.SetColumnWidth method

Normal görünümde belirtilen sütunun genişliğini ayarlar.

```csharp
public void SetColumnWidth(int column, double width)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sütun | Int32 | Sütun indeksi. |
| genişlik | Double | Sütun genişliği karakter biriminde. Sütun genişliği 0 ile 255 arasında olmalıdır. |

### Açıklamalar

Elektronik tablo için sütun genişliği, normal stilin yazı tipinde 0~9 sayılarının maksimum rakam genişliğinin karakter sayısı olarak ölçülür.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodSetColumnWidthWithInt32DoubleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            cells.SetColumnWidth(0, 25.5);
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


