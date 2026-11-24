---
title: "Workbook.CreateStyle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Workbook-Methode. Erstellt einen neuen Stil"
type: docs
url: /de/net/aspose.cells/workbook/createstyle/
---
## CreateStyle() {#createstyle}

Erstellt einen neuen Stil.

```csharp
public Style CreateStyle()
```

### Rückgabewert

Gibt ein Stilobjekt zurück.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCreateStyleDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Einen neuen Stil mit der CreateStyle-Methode erstellen
            Style newStyle = workbook.CreateStyle();
            
            // Stileigenschaften festlegen
            newStyle.Font.Name = "Arial";
            newStyle.Font.Size = 12;
            newStyle.Font.IsBold = true;
            newStyle.ForegroundColor = System.Drawing.Color.LightBlue;
            newStyle.Pattern = BackgroundType.Solid;
            newStyle.IsTextWrapped = true;
            
            // Stil-Flag erstellen und Flags setzen
            StyleFlag flag = new StyleFlag();
            flag.FontName = true;
            flag.FontSize = true;
            flag.FontBold = true;
            flag.CellShading = true;
            flag.WrapText = true;
            
            // Den Stil auf Zelle A1 anwenden
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("This text has a custom style with wrapping");
            worksheet.Cells.ApplyStyle(newStyle, flag);
            
            // Spalte automatisch anpassen
            worksheet.AutoFitColumn(0);
            
            // Speichere die Arbeitsmappe
            workbook.Save("CreateStyleDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [Style](../../style/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CreateStyle(bool) {#createstyle_1}

Erstellt einen neuen Stil.

```csharp
public Style CreateStyle(bool cloneDefaultStyle)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cloneDefaultStyle | Boolean | Gibt an, ob der Standardstil geklont wird |

### Rückgabewert

Gibt ein Stilobjekt zurück.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCreateStyleWithBooleanDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook wb = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // Erstelle einen neuen Stil (false = nicht vom Standardstil erben)
            Style style = wb.CreateStyle(false);
            style.Font.Color = System.Drawing.Color.Blue;
            style.Font.IsBold = true;
            
            // Wende den Stil auf eine Zelle an
            Cell cell = cells["A1"];
            cell.SetStyle(style);
            cell.PutValue("Styled Text");
            
            // Speichere die Arbeitsmappe
            wb.Save("CreateStyleDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [Style](../../style/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


