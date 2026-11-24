---
title: "Cell.GetDisplayStyle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cell-Methode. Gibt den Anzeigestil dieser Zelle zurück"
type: docs
url: /de/net/aspose.cells/cell/getdisplaystyle/
---
## GetDisplayStyle() {#getdisplaystyle}

Ermittelt den Anzeigestil dieser Zelle.

```csharp
public Style GetDisplayStyle()
```

### Rückgabewert

Anzeigestil dieser Zelle

### Hinweise

Entspricht der Verwendung von SideBorders für `GetDisplayStyle`. Das bedeutet, dass diese Methode die oberen/unteren/linken/rechten Ränder dieser Zelle anhand des Stils ([`GetStyle`](../getstyle/)) ihrer benachbarten Zellen prüft und anpasst, jedoch nicht die zusammengeführten Zellen prüft und nicht den Anzeigestil der benachbarten Zellen prüft.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class CellMethodGetDisplayStyleDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Stil für Zelle A1 festlegen
            Style style1 = workbook.CreateStyle();
            style1.ForegroundColor = Color.FromArgb(157, 195, 230);
            worksheet.Cells["A1"].SetStyle(style1);
            
            // Stil für Zelle A23 festlegen
            Style style2 = workbook.CreateStyle();
            style2.ForegroundColor = Color.Red;
            worksheet.Cells["A23"].SetStyle(style2);
            
            // Stile abrufen und anzeigen
            Style displayStyle1 = worksheet.Cells["A1"].GetDisplayStyle();
            Console.WriteLine("A1 Foreground Color: " + displayStyle1.ForegroundColor);
            
            Style displayStyle2 = worksheet.Cells["A23"].GetDisplayStyle();
            Console.WriteLine("A23 Foreground Color: " + displayStyle2.ForegroundColor);
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

## GetDisplayStyle(bool) {#getdisplaystyle_2}

Ermittelt den Anzeigestil dieser Zelle.

```csharp
public Style GetDisplayStyle(bool includeMergedBorders)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| includeMergedBorders | Boolean | Gibt an, ob die Ränder zusammengeführter Zellen geprüft werden. |

### Rückgabewert

Anzeigestil dieser Zelle

### Hinweise

Wenn das angegebene Flag false ist, entspricht es `GetDisplayStyle`. Andernfalls entspricht es der Verwendung von SideBorders&#x7C;DynamicStyleBorders für `GetDisplayStyle`.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetDisplayStyleWithBooleanDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Greifen Sie auf die Zelle B2 zu und setzen Sie einige Stileigenschaften.
            Cell cell = worksheet.Cells["B2"];
            Style cellStyle = cell.GetStyle();
            cellStyle.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;
            cell.SetStyle(cellStyle);
            
            // Ermitteln Sie den Anzeigestil mit Formatierung (true-Parameter).
            Style displayStyle = cell.GetDisplayStyle(true);
            
            // Geben Sie den Stil der rechten Rahmenlinie aus.
            Console.WriteLine("Right Border Line Style: " + displayStyle.Borders[BorderType.RightBorder].LineStyle);
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

## GetDisplayStyle(BorderType) {#getdisplaystyle_1}

Ermittelt den Anzeigestil dieser Zelle.

```csharp
public Style GetDisplayStyle(BorderType adjacentBorders)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| adjacentBorders | BorderType | Gibt an, welche Rahmen überprüft und gemäß den Rahmen benachbarter Zellen angepasst werden müssen. |

### Rückgabewert

Anzeigestil dieser Zelle

### Hinweise

Wenn diese Zelle auch von anderen Einstellungen wie bedingter Formatierung, Listobjekten usw. betroffen ist, kann der Anzeigestil von [`GetStyle`](../getstyle/) abweichen. Für Flags zum Anpassen von Rahmen gemäß benachbarten Zellen bedeuten TopBorder/BottomBorder /LeftBorder/RightBorder, ob die unteren/oberen/rechten/linken Rahmen der links/rechts/oben/unten benachbarten Zellen überprüft und kombiniert werden sollen. Aus Leistungs- und Kompatibilitätsgründen werden einige Enums verwendet, um spezielle Vorgänge zu kennzeichnen: Horizontal/Vertical geben an, ob der untere/rechte Rahmen zusammengeführter Zellen mit diesem kombiniert werden soll. Diagonal (das heißt, sowohl DiagonalUpBorder als auch DiagonalDownBorder wurden gesetzt) bedeutet, dass Rahmen aus dem Anzeigestil benachbarter Zellen überprüft und kombiniert werden. Bitte beachten Sie, dass das Prüfen von Rahmen/Styles benachbarter Zellen, insbesondere der Anzeigestile, ein zeitaufwändiger Vorgang ist. Wenn die Rahmen für den zurückgegebenen Stil nicht benötigt werden, führt die Verwendung von None zum Deaktivieren des Prozesses für benachbarte Zellen zu besserer Leistung. Beim Abrufen von Rahmen benachbarter Zellen aus ausschließlich auf diesen Zellen definierten Styles (ohne Diagonal zu setzen) kann die Leistung ebenfalls besser sein, da das Prüfen des Anzeigestils einer Zelle ebenfalls zeitintensiv ist.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetDisplayStyleWithBorderTypeDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;

            // Beispieldaten festlegen
            for (int i = 0; i < 10; i++)
            {
                cells[i, 0].PutValue(i);
            }

            // Bedingte Formatierung erstellen
            FormatConditionCollection fcs = sheet.ConditionalFormattings[sheet.ConditionalFormattings.Add()];
            fcs.AddArea(CellArea.CreateCellArea(0, 0, 9, 0));
            fcs.AddCondition(FormatConditionType.ColorScale);

            // Ermitteln Sie den Anzeigestil mit unterschiedlichen Rahmentypen.
            for (int i = 0; i < 10; i++)
            {
                Style styleWithBorder = cells[i, 0].GetDisplayStyle(BorderType.TopBorder);
                Style styleWithoutBorder = cells[i, 0].GetDisplayStyle(BorderType.None);

                Console.WriteLine($"Cell {i + 1}:");
                Console.WriteLine($"  Style with border - Foreground: {styleWithBorder.ForegroundArgbColor:X}");
                Console.WriteLine($"  Style without border - Foreground: {styleWithoutBorder.ForegroundArgbColor:X}");
            }
        }
    }
}
```

### Siehe auch

* class [Style](../../style/)
* enum [BorderType](../../bordertype/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


