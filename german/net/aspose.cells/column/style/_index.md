---
title: "Column.Style"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Column-Eigenschaft. Gibt den Stil dieser Spalte zurück"
type: docs
url: /de/net/aspose.cells/column/style/
---
## Column.Style property

Ermittelt den Stil dieser Spalte.

```csharp
[Obsolete("Use Column.GetStyle() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public Style Style { get; }
```

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Methode Column.GetStyle(), um den Standardstil dieser Spalte zu erhalten. Diese Eigenschaft wird 12 Monate nach Dezember 2022 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class ColumnPropertyStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Greifen Sie auf die erste Spalte zu
            Column column = worksheet.Cells.Columns[0];
            
            // Aktuelle Formatierung mit der Style-Eigenschaft abrufen
            Style originalStyle = column.Style;
            Console.WriteLine("Original column style - Background: " + originalStyle.BackgroundColor);
            
            // Neue Formatierung erstellen und Eigenschaften ändern
            Style newStyle = workbook.CreateStyle();
            newStyle.BackgroundColor = Color.LightBlue;
            newStyle.Font.IsBold = true;
            newStyle.HorizontalAlignment = TextAlignmentType.Center;
            
            // Neue Formatierung auf die Spalte anwenden
            column.SetStyle(newStyle);
            
            // Daten hinzufügen, um die Anwendung der Formatierung zu demonstrieren
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Data 1");
            worksheet.Cells["A3"].PutValue("Data 2");
            
            // Formatierungsänderungen überprüfen
            Console.WriteLine("New column style applied - Background: " + column.GetStyle().BackgroundColor);
            
            // Speichern mit Anpassung der Spaltenbreite
            column.Width = 15;
            workbook.Save("ColumnStyleDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Style](../../style/)
* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


