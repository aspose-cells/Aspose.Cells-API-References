---
title: "Workbook.CreateStyle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Workbook-metod. Skapar en ny stil"
type: docs
url: /sv/net/aspose.cells/workbook/createstyle/
---
## CreateStyle() {#createstyle}

Skapar en ny stil.

```csharp
public Style CreateStyle()
```

### Returvärde

Returnerar ett stilobjekt.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCreateStyleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa en ny stil med metoden CreateStyle
            Style newStyle = workbook.CreateStyle();
            
            // Ställ in stilens egenskaper
            newStyle.Font.Name = "Arial";
            newStyle.Font.Size = 12;
            newStyle.Font.IsBold = true;
            newStyle.ForegroundColor = System.Drawing.Color.LightBlue;
            newStyle.Pattern = BackgroundType.Solid;
            newStyle.IsTextWrapped = true;
            
            // Skapa stilflagga och sätt flaggor
            StyleFlag flag = new StyleFlag();
            flag.FontName = true;
            flag.FontSize = true;
            flag.FontBold = true;
            flag.CellShading = true;
            flag.WrapText = true;
            
            // Applicera stilen på cell A1
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("This text has a custom style with wrapping");
            worksheet.Cells.ApplyStyle(newStyle, flag);
            
            // Anpassa kolumnen automatiskt
            worksheet.AutoFitColumn(0);
            
            // Spara arbetsboken
            workbook.Save("CreateStyleDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [Style](../../style/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CreateStyle(bool) {#createstyle_1}

Skapar en ny stil.

```csharp
public Style CreateStyle(bool cloneDefaultStyle)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cloneDefaultStyle | Boolean | Anger om standardstilen klonas |

### Returvärde

Returnerar ett stilobjekt.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCreateStyleWithBooleanDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook wb = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // Skapa en ny stil (false = ärva inte från standardstilen)
            Style style = wb.CreateStyle(false);
            style.Font.Color = System.Drawing.Color.Blue;
            style.Font.IsBold = true;
            
            // Tillämpa stilen på en cell
            Cell cell = cells["A1"];
            cell.SetStyle(style);
            cell.PutValue("Styled Text");
            
            // Spara arbetsboken
            wb.Save("CreateStyleDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [Style](../../style/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


