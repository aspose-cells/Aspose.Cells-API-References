---
title: "Cell.SetStyle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cell-metod. Ställer in cellstilen"
type: docs
url: /sv/net/aspose.cells/cell/setstyle/
---
## SetStyle(Style) {#setstyle}

Ställer in cellstilen.

```csharp
public void SetStyle(Style style)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| style | Stil | Cellstilen. |

### Anmärkningar

Om kantinställningarna ändras, kommer kanten på justeringsceller också att uppdateras.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodSetStyleWithStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Skapa en stil och ange dess egenskaper
            Style style = workbook.CreateStyle();
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = System.Drawing.Color.Yellow;

            // Applicera stilen på cell B2 (1,1 i nollbaserat index)
            cells[1, 1].SetStyle(style);

            // Spara arbetsboken
            workbook.Save("SetStyleDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [Style](../../style/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetStyle(Style, bool) {#setstyle_2}

Applicera den ändrade egenskapen för stilen på cellen.

```csharp
public void SetStyle(Style style, bool explicitFlag)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| style | Stil | Cellstilen. |
| explicitFlag | Boolean | True, endast skriva över formatering som är explicit inställd. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodSetStyleWithStyleBooleanDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa stilar direkt
            Style style1 = workbook.CreateStyle();
            style1.Name = "MyStyle1";
            style1.Font.Name = "Arial";
            style1.Font.Size = 12;
            style1.Font.IsBold = true;
            
            Style style2 = workbook.CreateStyle();
            style2.Name = "MyStyle2";
            style2.Font.Name = "Times New Roman";
            style2.Font.Size = 14;
            style2.Font.Color = System.Drawing.Color.Red;
            
            // Applicera stilar på celler med SetStyle-metoden
            Cell cell1 = worksheet.Cells["A1"];
            cell1.PutValue("Styled Text 1");
            cell1.SetStyle(style1, true); // true to preserve existing style elements not defined in the new style
            
            Cell cell2 = worksheet.Cells["A2"];
            cell2.PutValue("Styled Text 2");
            cell2.SetStyle(style2, false); // false to overwrite all style elements
            
            // Spara arbetsboken
            workbook.Save("SetStyleDemo.xlsx");
        }
    }
}
```

### Se även

* class [Style](../../style/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetStyle(Style, StyleFlag) {#setstyle_1}

Applicera cellstilen baserat på flaggor.

```csharp
public void SetStyle(Style style, StyleFlag flag)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| style | Stil | Cellstilen. |
| flagga | StyleFlag | Stilflaggan. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class CellMethodSetStyleWithStyleStyleFlagDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Skapa en stil och ange dess egenskaper
            Style style = workbook.CreateStyle();
            style.Font.Color = Color.Red;
            style.Name = "CustomStyle";

            // Skapa en stilflagga och sätt den för att tillämpa all formatering
            StyleFlag flag = new StyleFlag();
            flag.All = true;

            // Hämta celler och sätt värde till A1
            Cells cells = sheet.Cells;
            Cell cell = cells["A1"];
            cell.PutValue("Sample Text");

            // Applicera stilen på cellen med SetStyle
            cell.SetStyle(style, flag);

            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [Style](../../style/)
* class [StyleFlag](../../styleflag/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


