---
title: "Klasse CellValue"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.CellValue Klasse. Stellt den Zellenwert und den entsprechenden Typ dar"
type: docs
url: /de/net/aspose.cells/cellvalue/
---
## CellValue class

Stellt den Zellenwert und den entsprechenden Typ dar.

```csharp
public class CellValue
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [CellValue](cellvalue/)() | Der Standardkonstruktor. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Type](../../aspose.cells/cellvalue/type/) { get; set; } | Liest oder setzt den Typ des Zellenwerts. |
| [Value](../../aspose.cells/cellvalue/value/) { get; set; } | Liest oder setzt den Zellenwert. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellValueDemo
    {
        public static void CellValueExample()
        {
            // Erstellen Sie eine neue Arbeitsmappe und rufen Sie das erste Arbeitsblatt ab
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstellen Sie eine CellValue‑Instanz
            CellValue cellValue = new CellValue();

            // Setzen Sie den Typ und den Wert der Zelle
            cellValue.Type = CellValueType.IsNumeric;
            cellValue.Value = 123.45;

            // Weisen Sie den CellValue einer Zelle im Arbeitsblatt zu
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue(cellValue.Value);

            // Speichere die Arbeitsmappe
            workbook.Save("CellValueExample.xlsx");
            workbook.Save("CellValueExample.pdf");
            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


