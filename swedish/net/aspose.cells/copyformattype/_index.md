---
title: "Enum CopyFormatType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.CopyFormatType‑enum. Representerar typen av kopieringsformat när rader infogas"
type: docs
url: /sv/net/aspose.cells/copyformattype/
---
## CopyFormatType enumeration

Representerar typen av kopieringsformat när rader infogas.

```csharp
public enum CopyFormatType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| SameAsAbove | `0` | Formaterar på samma sätt som raden ovan. |
| SameAsBelow | `1` | Formaterar på samma sätt som raden nedan. |
| Clear | `2` | Rensar formatering. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CopyFormatTypeDemo
    {
        public static void CopyFormatTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fyll i några data i kalkylbladet
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["A3"].PutValue("Data2");

            // Skapa InsertOptions och ange CopyFormatType
            InsertOptions insertOptions = new InsertOptions();
            insertOptions.CopyFormatType = CopyFormatType.SameAsAbove;

            // Infoga en rad på den andra positionen med den angivna formattypen
            worksheet.Cells.InsertRows(1, 1, insertOptions);

            // Spara arbetsboken
            workbook.Save("CopyFormatTypeExample.xlsx");
            workbook.Save("CopyFormatTypeExample.pdf");
            return;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


