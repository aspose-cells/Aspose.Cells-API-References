---
title: "Column.Style"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Column-egenskap. Hämtar stilen för den här kolumnen"
type: docs
url: /sv/net/aspose.cells/column/style/
---
## Column.Style property

Hämtar stilen för den här kolumnen.

```csharp
[Obsolete("Use Column.GetStyle() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public Style Style { get; }
```

### Anmärkningar

OBS: Detta medlem är nu föråldrad. Använd istället Column.GetStyle()‑metoden för att hämta standardstilen för den här kolumnen. Denna egenskap kommer att tas bort 12 månader senare sedan december 2022. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

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
            
            // Åtkomst till den första kolumnen
            Column column = worksheet.Cells.Columns[0];
            
            // Hämta aktuell stil med Style‑egenskapen
            Style originalStyle = column.Style;
            Console.WriteLine("Original column style - Background: " + originalStyle.BackgroundColor);
            
            // Skapa ny stil och ändra egenskaper
            Style newStyle = workbook.CreateStyle();
            newStyle.BackgroundColor = Color.LightBlue;
            newStyle.Font.IsBold = true;
            newStyle.HorizontalAlignment = TextAlignmentType.Center;
            
            // Applicera ny stil på kolumnen
            column.SetStyle(newStyle);
            
            // Lägg till data för att demonstrera stiltillämpning
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Data 1");
            worksheet.Cells["A3"].PutValue("Data 2");
            
            // Verifiera stiländringar
            Console.WriteLine("New column style applied - Background: " + column.GetStyle().BackgroundColor);
            
            // Spara med justering av kolumnbredd
            column.Width = 15;
            workbook.Save("ColumnStyleDemo.xlsx");
        }
    }
}
```

### Se även

* class [Style](../../style/)
* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


