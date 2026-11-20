---
title: "Stil"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt den Anzeigestil von Excel-Dokumenten dar, z. B. Schriftfarbe, Ausrichtung, Rahmen usw."
type: docs
url: /de/java/com.aspose.cells/style/
---

**Inheritance:**
java.lang.Object
```
public class Style
```

Stellt den Anzeigestil von Excel-Dokumenten dar, z. B. Schrift, Farbe, Ausrichtung, Rahmen usw. Das Style‑Objekt enthält alle Stilattribute (Schrift, Zahlenformat, Ausrichtung usw.) als Eigenschaften.

**Example**

```
         Workbook workbook = new Workbook();
 
         WorksheetCollection sheets = workbook.getWorksheets();
         Cell cell = sheets.get(0).getCells().get("A1");
         Style style =  cell.getStyle();
         style.getFont().setName("Times New Roman");
         style.getFont().setColor(Color.getBlue());
         cell.setStyle(style);
```
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [Style()](#Style--) | Initialisiert eine neue Instanz der [Style](../../com.aspose.cells/style)-Klasse. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [copy(Style style)](#copy-com.aspose.cells.Style-) | Kopiert Daten aus einem anderen Stilobjekt |
| [equals(Object obj)](#equals-java.lang.Object-) | Bestimmt, ob zwei Style‑Instanzen gleich sind. |
| [getBackgroundArgbColor()](#getBackgroundArgbColor--) | Liest die Hintergrundfarbe mit einem 32‑Bit‑ARGB‑Wert. |
| [getBackgroundColor()](#getBackgroundColor--) | Liest die Hintergrundfarbe eines Stils. |
| [getBackgroundThemeColor()](#getBackgroundThemeColor--) | Liest die Hintergrund‑Designfarbe. |
| [getBorders()](#getBorders--) | Liest die [BorderCollection](../../com.aspose.cells/bordercollection) des Stils. |
| [getBottomBorder()](#getBottomBorder--) | Liest den unteren Rand. |
| [getClass()](#getClass--) |  |
| [getCultureCustom()](#getCultureCustom--) | Liest die kulturspezifische Musterzeichenfolge für das Zahlenformat. |
| [getCustom()](#getCustom--) | Stellt die benutzerdefinierte Zahlenformatzeichenfolge dieses Stilobjekts dar. |
| [getFont()](#getFont--) | Liest ein [getFont()](../../com.aspose.cells/style\#getFont--)‑Objekt. |
| [getForegroundArgbColor()](#getForegroundArgbColor--) | Liest die Vordergrundfarbe mit einem 32‑Bit‑ARGB‑Wert. |
| [getForegroundColor()](#getForegroundColor--) | Liest die Vordergrundfarbe eines Stils. |
| [getForegroundThemeColor()](#getForegroundThemeColor--) | Liest die Vordergrund‑Designfarbe. |
| [getHorizontalAlignment()](#getHorizontalAlignment--) | Liest den horizontalen Ausrichtungstyp des Textes in einer Zelle. |
| [getIndentLevel()](#getIndentLevel--) | Stellt die Einzugsebene für die Zelle oder den Bereich dar. |
| [getInvariantCustom()](#getInvariantCustom--) | Liest die kulturlose Musterzeichenfolge für das Zahlenformat. |
| [getLeftBorder()](#getLeftBorder--) | Liest den linken Rand. |
| [getName()](#getName--) | Ruft den Namen des Stils ab. |
| [getNumber()](#getNumber--) | Ruft das Anzeigeformat von Zahlen und Datumsangaben ab. |
| [getParentStyle()](#getParentStyle--) | Ruft den übergeordneten Stil dieses Stils ab. |
| [getPattern()](#getPattern--) | Ruft den Hintergrundmuster‑Typ der Zelle ab. |
| [getQuotePrefix()](#getQuotePrefix--) | Gibt an, ob der Zellenwert mit einem einfachen Anführungszeichen beginnt. |
| [getRightBorder()](#getRightBorder--) | Ruft den rechten Rand ab. |
| [getRotationAngle()](#getRotationAngle--) | Stellt den Textdrehwinkel dar. |
| [getShrinkToFit()](#getShrinkToFit--) | Stellt dar, ob der Text automatisch verkleinert wird, um in die verfügbare Spaltenbreite zu passen. |
| [getTextDirection()](#getTextDirection--) | Stellt die Lesereihenfolge des Textes dar. |
| [getTopBorder()](#getTopBorder--) | Ruft den oberen Rand ab. |
| [getTwoColorGradient()](#getTwoColorGradient--) | Ruft die Einstellung für den Zweifarbverlauf ab. |
| [getTwoColorGradientSetting()](#getTwoColorGradientSetting--) | Ruft die Einstellung für den Zweifarbverlauf ab. |
| [getVerticalAlignment()](#getVerticalAlignment--) | Ruft den vertikalen Ausrichtungstyp des Textes in einer Zelle ab. |
| [hasBorders()](#hasBorders--) | Überprüft, ob für den Stil Rahmen festgelegt wurden. |
| [hashCode()](#hashCode--) | Dient als Hashfunktion für ein Style-Objekt. |
| [isAlignmentApplied()](#isAlignmentApplied--) | Gibt an, ob die Ausrichtungsformatierung angewendet werden soll. |
| [isBorderApplied()](#isBorderApplied--) | Gibt an, ob die Rahmenformatierung angewendet werden soll. |
| [isCheckBox()](#isCheckBox--) | Gibt an, ob es sich um einen Stil für ein Kontrollkästchen handelt |
| [isDateTime()](#isDateTime--) | Gibt an, ob das Zahlenformat ein Datumsformat ist. |
| [isFillApplied()](#isFillApplied--) | Gibt an, ob die Füllformatierung angewendet werden soll. |
| [isFontApplied()](#isFontApplied--) | Gibt an, ob die Schriftformatierung angewendet werden soll. |
| [isFormulaHidden()](#isFormulaHidden--) | Stellt dar, ob die Formel verborgen wird, wenn das Arbeitsblatt geschützt ist. |
| [isGradient()](#isGradient--) | Gibt an, ob die Zellenhintergrundschattierung ein Verlaufsmuster ist. |
| [isJustifyDistributed()](#isJustifyDistributed--) | Gibt an, ob für die letzte Textzeile die Block‑ oder Verteilt‑Ausrichtung verwendet werden soll. |
| [isLocked()](#isLocked--) | Ruft einen Wert ab, der angibt, ob eine Zelle bearbeitet werden kann oder nicht. |
| [isModified(int modifyFlag)](#isModified-int-) | Überprüft, ob die angegebenen Eigenschaften des Stils geändert wurden. |
| [isNumberFormatApplied()](#isNumberFormatApplied--) | Gibt an, ob die Zahlenformatierung angewendet werden soll. |
| [isPercent()](#isPercent--) | Gibt an, ob das Zahlenformat ein Prozentformat ist. |
| [isProtectionApplied()](#isProtectionApplied--) | Gibt an, ob die Schutzformatierung angewendet werden soll. |
| [isTextWrapped()](#isTextWrapped--) | Ermittelt einen Wert, der angibt, ob der Text innerhalb einer Zelle umgebrochen ist. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAlignmentApplied(boolean value)](#setAlignmentApplied-boolean-) | Gibt an, ob die Ausrichtungsformatierung angewendet werden soll. |
| [setBackgroundArgbColor(int value)](#setBackgroundArgbColor-int-) | Legt die Hintergrundfarbe mit einem 32‑Bit‑ARGB‑Wert fest. |
| [setBackgroundColor(Color value)](#setBackgroundColor-com.aspose.cells.Color-) | Legt die Hintergrundfarbe eines Stils fest. |
| [setBackgroundThemeColor(ThemeColor value)](#setBackgroundThemeColor-com.aspose.cells.ThemeColor-) | Legt die Hintergrund‑Designfarbe fest. |
| [setBorder(int borderType, int borderStyle, CellsColor borderColor)](#setBorder-int-int-com.aspose.cells.CellsColor-) | Legt die Rahmen des Stils fest. |
| [setBorder(int borderType, int borderStyle, Color borderColor)](#setBorder-int-int-com.aspose.cells.Color-) | Legt die Rahmen des Stils fest. |
| [setBorderApplied(boolean value)](#setBorderApplied-boolean-) | Gibt an, ob die Rahmenformatierung angewendet werden soll. |
| [setCheckBox(boolean value)](#setCheckBox-boolean-) | Gibt an, ob es sich um einen Stil für ein Kontrollkästchen handelt |
| [setCultureCustom(String value)](#setCultureCustom-java.lang.String-) | Legt die kulturspezifische Musterzeichenfolge für das Zahlenformat fest. |
| [setCustom(String value)](#setCustom-java.lang.String-) | Stellt die benutzerdefinierte Zahlenformatzeichenfolge dieses Stilobjekts dar. |
| [setCustom(String custom, boolean builtinPreference)](#setCustom-java.lang.String-boolean-) | Legt die benutzerdefinierte Zahlenformatzeichenfolge einer Zelle fest. |
| [setFillApplied(boolean value)](#setFillApplied-boolean-) | Gibt an, ob die Füllformatierung angewendet werden soll. |
| [setFontApplied(boolean value)](#setFontApplied-boolean-) | Gibt an, ob die Schriftformatierung angewendet werden soll. |
| [setForegroundArgbColor(int value)](#setForegroundArgbColor-int-) | Legt die Vordergrundfarbe mit einem 32‑Bit‑ARGB‑Wert fest. |
| [setForegroundColor(Color value)](#setForegroundColor-com.aspose.cells.Color-) | Legt die Vordergrundfarbe eines Stils fest. |
| [setForegroundThemeColor(ThemeColor value)](#setForegroundThemeColor-com.aspose.cells.ThemeColor-) | Legt die Vordergrund‑Designfarbe fest. |
| [setFormulaHidden(boolean value)](#setFormulaHidden-boolean-) | Stellt dar, ob die Formel verborgen wird, wenn das Arbeitsblatt geschützt ist. |
| [setGradient(boolean value)](#setGradient-boolean-) | Gibt an, ob die Zellenhintergrundschattierung ein Verlaufsmuster ist. |
| [setHorizontalAlignment(int value)](#setHorizontalAlignment-int-) | Legt den horizontalen Ausrichtungstyp des Textes in einer Zelle fest. |
| [setIndentLevel(int value)](#setIndentLevel-int-) | Stellt die Einzugsebene für die Zelle oder den Bereich dar. |
| [setJustifyDistributed(boolean value)](#setJustifyDistributed-boolean-) | Gibt an, ob für die letzte Textzeile die Block‑ oder Verteilt‑Ausrichtung verwendet werden soll. |
| [setLocked(boolean value)](#setLocked-boolean-) | Legt einen Wert fest, der angibt, ob eine Zelle bearbeitet werden kann oder nicht. |
| [setName(String value)](#setName-java.lang.String-) | Legt den Namen des Stils fest. |
| [setNumber(int value)](#setNumber-int-) | Legt das Anzeigeformat von Zahlen und Datumsangaben fest. |
| [setNumberFormatApplied(boolean value)](#setNumberFormatApplied-boolean-) | Gibt an, ob die Zahlenformatierung angewendet werden soll. |
| [setOutlineBorders(int borderStyle, CellsColor borderColor)](#setOutlineBorders-int-com.aspose.cells.CellsColor-) | Lege die Umrissrahmen fest |
| [setOutlineBorders(int borderStyle, Color borderColor)](#setOutlineBorders-int-com.aspose.cells.Color-) | Lege die Umrissrahmen fest |
| [setPattern(int value)](#setPattern-int-) | Legt den Hintergrundmustertyp der Zelle fest. |
| [setPatternColor(int pattern, Color color1, Color color2)](#setPatternColor-int-com.aspose.cells.Color-com.aspose.cells.Color-) | Legt die Hintergrundfarbe fest. |
| [setProtectionApplied(boolean value)](#setProtectionApplied-boolean-) | Gibt an, ob die Schutzformatierung angewendet werden soll. |
| [setQuotePrefix(boolean value)](#setQuotePrefix-boolean-) | Gibt an, ob der Zellenwert mit einem einfachen Anführungszeichen beginnt. |
| [setRotationAngle(int value)](#setRotationAngle-int-) | Stellt den Textdrehwinkel dar. |
| [setShrinkToFit(boolean value)](#setShrinkToFit-boolean-) | Stellt dar, ob der Text automatisch verkleinert wird, um in die verfügbare Spaltenbreite zu passen. |
| [setTextDirection(int value)](#setTextDirection-int-) | Stellt die Lesereihenfolge des Textes dar. |
| [setTextWrapped(boolean value)](#setTextWrapped-boolean-) | Legt einen Wert fest, der angibt, ob der Text innerhalb einer Zelle umgebrochen ist. |
| [setTwoColorGradient(Color color1, Color color2, int gradientStyleType, int variant)](#setTwoColorGradient-com.aspose.cells.Color-com.aspose.cells.Color-int-int-) | Setzt die angegebene Füllung auf einen Zweifarbverlauf. |
| [setVerticalAlignment(int value)](#setVerticalAlignment-int-) | Legt den vertikalen Ausrichtungstyp des Textes in einer Zelle fest. |
| [toJson()](#toJson--) | Konvertiere [Style](../../com.aspose.cells/style) in JSON‑Strukturdaten. |
| [toString()](#toString--) |  |
| [update()](#update--) | Wende den benannten Stil auf die Stile der Zellen an, die diesen benannten Stil verwenden. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### Style() {#Style--}
```
public Style()
```


Initialisiert eine neue Instanz der [Style](../../com.aspose.cells/style)-Klasse.

**Remarks**

HINWEIS: Dieser Konstruktor ist jetzt veraltet. Verwenden Sie stattdessen die Methode CellsFactory.CreateStyle(). Diese Eigenschaft wird 6 Monate später seit Oktober 2016 entfernt werden. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

### copy(Style style) {#copy-com.aspose.cells.Style-}
```
public void copy(Style style)
```


Kopiert Daten aus einem anderen Stilobjekt

**Remarks**

Diese Methode kopiert den Namen des Stils nicht. Wenn Sie den Namen kopieren möchten, rufen Sie bitte nach dem Kopieren des Stils den folgenden Code auf: destStyle.Name = style.Name.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | Quell-Style-Objekt |

### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Bestimmt, ob zwei Style‑Instanzen gleich sind.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| obj | java.lang.Object | Das Style-Objekt zum Vergleich mit dem aktuellen Style-Objekt. |

**Returns:**
boolean – true, wenn das angegebene Objekt dem aktuellen Objekt entspricht; andernfalls false.
### getBackgroundArgbColor() {#getBackgroundArgbColor--}
```
public int getBackgroundArgbColor()
```


Liest die Hintergrundfarbe mit einem 32‑Bit‑ARGB‑Wert.

**Returns:**
int
### getBackgroundColor() {#getBackgroundColor--}
```
public Color getBackgroundColor()
```


Liest die Hintergrundfarbe eines Stils.

**Remarks**

Wenn Sie die Farbe einer Zelle festlegen möchten, verwenden Sie bitte die Eigenschaft Style.ForegroundColor. Nur wenn das Zellen-Style-Muster nicht „none“ oder „solid“ ist, wirkt sich diese Eigenschaft aus.

**Returns:**
[Color](../../com.aspose.cells/color)
### getBackgroundThemeColor() {#getBackgroundThemeColor--}
```
public ThemeColor getBackgroundThemeColor()
```


Liest die Hintergrund‑Designfarbe.

**Remarks**

Wenn die Hintergrundfarbe keine Designfarbe ist, wird NULL zurückgegeben.

**Returns:**
[ThemeColor](../../com.aspose.cells/themecolor)
### getBorders() {#getBorders--}
```
public BorderCollection getBorders()
```


Liest die [BorderCollection](../../com.aspose.cells/bordercollection) des Stils.

**Returns:**
[BorderCollection](../../com.aspose.cells/bordercollection)
### getBottomBorder() {#getBottomBorder--}
```
public Border getBottomBorder()
```


Liest den unteren Rand.

**Returns:**
[Border](../../com.aspose.cells/border)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCultureCustom() {#getCultureCustom--}
```
public String getCultureCustom()
```


Gibt die kulturspezifische Musterzeichenfolge für das Zahlenformat zurück. Wenn für dieses Objekt kein Zahlenformat festgelegt wurde, wird null zurückgegeben. Ist das Zahlenformat eingebaut, wird die dem eingebauten Zahlenformat entsprechende Musterzeichenfolge zurückgegeben.

**Remarks**

Für eingebautes Zahlenformat sind sowohl der Musterinhalt (z. B. ein eingebautes Datumsformat ist \"m/d/y\" für einige Gebietsschemas, für andere wird es zu \"d/m/y\") als auch der Formatbezeichner (z. B. verwenden einige Gebietsschemas ein anderes Zeichen als 'y' für den Jahresanteil bei der Datumsformatierung) kulturbabhängig; Für vom Benutzer angegebenes benutzerdefiniertes Format werden nur die Formatbezeichner gemäß der Kultur geändert, andere Teile des Formatmusters bleiben unverändert.

**Returns:**
java.lang.String
### getCustom() {#getCustom--}
```
public String getCustom()
```


Stellt die benutzerdefinierte Zahlenformatzeichenfolge dieses Style-Objekts dar. Wenn das benutzerdefinierte Zahlenformat nicht festgelegt ist (z. B. das Zahlenformat ist eingebaut), wird \"\" zurückgegeben.

**Remarks**

Die zurückgegebene benutzerdefinierte Zeichenfolge ist kulturlos.

**Returns:**
java.lang.String
### getFont() {#getFont--}
```
public Font getFont()
```


Liest ein [getFont()](../../com.aspose.cells/style\#getFont--)‑Objekt.

**Returns:**
[Font](../../com.aspose.cells/font)
### getForegroundArgbColor() {#getForegroundArgbColor--}
```
public int getForegroundArgbColor()
```


Liest die Vordergrundfarbe mit einem 32‑Bit‑ARGB‑Wert.

**Returns:**
int
### getForegroundColor() {#getForegroundColor--}
```
public Color getForegroundColor()
```


Liest die Vordergrundfarbe eines Stils.

**Remarks**

Das bedeutet, dass keine Farbe eingestellt ist, wenn Color.Empty zurückgegeben wird.

**Returns:**
[Color](../../com.aspose.cells/color)
### getForegroundThemeColor() {#getForegroundThemeColor--}
```
public ThemeColor getForegroundThemeColor()
```


Liest die Vordergrund‑Designfarbe.

**Remarks**

Wenn die Vordergrundfarbe keine Designfarbe ist, wird NULL zurückgegeben.

**Returns:**
[ThemeColor](../../com.aspose.cells/themecolor)
### getHorizontalAlignment() {#getHorizontalAlignment--}
```
public int getHorizontalAlignment()
```


Liest den horizontalen Ausrichtungstyp des Textes in einer Zelle.

Siehe [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Returns:**
int
### getIndentLevel() {#getIndentLevel--}
```
public int getIndentLevel()
```


Stellt die Einzugsebene für die Zelle oder den Bereich dar. Kann nur ein ganzzahliger Wert von 0 bis 250 sein.

**Remarks**

Wenn die horizontale Ausrichtung des Textes auf einen anderen Wert als links oder rechts gesetzt wird, wird die Einzugsebene auf Null zurückgesetzt.

**Returns:**
int
### getInvariantCustom() {#getInvariantCustom--}
```
public String getInvariantCustom()
```


Gibt die kulturunabhängige Musterzeichenfolge für das Zahlenformat zurück. Wenn für dieses Objekt kein Zahlenformat festgelegt wurde, wird null zurückgegeben. Ist das Zahlenformat eingebaut, wird die dem eingebauten Zahlenformat entsprechende Musterzeichenfolge zurückgegeben.

**Remarks**

Für eingebaute Zahlenformate ist der zurückgegebene Musterinhalt weiterhin kulturbabhängig, z. B. gibt er für einige Gebietsschemas \"m/d/y\" und für andere \"d/m/y\" zurück. Der Unterschied zu [getCultureCustom()](../../com.aspose.cells/style\\#getCultureCustom--) besteht darin (das ist ebenfalls das, was kulturunabhängig bedeutet): Die Formatbezeichner und Trennzeichen bleiben standardisiert, z. B. wird '/' immer als Datums‑Trennzeichen verwendet und \"y\" immer als Jahres‑Teil, unabhängig davon, welches Sonderzeichen für das jeweilige Gebietsschema verwendet wird.

**Returns:**
java.lang.String
### getLeftBorder() {#getLeftBorder--}
```
public Border getLeftBorder()
```


Liest den linken Rand.

**Returns:**
[Border](../../com.aspose.cells/border)
### getName() {#getName--}
```
public String getName()
```


Ruft den Namen des Stils ab.

**Returns:**
java.lang.String
### getNumber() {#getNumber--}
```
public int getNumber()
```


Gibt das Anzeigeformat von Zahlen und Datumsangaben zurück. Die Formatierungsmuster unterscheiden sich je nach Region.

**Remarks**

Beispielweise werden die Formatierungsmuster für die Region en\\_US durch Zahlen dargestellt:

| Value | Typ | Formatzeichenfolge |
| ----- | ---------- | ---------------------------------------------------- |
| 0 | General | `General` |
| 1 | Decimal | `0` |
| 2 | Decimal | `0.00` |
| 3 | Decimal | `#,##0` |
| 4 | Decimal | `#,##0.00` |
| 5 | Currency | `$#,##0_);($#,##0)` |
| 6 | Currency | `$#,##0_);[Red](../$#,##0)` |
| 7 | Currency | `$#,##0.00_);($#,##0.00)` |
| 8 | Currency | `$#,##0.00_);[Rot](../$#,##0.00)` |
| 9 | Percentage | `0%` |
| 10 | Percentage | `0.00%` |
| 11 | Scientific | `0.00E+00` |
| 12 | Fraction | `# ?/?` |
| 13 | Fraction | `# ??/??` |
| 14 | Date | `m/d/yyyy` |
| 15 | Date | `d-mmm-yy` |
| 16 | Date | `d-mmm` |
| 17 | Date | `mmm-yy` |
| 18 | Time | `h:mm AM/PM` |
| 19 | Time | `h:mm:ss AM/PM` |
| 20 | Time | `h:mm` |
| 21 | Time | `h:mm:ss` |
| 22 | Time | `m/d/yyyy h:mm` |
| 37 | Accounting | `#,##0_);(#,##0)` |
| 38 | Accounting | `#,##0_);[Rot](../#,##0)` |
| 39 | Accounting | `#,##0.00_);(#,##0.00)` |
| 40 | Accounting | `#,##0.00_);[Rot](../#,##0.00)` |
| 41 | Accounting | `_(* #,##0_);_(* (#,##0);_(* "-"_);_(@_)` |
| 42 | Currency | `_($* #,##0_);_($* (#,##0);_($* "-"_);_(@_)` |
| 43 | Accounting | `_(* #,##0.00_);_(* (#,##0.00);_(* "-"??_);_(@_)` |
| 44 | Currency | `_($* #,##0.00_);_($* (#,##0.00);_($* "-"??_);_(@_)` |
| 45 | Time | `mm:ss` |
| 46 | Time | `[h]:mm:ss` |
| 47 | Time | `mm:ss.0` |
| 48 | Scientific | `##0.0E+0` |
| 49 | Text | `@` |

**Returns:**
int
### getParentStyle() {#getParentStyle--}
```
public Style getParentStyle()
```


Ruft den übergeordneten Stil dieses Stils ab.

**Returns:**
[Style](../../com.aspose.cells/style)
### getPattern() {#getPattern--}
```
public int getPattern()
```


Ruft den Hintergrundmuster‑Typ der Zelle ab.

Siehe [BackgroundType](../../com.aspose.cells/backgroundtype).

**Returns:**
int
### getQuotePrefix() {#getQuotePrefix--}
```
public boolean getQuotePrefix()
```


Gibt an, ob der Zellenwert mit einem einfachen Anführungszeichen beginnt.

**Returns:**
boolean
### getRightBorder() {#getRightBorder--}
```
public Border getRightBorder()
```


Ruft den rechten Rand ab.

**Returns:**
[Border](../../com.aspose.cells/border)
### getRotationAngle() {#getRotationAngle--}
```
public int getRotationAngle()
```


Stellt den Textdrehwinkel dar.

**Remarks**

0: Nicht gedreht.

255: Oben nach unten.

\-90: Abwärts.

90: Aufwärts.

Sie können 255 oder einen Wert im Bereich von -90 bis 90 setzen.

**Returns:**
int
### getShrinkToFit() {#getShrinkToFit--}
```
public boolean getShrinkToFit()
```


Stellt dar, ob der Text automatisch verkleinert wird, um in die verfügbare Spaltenbreite zu passen.

**Returns:**
boolean
### getTextDirection() {#getTextDirection--}
```
public int getTextDirection()
```


Stellt die Lesereihenfolge des Textes dar.

Siehe [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Returns:**
int
### getTopBorder() {#getTopBorder--}
```
public Border getTopBorder()
```


Ruft den oberen Rand ab.

**Returns:**
[Border](../../com.aspose.cells/border)
### getTwoColorGradient() {#getTwoColorGradient--}
```
public Object[] getTwoColorGradient()
```


Ruft die Einstellung für den Zweifarbverlauf ab.

**Remarks**

HINWEIS: Diese Methode ist jetzt veraltet. Verwenden Sie stattdessen die Methode Style.GetTwoColorGradientSetting(). Diese Eigenschaft wird 12 Monate später, seit Dezember 2022, entfernt werden. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Returns:**
java.lang.Object[] - Gibt alle Einstellungen zum Zweifarbverlauf zurück [0] : Color1 [1] : Color2 [2] : GradientStyleType [3] : Variant
### getTwoColorGradientSetting() {#getTwoColorGradientSetting--}
```
public TwoColorGradient getTwoColorGradientSetting()
```


Ruft die Einstellung für den Zweifarbverlauf ab.

**Returns:**
[TwoColorGradient](../../com.aspose.cells/twocolorgradient)
### getVerticalAlignment() {#getVerticalAlignment--}
```
public int getVerticalAlignment()
```


Ruft den vertikalen Ausrichtungstyp des Textes in einer Zelle ab.

Siehe [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Returns:**
int
### hasBorders() {#hasBorders--}
```
public boolean hasBorders()
```


Überprüft, ob für den Stil Rahmen festgelegt wurden.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public int hashCode()
```


Dient als Hashfunktion für ein Style-Objekt.

**Remarks**

Diese Methode ist nur für den internen Gebrauch.

**Returns:**
int - Ein Hashcode für das aktuelle Objekt.
### isAlignmentApplied() {#isAlignmentApplied--}
```
public boolean isAlignmentApplied()
```


Gibt an, ob die Ausrichtungsformatierung angewendet werden soll.

**Remarks**

Nur für benannten Stil.

**Returns:**
boolean
### isBorderApplied() {#isBorderApplied--}
```
public boolean isBorderApplied()
```


Gibt an, ob die Rahmenformatierung angewendet werden soll.

**Remarks**

Nur für benannten Stil.

**Returns:**
boolean
### isCheckBox() {#isCheckBox--}
```
public boolean isCheckBox()
```


Gibt an, ob es sich um einen Stil für ein Kontrollkästchen handelt

**Returns:**
boolean
### isDateTime() {#isDateTime--}
```
public boolean isDateTime()
```


Gibt an, ob das Zahlenformat ein Datumsformat ist.

**Returns:**
boolean
### isFillApplied() {#isFillApplied--}
```
public boolean isFillApplied()
```


Gibt an, ob die Füllformatierung angewendet werden soll.

**Remarks**

Nur für benannten Stil.

**Returns:**
boolean
### isFontApplied() {#isFontApplied--}
```
public boolean isFontApplied()
```


Gibt an, ob die Schriftformatierung angewendet werden soll.

**Remarks**

Nur für benannten Stil.

**Returns:**
boolean
### isFormulaHidden() {#isFormulaHidden--}
```
public boolean isFormulaHidden()
```


Stellt dar, ob die Formel verborgen wird, wenn das Arbeitsblatt geschützt ist.

**Returns:**
boolean
### isGradient() {#isGradient--}
```
public boolean isGradient()
```


Gibt an, ob die Zellenhintergrundschattierung ein Verlaufsmuster ist.

**Returns:**
boolean
### isJustifyDistributed() {#isJustifyDistributed--}
```
public boolean isJustifyDistributed()
```


Gibt an, ob für die letzte Textzeile die Block‑ oder Verteilt‑Ausrichtung verwendet werden soll.

**Remarks**

Dies ist typisch für ostasiatische Ausrichtungen, aber nicht in anderen Kontexten. Funktioniert nur bei verteilter horizontaler Ausrichtung.

**Returns:**
boolean
### isLocked() {#isLocked--}
```
public boolean isLocked()
```


Ruft einen Wert ab, der angibt, ob eine Zelle bearbeitet werden kann oder nicht.

**Remarks**

Das Sperren von Zellen hat keine Wirkung, wenn das Arbeitsblatt nicht geschützt ist.

**Returns:**
boolean
### isModified(int modifyFlag) {#isModified-int-}
```
public boolean isModified(int modifyFlag)
```


Prüft, ob die angegebenen Eigenschaften des Stils geändert wurden. Wird für den Stil von ConditionalFormattings verwendet, um zu prüfen, ob die angegebenen Eigenschaften dieses Stils beim Anwenden von ConditionalFormattings auf eine Zelle verwendet werden sollen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| modifyFlag | int | [StyleModifyFlag](../../com.aspose.cells/stylemodifyflag). Stiländerungsflags |

**Returns:**
boolean - true, wenn die angegebenen Eigenschaften geändert wurden
### isNumberFormatApplied() {#isNumberFormatApplied--}
```
public boolean isNumberFormatApplied()
```


Gibt an, ob die Zahlenformatierung angewendet werden soll.

**Remarks**

Nur für benannten Stil.

**Returns:**
boolean
### isPercent() {#isPercent--}
```
public boolean isPercent()
```


Gibt an, ob das Zahlenformat ein Prozentformat ist.

**Returns:**
boolean
### isProtectionApplied() {#isProtectionApplied--}
```
public boolean isProtectionApplied()
```


Gibt an, ob die Schutzformatierung angewendet werden soll.

**Remarks**

Nur für benannten Stil.

**Returns:**
boolean
### isTextWrapped() {#isTextWrapped--}
```
public boolean isTextWrapped()
```


Ermittelt einen Wert, der angibt, ob der Text innerhalb einer Zelle umgebrochen ist.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setAlignmentApplied(boolean value) {#setAlignmentApplied-boolean-}
```
public void setAlignmentApplied(boolean value)
```


Gibt an, ob die Ausrichtungsformatierung angewendet werden soll.

**Remarks**

Nur für benannten Stil.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setBackgroundArgbColor(int value) {#setBackgroundArgbColor-int-}
```
public void setBackgroundArgbColor(int value)
```


Legt die Hintergrundfarbe mit einem 32‑Bit‑ARGB‑Wert fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setBackgroundColor(Color value) {#setBackgroundColor-com.aspose.cells.Color-}
```
public void setBackgroundColor(Color value)
```


Legt die Hintergrundfarbe eines Stils fest.

**Remarks**

Wenn Sie die Farbe einer Zelle festlegen möchten, verwenden Sie bitte die Eigenschaft Style.ForegroundColor. Nur wenn das Zellen-Style-Muster nicht „none“ oder „solid“ ist, wirkt sich diese Eigenschaft aus.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setBackgroundThemeColor(ThemeColor value) {#setBackgroundThemeColor-com.aspose.cells.ThemeColor-}
```
public void setBackgroundThemeColor(ThemeColor value)
```


Legt die Hintergrund‑Designfarbe fest.

**Remarks**

Wenn die Hintergrundfarbe keine Designfarbe ist, wird NULL zurückgegeben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [ThemeColor](../../com.aspose.cells/themecolor) |  |

### setBorder(int borderType, int borderStyle, CellsColor borderColor) {#setBorder-int-int-com.aspose.cells.CellsColor-}
```
public boolean setBorder(int borderType, int borderStyle, CellsColor borderColor)
```


Legt die Rahmen des Stils fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| borderType | int | [BorderType](../../com.aspose.cells/bordertype). Die zu setzenden Rahmen, können eine Kombination von [BorderType](../../com.aspose.cells/bordertype) sein. |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). Der Stil des Rahmens. |
| borderColor | [CellsColor](../../com.aspose.cells/cellscolor) | Die Farbe des Rahmens. |

**Returns:**
boolean - Ob die aktuellen Rahmen-Einstellungen geändert wurden.
### setBorder(int borderType, int borderStyle, Color borderColor) {#setBorder-int-int-com.aspose.cells.Color-}
```
public boolean setBorder(int borderType, int borderStyle, Color borderColor)
```


Legt die Rahmen des Stils fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| borderType | int | [BorderType](../../com.aspose.cells/bordertype). Die zu setzenden Rahmen, können eine Kombination von [BorderType](../../com.aspose.cells/bordertype) sein. |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). Der Stil des Rahmens. |
| borderColor | [Color](../../com.aspose.cells/color) | Die Farbe des Rahmens. |

**Returns:**
boolean - Ob die aktuellen Rahmen-Einstellungen geändert wurden.
### setBorderApplied(boolean value) {#setBorderApplied-boolean-}
```
public void setBorderApplied(boolean value)
```


Gibt an, ob die Rahmenformatierung angewendet werden soll.

**Remarks**

Nur für benannten Stil.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setCheckBox(boolean value) {#setCheckBox-boolean-}
```
public void setCheckBox(boolean value)
```


Gibt an, ob es sich um einen Stil für ein Kontrollkästchen handelt

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setCultureCustom(String value) {#setCultureCustom-java.lang.String-}
```
public void setCultureCustom(String value)
```


Legt die kulturspezifische Musterzeichenfolge für das Zahlenformat fest. Wenn für dieses Objekt kein Zahlenformat festgelegt wurde, wird null zurückgegeben. Ist das Zahlenformat eingebaut, wird die dem eingebauten Zahlenformat entsprechende Musterzeichenfolge zurückgegeben.

**Remarks**

Für eingebautes Zahlenformat sind sowohl der Musterinhalt (z. B. ein eingebautes Datumsformat ist \"m/d/y\" für einige Gebietsschemas, für andere wird es zu \"d/m/y\") als auch der Formatbezeichner (z. B. verwenden einige Gebietsschemas ein anderes Zeichen als 'y' für den Jahresanteil bei der Datumsformatierung) kulturbabhängig; Für vom Benutzer angegebenes benutzerdefiniertes Format werden nur die Formatbezeichner gemäß der Kultur geändert, andere Teile des Formatmusters bleiben unverändert.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setCustom(String value) {#setCustom-java.lang.String-}
```
public void setCustom(String value)
```


Stellt die benutzerdefinierte Zahlenformatzeichenfolge dieses Style-Objekts dar. Wenn das benutzerdefinierte Zahlenformat nicht festgelegt ist (z. B. das Zahlenformat ist eingebaut), wird \"\" zurückgegeben.

**Remarks**

Die zurückgegebene benutzerdefinierte Zeichenfolge ist kulturlos.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setCustom(String custom, boolean builtinPreference) {#setCustom-java.lang.String-boolean-}
```
public void setCustom(String custom, boolean builtinPreference)
```


Legt die benutzerdefinierte Zahlenformatzeichenfolge einer Zelle fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| benutzerdefiniert | java.lang.String | Benutzerdefinierte Zahlenformatzeichenfolge, sollte das InvariantCulture-Muster sein. |
| builtinPreference | boolean | Wenn die angegebene benutzerdefinierte Zahlenformatzeichenfolge mit einem der integrierten Zahlenformate übereinstimmt, die den aktuellen regionalen Einstellungen entsprechen, wird das Zahlenformat als eingebaut statt als benutzerdefiniert festgelegt. |

### setFillApplied(boolean value) {#setFillApplied-boolean-}
```
public void setFillApplied(boolean value)
```


Gibt an, ob die Füllformatierung angewendet werden soll.

**Remarks**

Nur für benannten Stil.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setFontApplied(boolean value) {#setFontApplied-boolean-}
```
public void setFontApplied(boolean value)
```


Gibt an, ob die Schriftformatierung angewendet werden soll.

**Remarks**

Nur für benannten Stil.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setForegroundArgbColor(int value) {#setForegroundArgbColor-int-}
```
public void setForegroundArgbColor(int value)
```


Legt die Vordergrundfarbe mit einem 32‑Bit‑ARGB‑Wert fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setForegroundColor(Color value) {#setForegroundColor-com.aspose.cells.Color-}
```
public void setForegroundColor(Color value)
```


Legt die Vordergrundfarbe eines Stils fest.

**Remarks**

Das bedeutet, dass keine Farbe eingestellt ist, wenn Color.Empty zurückgegeben wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setForegroundThemeColor(ThemeColor value) {#setForegroundThemeColor-com.aspose.cells.ThemeColor-}
```
public void setForegroundThemeColor(ThemeColor value)
```


Legt die Vordergrund‑Designfarbe fest.

**Remarks**

Wenn die Vordergrundfarbe keine Designfarbe ist, wird NULL zurückgegeben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [ThemeColor](../../com.aspose.cells/themecolor) |  |

### setFormulaHidden(boolean value) {#setFormulaHidden-boolean-}
```
public void setFormulaHidden(boolean value)
```


Stellt dar, ob die Formel verborgen wird, wenn das Arbeitsblatt geschützt ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setGradient(boolean value) {#setGradient-boolean-}
```
public void setGradient(boolean value)
```


Gibt an, ob die Zellenhintergrundschattierung ein Verlaufsmuster ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setHorizontalAlignment(int value) {#setHorizontalAlignment-int-}
```
public void setHorizontalAlignment(int value)
```


Legt den horizontalen Ausrichtungstyp des Textes in einer Zelle fest.

Siehe [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setIndentLevel(int value) {#setIndentLevel-int-}
```
public void setIndentLevel(int value)
```


Stellt die Einzugsebene für die Zelle oder den Bereich dar. Kann nur ein ganzzahliger Wert von 0 bis 250 sein.

**Remarks**

Wenn die horizontale Ausrichtung des Textes auf einen anderen Wert als links oder rechts gesetzt wird, wird die Einzugsebene auf Null zurückgesetzt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setJustifyDistributed(boolean value) {#setJustifyDistributed-boolean-}
```
public void setJustifyDistributed(boolean value)
```


Gibt an, ob für die letzte Textzeile die Block‑ oder Verteilt‑Ausrichtung verwendet werden soll.

**Remarks**

Dies ist typisch für ostasiatische Ausrichtungen, aber nicht in anderen Kontexten. Funktioniert nur bei verteilter horizontaler Ausrichtung.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


Legt einen Wert fest, der angibt, ob eine Zelle bearbeitet werden kann oder nicht.

**Remarks**

Das Sperren von Zellen hat keine Wirkung, wenn das Arbeitsblatt nicht geschützt ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Legt den Namen des Stils fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setNumber(int value) {#setNumber-int-}
```
public void setNumber(int value)
```


Legt das Anzeigeformat von Zahlen und Datumsangaben fest. Die Formatierungsmuster unterscheiden sich je nach Region.

**Remarks**

Beispielweise werden die Formatierungsmuster für die Region en\\_US durch Zahlen dargestellt:

| Value | Typ | Formatzeichenfolge |
| ----- | ---------- | ---------------------------------------------------- |
| 0 | General | `General` |
| 1 | Decimal | `0` |
| 2 | Decimal | `0.00` |
| 3 | Decimal | `#,##0` |
| 4 | Decimal | `#,##0.00` |
| 5 | Currency | `$#,##0_);($#,##0)` |
| 6 | Currency | `$#,##0_);[Red](../$#,##0)` |
| 7 | Currency | `$#,##0.00_);($#,##0.00)` |
| 8 | Currency | `$#,##0.00_);[Rot](../$#,##0.00)` |
| 9 | Percentage | `0%` |
| 10 | Percentage | `0.00%` |
| 11 | Scientific | `0.00E+00` |
| 12 | Fraction | `# ?/?` |
| 13 | Fraction | `# ??/??` |
| 14 | Date | `m/d/yyyy` |
| 15 | Date | `d-mmm-yy` |
| 16 | Date | `d-mmm` |
| 17 | Date | `mmm-yy` |
| 18 | Time | `h:mm AM/PM` |
| 19 | Time | `h:mm:ss AM/PM` |
| 20 | Time | `h:mm` |
| 21 | Time | `h:mm:ss` |
| 22 | Time | `m/d/yyyy h:mm` |
| 37 | Accounting | `#,##0_);(#,##0)` |
| 38 | Accounting | `#,##0_);[Rot](../#,##0)` |
| 39 | Accounting | `#,##0.00_);(#,##0.00)` |
| 40 | Accounting | `#,##0.00_);[Rot](../#,##0.00)` |
| 41 | Accounting | `_(* #,##0_);_(* (#,##0);_(* "-"_);_(@_)` |
| 42 | Currency | `_($* #,##0_);_($* (#,##0);_($* "-"_);_(@_)` |
| 43 | Accounting | `_(* #,##0.00_);_(* (#,##0.00);_(* "-"??_);_(@_)` |
| 44 | Currency | `_($* #,##0.00_);_($* (#,##0.00);_($* "-"??_);_(@_)` |
| 45 | Time | `mm:ss` |
| 46 | Time | `[h]:mm:ss` |
| 47 | Time | `mm:ss.0` |
| 48 | Scientific | `##0.0E+0` |
| 49 | Text | `@` |

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setNumberFormatApplied(boolean value) {#setNumberFormatApplied-boolean-}
```
public void setNumberFormatApplied(boolean value)
```


Gibt an, ob die Zahlenformatierung angewendet werden soll.

**Remarks**

Nur für benannten Stil.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setOutlineBorders(int borderStyle, CellsColor borderColor) {#setOutlineBorders-int-com.aspose.cells.CellsColor-}
```
public void setOutlineBorders(int borderStyle, CellsColor borderColor)
```


Lege die Umrissrahmen fest

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). Der Typ der Rahmen. |
| borderColor | [CellsColor](../../com.aspose.cells/cellscolor) | Die Farbe der Rahmen |

### setOutlineBorders(int borderStyle, Color borderColor) {#setOutlineBorders-int-com.aspose.cells.Color-}
```
public void setOutlineBorders(int borderStyle, Color borderColor)
```


Lege die Umrissrahmen fest

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). Der Typ der Rahmen. |
| borderColor | [Color](../../com.aspose.cells/color) | Die Farbe der Rahmen |

### setPattern(int value) {#setPattern-int-}
```
public void setPattern(int value)
```


Legt den Hintergrundmustertyp der Zelle fest.

Siehe [BackgroundType](../../com.aspose.cells/backgroundtype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setPatternColor(int pattern, Color color1, Color color2) {#setPatternColor-int-com.aspose.cells.Color-com.aspose.cells.Color-}
```
public void setPatternColor(int pattern, Color color1, Color color2)
```


Legt die Hintergrundfarbe fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| pattern | int | [BackgroundType](../../com.aspose.cells/backgroundtype). Das Muster. |
| color1 | [Color](../../com.aspose.cells/color) | Die Vordergrundfarbe. |
| color2 | [Color](../../com.aspose.cells/color) | Die Hintergrundfarbe. Funktioniert nur, wenn das Muster nicht BackgroundType.None und BackgroundType.Solid ist. |

### setProtectionApplied(boolean value) {#setProtectionApplied-boolean-}
```
public void setProtectionApplied(boolean value)
```


Gibt an, ob die Schutzformatierung angewendet werden soll.

**Remarks**

Nur für benannten Stil.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setQuotePrefix(boolean value) {#setQuotePrefix-boolean-}
```
public void setQuotePrefix(boolean value)
```


Gibt an, ob der Zellenwert mit einem einfachen Anführungszeichen beginnt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setRotationAngle(int value) {#setRotationAngle-int-}
```
public void setRotationAngle(int value)
```


Stellt den Textdrehwinkel dar.

**Remarks**

0: Nicht gedreht.

255: Oben nach unten.

\-90: Abwärts.

90: Aufwärts.

Sie können 255 oder einen Wert im Bereich von -90 bis 90 setzen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setShrinkToFit(boolean value) {#setShrinkToFit-boolean-}
```
public void setShrinkToFit(boolean value)
```


Stellt dar, ob der Text automatisch verkleinert wird, um in die verfügbare Spaltenbreite zu passen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setTextDirection(int value) {#setTextDirection-int-}
```
public void setTextDirection(int value)
```


Stellt die Lesereihenfolge des Textes dar.

Siehe [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setTextWrapped(boolean value) {#setTextWrapped-boolean-}
```
public void setTextWrapped(boolean value)
```


Legt einen Wert fest, der angibt, ob der Text innerhalb einer Zelle umgebrochen ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setTwoColorGradient(Color color1, Color color2, int gradientStyleType, int variant) {#setTwoColorGradient-com.aspose.cells.Color-com.aspose.cells.Color-int-int-}
```
public void setTwoColorGradient(Color color1, Color color2, int gradientStyleType, int variant)
```


Setzt die angegebene Füllung auf einen Zweifarbverlauf.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| color1 | [Color](../../com.aspose.cells/color) | Eine Farbverlauffarbe. |
| color2 | [Color](../../com.aspose.cells/color) | Zwei Gradientfarben. |
| gradientStyleType | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). Gradient-Schattierungsstil. |
| Variante | int | Die Gradientvariante. Kann ein Wert von 1 bis 4 sein, entsprechend einer der vier Varianten auf der Registerkarte Gradient im Dialogfeld Fülleffekte. Wenn der Stil GradientStyle.FromCenter ist, kann das Variant-Argument nur 1 oder 2 sein. |

### setVerticalAlignment(int value) {#setVerticalAlignment-int-}
```
public void setVerticalAlignment(int value)
```


Legt den vertikalen Ausrichtungstyp des Textes in einer Zelle fest.

Siehe [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### toJson() {#toJson--}
```
public String toJson()
```


Konvertiere [Style](../../com.aspose.cells/style) in JSON‑Strukturdaten.

**Returns:**
java.lang.String -
### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### update() {#update--}
```
public void update()
```


Wenden Sie den benannten Stil auf die Stile der Zellen an, die diesen benannten Stil verwenden. Es funktioniert wie das Klicken auf die Schaltfläche "ok", nachdem Sie den Stil bearbeitet haben. Gilt nur für benannte Stile.

### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

