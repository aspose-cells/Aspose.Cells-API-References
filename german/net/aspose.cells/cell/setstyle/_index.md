---
title: "Cell.SetStyle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cell-Methode. Setzt den Zellenstil"
type: docs
url: /de/net/aspose.cells/cell/setstyle/
---
## SetStyle(Style) {#setstyle}

Setzt den Zellenstil.

```csharp
public void SetStyle(Style style)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Stil | Stil | Der Zellenstil. |

### Hinweise

Wenn die Rahmen-Einstellungen geändert werden, wird auch der Rahmen der angepassten Zellen aktualisiert.

### Beispiele

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

            // Erstellen Sie einen Stil und setzen Sie dessen Eigenschaften
            Style style = workbook.CreateStyle();
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = System.Drawing.Color.Yellow;

            // Wenden Sie den Stil auf Zelle B2 (1,1 im nullbasierten Index) an
            cells[1, 1].SetStyle(style);

            // Speichere die Arbeitsmappe
            workbook.Save("SetStyleDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [Style](../../style/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetStyle(Style, bool) {#setstyle_2}

Wendet die geänderte Eigenschaft des Stils auf die Zelle an.

```csharp
public void SetStyle(Style style, bool explicitFlag)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Stil | Stil | Der Zellenstil. |
| explicitFlag | Boolean | True, überschreibt nur Formatierungen, die explizit gesetzt sind. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodSetStyleWithStyleBooleanDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Stile direkt erstellen
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
            
            // Wenden Sie Stile mit der SetStyle-Methode auf Zellen an
            Cell cell1 = worksheet.Cells["A1"];
            cell1.PutValue("Styled Text 1");
            cell1.SetStyle(style1, true); // true to preserve existing style elements not defined in the new style
            
            Cell cell2 = worksheet.Cells["A2"];
            cell2.PutValue("Styled Text 2");
            cell2.SetStyle(style2, false); // false to overwrite all style elements
            
            // Speichere die Arbeitsmappe
            workbook.Save("SetStyleDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Style](../../style/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetStyle(Style, StyleFlag) {#setstyle_1}

Wendet den Zellenstil basierend auf Flags an.

```csharp
public void SetStyle(Style style, StyleFlag flag)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Stil | Stil | Der Zellenstil. |
| Flag | StyleFlag | Das Stil-Flag. |

### Beispiele

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
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Erstellen Sie einen Stil und setzen Sie dessen Eigenschaften
            Style style = workbook.CreateStyle();
            style.Font.Color = Color.Red;
            style.Name = "CustomStyle";

            // Erstellen Sie ein Stil-Flag und setzen Sie es, um alle Formatierungen anzuwenden
            StyleFlag flag = new StyleFlag();
            flag.All = true;

            // Zellen abrufen und den Wert auf A1 setzen
            Cells cells = sheet.Cells;
            Cell cell = cells["A1"];
            cell.PutValue("Sample Text");

            // Wenden Sie den Stil mit SetStyle auf die Zelle an
            cell.SetStyle(style, flag);

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [Style](../../style/)
* class [StyleFlag](../../styleflag/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


