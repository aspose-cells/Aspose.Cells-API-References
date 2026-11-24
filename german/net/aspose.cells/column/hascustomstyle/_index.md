---
title: "Column.HasCustomStyle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Column-Eigenschaft. Gibt an, ob diese Spalte benutzerdefinierte Formatierungseinstellungen hat, die sich vom standardmäßig von der Arbeitsmappe geerbten unterscheiden."
type: docs
url: /de/net/aspose.cells/column/hascustomstyle/
---
## Column.HasCustomStyle property

Gibt an, ob diese Spalte benutzerdefinierte Formatierungseinstellungen hat (anders als die standardmäßige, vom Arbeitsbuch geerbte).

```csharp
public bool HasCustomStyle { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class ColumnPropertyHasCustomStyleDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Greifen Sie auf die erste Spalte zu
            Column column = worksheet.Cells.Columns[0];

            // Anfangswert von HasCustomState anzeigen
            Console.WriteLine("Initial HasCustomStyle: " + column.HasCustomStyle);

            // Spaltenformatierung ändern, um die Änderung von HasCustomStyle zu demonstrieren
            Style columnStyle = column.GetStyle();
            columnStyle.BackgroundColor = Color.LightBlue;
            column.SetStyle(columnStyle);

            // Aktualisierten HasCustomStyle-Wert anzeigen
            Console.WriteLine("After style modification - HasCustomStyle: " + column.HasCustomStyle);

            // Erstelle eine weitere Spalte mit Standardstil zum Vergleich
            Column secondColumn = worksheet.Cells.Columns[1];
            Console.WriteLine("Second column HasCustomStyle: " + secondColumn.HasCustomStyle);

            // Speichere die Arbeitsmappe
            workbook.Save("ColumnHasCustomStyleDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


