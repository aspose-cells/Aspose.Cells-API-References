---
title: "Klasse Style"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Style Klasse. Stellt den Anzeigestil von Excel-Dokumenten dar, wie Schriftfarbe, Ausrichtung, Rahmen usw. Das Style-Objekt enthält alle Stilattribute wie Schrift, Zahlenformat, Ausrichtung und dergleichen als Eigenschaften."
type: docs
url: /de/net/aspose.cells/style/
---
## Style class

Stellt den Anzeigestil eines Excel-Dokuments dar, wie Schriftart, Farbe, Ausrichtung, Rahmen usw. Das Style-Objekt enthält alle Stilattribute (Schriftart, Zahlenformat, Ausrichtung usw.) als Eigenschaften.

```csharp
public class Style
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [Style](style/)() | (**Obsolete.**) Initialisiert eine neue Instanz der `Style` Klasse. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [BackgroundArgbColor](../../aspose.cells/style/backgroundargbcolor/) { get; set; } | Liest und setzt die Hintergrundfarbe mit einem 32‑Bit‑ARGB‑Wert. |
| [BackgroundColor](../../aspose.cells/style/backgroundcolor/) { get; set; } | Liest oder setzt die Hintergrundfarbe eines Stils. |
| [BackgroundThemeColor](../../aspose.cells/style/backgroundthemecolor/) { get; set; } | Liest und setzt die Hintergrund‑Themenfarbe. |
| [Borders](../../aspose.cells/style/borders/) { get; } | Liest die [`BorderCollection`](../bordercollection/) des Stils. |
| [BottomBorder](../../aspose.cells/style/bottomborder/) { get; } | Liest den unteren Rand. |
| [CultureCustom](../../aspose.cells/style/culturecustom/) { get; set; } | Liest und setzt die kulturspezifische Musterzeichenfolge für das Zahlenformat. Wenn für dieses Objekt kein Zahlenformat festgelegt wurde, wird null zurückgegeben. Ist das Zahlenformat eingebaut, wird die dem eingebauten Zahlenformat entsprechende Musterzeichenfolge zurückgegeben. |
| [Custom](../../aspose.cells/style/custom/) { get; set; } | Stellt die benutzerdefinierte Zahlenformatzeichenfolge dieses Style‑Objekts dar. Wenn das benutzerdefinierte Zahlenformat nicht gesetzt ist (z. B. das Zahlenformat ist eingebaut), wird \"\" zurückgegeben. |
| [Font](../../aspose.cells/style/font/) { get; } | Liest ein [`Font`](./font/) Objekt. |
| [ForegroundArgbColor](../../aspose.cells/style/foregroundargbcolor/) { get; set; } | Liest und setzt die Vordergrundfarbe mit einem 32‑Bit‑ARGB‑Wert. |
| [ForegroundColor](../../aspose.cells/style/foregroundcolor/) { get; set; } | Liest oder setzt die Vordergrundfarbe eines Stils. |
| [ForegroundThemeColor](../../aspose.cells/style/foregroundthemecolor/) { get; set; } | Liest und setzt die Vordergrund‑Themenfarbe. |
| [HasBorders](../../aspose.cells/style/hasborders/) { get; } | Überprüft, ob für den Stil Rahmen festgelegt wurden. |
| [HorizontalAlignment](../../aspose.cells/style/horizontalalignment/) { get; set; } | Liest oder setzt den horizontalen Ausrichtungstyp des Textes in einer Zelle. |
| [IndentLevel](../../aspose.cells/style/indentlevel/) { get; set; } | Stellt die Einzugsebene für die Zelle oder den Bereich dar. Kann nur ein ganzzahliger Wert von 0 bis 250 sein. |
| [InvariantCustom](../../aspose.cells/style/invariantcustom/) { get; } | Liest die kulturlose Musterzeichenfolge für das Zahlenformat. Wenn für dieses Objekt kein Zahlenformat festgelegt wurde, wird null zurückgegeben. Ist das Zahlenformat eingebaut, wird die dem eingebauten Zahlenformat entsprechende Musterzeichenfolge zurückgegeben. |
| [IsAlignmentApplied](../../aspose.cells/style/isalignmentapplied/) { get; set; } | Gibt an, ob die Ausrichtungsformatierung angewendet werden soll. |
| [IsBorderApplied](../../aspose.cells/style/isborderapplied/) { get; set; } | Gibt an, ob die Rahmenformatierung angewendet werden soll. |
| [IsCheckBox](../../aspose.cells/style/ischeckbox/) { get; set; } | Gibt an, ob es sich um einen Stil einer Checkbox handelt |
| [IsDateTime](../../aspose.cells/style/isdatetime/) { get; } | Gibt an, ob das Zahlenformat ein Datumsformat ist. |
| [IsFillApplied](../../aspose.cells/style/isfillapplied/) { get; set; } | Gibt an, ob die Füllformatierung angewendet werden soll. |
| [IsFontApplied](../../aspose.cells/style/isfontapplied/) { get; set; } | Gibt an, ob die Schriftformatierung angewendet werden soll. |
| [IsFormulaHidden](../../aspose.cells/style/isformulahidden/) { get; set; } | Gibt an, ob die Formel verborgen wird, wenn das Arbeitsblatt geschützt ist. |
| [IsGradient](../../aspose.cells/style/isgradient/) { get; set; } | Gibt an, ob die Zellen Schattierung ein Farbverlaufsmuster ist. |
| [IsJustifyDistributed](../../aspose.cells/style/isjustifydistributed/) { get; set; } | Gibt an, ob die Zellen im Block- oder verteilten Ausrichtungsmodus in der letzten Textzeile verwendet werden sollen. |
| [IsLocked](../../aspose.cells/style/islocked/) { get; set; } | Liest oder setzt einen Wert, der angibt, ob eine Zelle bearbeitet werden kann oder nicht. |
| [IsNumberFormatApplied](../../aspose.cells/style/isnumberformatapplied/) { get; set; } | Gibt an, ob die Zahlenformatierung angewendet werden soll. |
| [IsPercent](../../aspose.cells/style/ispercent/) { get; } | Gibt an, ob das Zahlenformat ein Prozentformat ist. |
| [IsProtectionApplied](../../aspose.cells/style/isprotectionapplied/) { get; set; } | Gibt an, ob die Schutzformatierung angewendet werden soll. |
| [IsTextWrapped](../../aspose.cells/style/istextwrapped/) { get; set; } | Liest oder setzt einen Wert, der angibt, ob der Text innerhalb einer Zelle umgebrochen wird. |
| [LeftBorder](../../aspose.cells/style/leftborder/) { get; } | Liest den linken Rand. |
| [Name](../../aspose.cells/style/name/) { get; set; } | Liest oder setzt den Namen des Stils. |
| [Number](../../aspose.cells/style/number/) { get; set; } | Liest oder setzt das Anzeigeformat von Zahlen und Daten. Die Formatierungsmuster unterscheiden sich je nach Region. |
| [ParentStyle](../../aspose.cells/style/parentstyle/) { get; } | Liest den übergeordneten Stil dieses Stils. |
| [Pattern](../../aspose.cells/style/pattern/) { get; set; } | Liest oder setzt den Hintergrundmuster-Typ der Zelle. |
| [QuotePrefix](../../aspose.cells/style/quoteprefix/) { get; set; } | Gibt an, ob der Zellenwert mit einem einfachen Anführungszeichen beginnt. |
| [RightBorder](../../aspose.cells/style/rightborder/) { get; } | Liest den rechten Rand. |
| [RotationAngle](../../aspose.cells/style/rotationangle/) { get; set; } | Stellt den Textdrehwinkel dar. |
| [ShrinkToFit](../../aspose.cells/style/shrinktofit/) { get; set; } | Gibt an, ob der Text automatisch verkleinert wird, um in die verfügbare Spaltenbreite zu passen. |
| [TextDirection](../../aspose.cells/style/textdirection/) { get; set; } | Stellt die Lesereihenfolge des Textes dar. |
| [TopBorder](../../aspose.cells/style/topborder/) { get; } | Liest den oberen Rand. |
| [VerticalAlignment](../../aspose.cells/style/verticalalignment/) { get; set; } | Liest oder setzt den vertikalen Ausrichtungstyp des Textes in einer Zelle. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Copy](../../aspose.cells/style/copy/)(Style) | Kopiert Daten von einem anderen Stilobjekt |
| override [Equals](../../aspose.cells/style/equals/)(object) | Bestimmt, ob zwei Style-Instanzen gleich sind. |
| override [GetHashCode](../../aspose.cells/style/gethashcode/)() | Dient als Hash-Funktion für ein Style-Objekt. |
| [GetTwoColorGradient](../../aspose.cells/style/gettwocolorgradient/)(out Color, out Color, out GradientStyleType, out int) | (**Veraltet.**) Holen Sie die Einstellung für den Zweifarbverlauf. |
| [GetTwoColorGradientSetting](../../aspose.cells/style/gettwocolorgradientsetting/)() | Holen Sie die Einstellung für den Zweifarbverlauf. |
| [IsModified](../../aspose.cells/style/ismodified/)(StyleModifyFlag) | Überprüft, ob die angegebenen Eigenschaften des Stils geändert wurden. Wird für den Stil von ConditionalFormattings verwendet, um zu prüfen, ob die angegebenen Eigenschaften dieses Stils verwendet werden sollten, wenn ConditionalFormattings auf eine Zelle angewendet werden. |
| [SetBorder](../../aspose.cells/style/setborder/#setborder)(BorderType, CellBorderType, CellsColor) | Setzt die Ränder des Stils. |
| [SetBorder](../../aspose.cells/style/setborder/#setborder_1)(BorderType, CellBorderType, Color) | Setzt die Ränder des Stils. |
| [SetCustom](../../aspose.cells/style/setcustom/)(string, bool) | Setzt die Custom-Zahlenformatzeichenfolge einer Zelle. |
| [SetOutlineBorders](../../aspose.cells/style/setoutlineborders/#setoutlineborders)(CellBorderType, CellsColor) | Setze die Umrissränder |
| [SetOutlineBorders](../../aspose.cells/style/setoutlineborders/#setoutlineborders_1)(CellBorderType, Color) | Setze die Umrissränder |
| [SetPatternColor](../../aspose.cells/style/setpatterncolor/)(BackgroundType, Color, Color) | Setzt die Hintergrundfarbe. |
| [SetTwoColorGradient](../../aspose.cells/style/settwocolorgradient/)(Color, Color, GradientStyleType, int) | Setzt die angegebene Füllung auf einen Zweifarbverlauf. |
| [ToJson](../../aspose.cells/style/tojson/)() | Konvertiere `Style` zu JSON-Strukturdaten. |
| [Update](../../aspose.cells/style/update/)() | Wendet den benannten Stil auf die Stile der Zellen an, die diesen benannten Stil verwenden. Es funktioniert wie das Klicken auf die Schaltfläche \"ok\" nachdem Sie den Stil bearbeitet haben. Gilt nur für benannte Stile. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class StyleDemo
    {
        public static void StyleExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Greifen Sie auf eine Zelle aus dem Arbeitsblatt zu
            Cell cell = worksheet.Cells["A1"];
            
            // Ermitteln Sie den Stil der Zelle
            Style style = cell.GetStyle();
            
            // Setze verschiedene Eigenschaften des Stils
            style.Font.Name = "Times New Roman";
            style.Font.Color = Color.Blue;
            style.BackgroundColor = Color.Yellow;
            style.ForegroundColor = Color.Red;
            style.Pattern = BackgroundType.Solid;
            style.HorizontalAlignment = TextAlignmentType.Center;
            style.VerticalAlignment = TextAlignmentType.Center;
            style.IsTextWrapped = true;
            style.IsLocked = true;
            style.Number = 15; // Date format
            style.IndentLevel = 2;
            style.RotationAngle = 45;
            style.IsFormulaHidden = true;
            style.ShrinkToFit = true;
            style.TextDirection = TextDirectionType.RightToLeft;
            style.IsJustifyDistributed = true;
            style.QuotePrefix = true;
            style.IsGradient = true;
            style.IsNumberFormatApplied = true;
            style.IsFontApplied = true;
            style.IsAlignmentApplied = true;
            style.IsBorderApplied = true;
            style.IsFillApplied = true;
            style.IsProtectionApplied = true;
            style.BackgroundArgbColor = Color.Yellow.ToArgb();
            style.ForegroundArgbColor = Color.Red.ToArgb();
            style.Custom = "0.00%";
            style.CultureCustom = "0.00%";
            
            // Setze den Stil für die Zelle
            cell.SetStyle(style);
            
            // Speichere die Arbeitsmappe
            workbook.Save("StyleExample.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


