---
title: "Sınıf CellValue"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.CellValue sınıfı. Hücre değerini ve ilgili türü temsil eder."
type: docs
url: /tr/net/aspose.cells/cellvalue/
---
## CellValue class

Hücre değerini ve ilgili türü temsil eder.

```csharp
public class CellValue
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [CellValue](cellvalue/)() | Varsayılan yapıcı. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Type](../../aspose.cells/cellvalue/type/) { get; set; } | Hücre değerinin türünü alır veya ayarlar. |
| [Value](../../aspose.cells/cellvalue/value/) { get; set; } | Hücre değerini alır veya ayarlar. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellValueDemo
    {
        public static void CellValueExample()
        {
            // Yeni bir çalışma kitabı oluşturun ve ilk çalışma sayfasını alın.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // CellValue örneği oluşturun.
            CellValue cellValue = new CellValue();

            // Hücrenin türünü ve değerini ayarlayın.
            cellValue.Type = CellValueType.IsNumeric;
            cellValue.Value = 123.45;

            // CellValue'yu çalışma sayfasındaki bir hücreye atayın
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue(cellValue.Value);

            // Çalışma kitabını kaydedin
            workbook.Save("CellValueExample.xlsx");
            workbook.Save("CellValueExample.pdf");
            return;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


