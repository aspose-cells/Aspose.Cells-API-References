---
title: Style
second_title: Aspose.Cells für .NET-API-Referenz
description: Repräsentiert den Anzeigestil eines Excel-Dokuments wie z. B. Schriftart Farbe Ausrichtung Rahmen usw. Das Style-Objekt enthält alle Stilattribute Schriftart Zahlenformat Ausrichtung usw. als Eigenschaften.
type: docs
weight: 5750
url: /de/net/aspose.cells/style/
---
## Style class

Repräsentiert den Anzeigestil eines Excel-Dokuments, wie z. B. Schriftart, Farbe, Ausrichtung, Rahmen usw. Das Style-Objekt enthält alle Stilattribute (Schriftart, Zahlenformat, Ausrichtung usw.) als Eigenschaften.

```csharp
public class Style
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [BackgroundArgbColor](../../aspose.cells/style/backgroundargbcolor) { get; set; } | Ruft die Hintergrundfarbe mit einem 32-Bit-ARGB-Wert ab und legt sie fest. |
| [BackgroundColor](../../aspose.cells/style/backgroundcolor) { get; set; } | Ruft die Hintergrundfarbe eines Stils ab oder legt sie fest. |
| [BackgroundThemeColor](../../aspose.cells/style/backgroundthemecolor) { get; set; } | Ruft die Farbe des Hintergrundthemas ab und legt sie fest. |
| [Borders](../../aspose.cells/style/borders) { get; } | Ruft die ab[`BorderCollection`](../bordercollection) des Stils. |
| [CultureCustom](../../aspose.cells/style/culturecustom) { get; set; } | Ruft die kulturabhängige Musterzeichenfolge für das Zahlenformat ab und legt sie fest. Wenn für dieses Objekt kein Zahlenformat festgelegt wurde, wird null zurückgegeben. Wenn das Zahlenformat eingebaut ist, wird die Musterzeichenfolge zurückgegeben, die der eingebauten Zahl entspricht. |
| [Custom](../../aspose.cells/style/custom) { get; set; } | Stellt die benutzerdefinierte Zahlenformatzeichenfolge dieses Stilobjekts dar. Wenn das benutzerdefinierte Zahlenformat nicht festgelegt ist (z. B. ist das Zahlenformat integriert), wird "" zurückgegeben. |
| [Font](../../aspose.cells/style/font) { get; } | erhält a[`Font`](./font) Objekt. |
| [ForegroundArgbColor](../../aspose.cells/style/foregroundargbcolor) { get; set; } | Ruft die Vordergrundfarbe mit einem 32-Bit-ARGB-Wert ab und legt sie fest. |
| [ForegroundColor](../../aspose.cells/style/foregroundcolor) { get; set; } | Ruft die Vordergrundfarbe eines Stils ab oder legt sie fest. |
| [ForegroundThemeColor](../../aspose.cells/style/foregroundthemecolor) { get; set; } | Ruft die Farbe des Vordergrunddesigns ab und legt sie fest. |
| [HasBorders](../../aspose.cells/style/hasborders) { get; } | Prüft, ob für den Stil Rahmen gesetzt wurden. |
| [HorizontalAlignment](../../aspose.cells/style/horizontalalignment) { get; set; } | Ruft den horizontalen Ausrichtungstyp des Textes in einer Zelle ab oder legt ihn fest. |
| [IndentLevel](../../aspose.cells/style/indentlevel) { get; set; } | Repräsentiert die Einzugsebene für die Zelle oder den Bereich. Kann nur eine Ganzzahl von 0 bis 250 sein. |
| [InvariantCustom](../../aspose.cells/style/invariantcustom) { get; } | Ruft die kulturunabhängige Musterzeichenfolge für das Zahlenformat ab. Wenn für dieses Objekt kein Zahlenformat festgelegt wurde, wird null zurückgegeben. Wenn das Zahlenformat eingebaut ist, wird die der eingebauten Zahl entsprechende Musterzeichenfolge zurückgegeben. |
| [IsDateTime](../../aspose.cells/style/isdatetime) { get; } | Gibt an, ob das Zahlenformat ein Datumsformat ist. |
| [IsFormulaHidden](../../aspose.cells/style/isformulahidden) { get; set; } | Stellt dar, ob die Formel ausgeblendet wird, wenn das Arbeitsblatt geschützt ist. |
| [IsGradient](../../aspose.cells/style/isgradient) { get; set; } | Gibt an, ob die Zellschattierung ein Verlaufsmuster ist. |
| [IsJustifyDistributed](../../aspose.cells/style/isjustifydistributed) { get; set; } | Gibt an, ob die Zellen im Blocksatz oder in der verteilten Ausrichtung in der letzten Textzeile verwendet werden sollen. |
| [IsLocked](../../aspose.cells/style/islocked) { get; set; } | Ruft einen Wert ab oder legt einen Wert fest, der angibt, ob eine Zelle geändert werden kann oder nicht. |
| [IsPercent](../../aspose.cells/style/ispercent) { get; } | Gibt an, ob das Zahlenformat ein Prozentformat ist. |
| [IsTextWrapped](../../aspose.cells/style/istextwrapped) { get; set; } | Ruft einen Wert ab oder legt einen Wert fest, der angibt, ob der Text in einer Zelle umgebrochen ist. |
| [Name](../../aspose.cells/style/name) { get; set; } | Ruft den Namen des Stils ab oder legt ihn fest. |
| [Number](../../aspose.cells/style/number) { get; set; } | Ruft das Anzeigeformat von Zahlen und Daten ab oder legt es fest. Die Formatierungsmuster sind für verschiedene Regionen unterschiedlich. |
| [ParentStyle](../../aspose.cells/style/parentstyle) { get; } | Ruft den übergeordneten Stil dieses Stils ab. |
| [Pattern](../../aspose.cells/style/pattern) { get; set; } | Ruft den Typ des Zellenhintergrundmusters ab oder legt ihn fest. |
| [QuotePrefix](../../aspose.cells/style/quoteprefix) { get; set; } | Gibt an, ob der Wert der Zelle mit einem einfachen Anführungszeichen beginnt. |
| [RotationAngle](../../aspose.cells/style/rotationangle) { get; set; } | Stellt den Drehwinkel des Textes dar. |
| [ShrinkToFit](../../aspose.cells/style/shrinktofit) { get; set; } | Stellt dar, ob Text automatisch verkleinert wird, um in die verfügbare Spaltenbreite zu passen. |
| [TextDirection](../../aspose.cells/style/textdirection) { get; set; } | Stellt die Lesereihenfolge des Textes dar. |
| [VerticalAlignment](../../aspose.cells/style/verticalalignment) { get; set; } | Ruft den vertikalen Ausrichtungstyp des Textes in einer Zelle ab oder legt ihn fest. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Copy](../../aspose.cells/style/copy)(Style) | Kopiert Daten von einem anderen Stilobjekt |
| override [Equals](../../aspose.cells/style/equals)(object) | Bestimmt, ob zwei Style-Instanzen gleich sind. |
| override [GetHashCode](../../aspose.cells/style/gethashcode)() | Dient als Hash-Funktion für ein Style-Objekt. |
| [GetTwoColorGradient](../../aspose.cells/style/gettwocolorgradient)(out Color, out Color, out GradientStyleType, out int) | Holen Sie sich die zweifarbige Verlaufseinstellung. |
| [IsModified](../../aspose.cells/style/ismodified)(StyleModifyFlag) | Überprüft, ob die angegebenen Eigenschaften des Stils geändert wurden. Wird für den Stil von ConditionalFormattings verwendet, um zu prüfen, ob die angegebenen Eigenschaften dieses Stils verwendet werden sollen, wenn die ConditionalFormattings auf eine Zelle angewendet werden. |
| [SetBorder](../../aspose.cells/style/setborder)(BorderType, CellBorderType, Color) | Legt die Grenzen des Stils fest. |
| [SetCustom](../../aspose.cells/style/setcustom)(string, bool) | Legt die Zeichenfolge für das benutzerdefinierte Zahlenformat einer Zelle fest. |
| [SetPatternColor](../../aspose.cells/style/setpatterncolor)(BackgroundType, Color, Color) | Legt die Hintergrundfarbe fest. |
| [SetTwoColorGradient](../../aspose.cells/style/settwocolorgradient)(Color, Color, GradientStyleType, int) | Legt die angegebene Füllung auf einen zweifarbigen Farbverlauf fest. |
| [Update](../../aspose.cells/style/update)() | Wenden Sie den benannten Stil auf die Stile der Zellen an, die diesen benannten Stil verwenden. Es funktioniert so, als ob Sie auf die Schaltfläche „OK“ klicken, nachdem Sie die Änderung des Stils abgeschlossen haben. Gilt nur für den benannten Stil. |

### Beispiele

```csharp
[C#]
Workbook workbook = new Workbook();

WorksheetCollection sheets = workbook.Worksheets;
Cell cell = sheets[0].Cells["A1"];
Style style =  cell.GetStyle();
style.Font.Name = "Times New Roman";
style.Font.Color = Color.Blue;
cell.SetStyle(style);
```

### Siehe auch

* namensraum [Aspose.Cells](../../aspose.cells)
* Montage [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
