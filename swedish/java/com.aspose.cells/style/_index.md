---
title: "Style"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar visningsstil för Excel-dokument såsom teckensnitt, färg, justering, kant etc."
type: docs
url: /sv/java/com.aspose.cells/style/
---

**Inheritance:**
java.lang.Object
```
public class Style
```

Representerar visningsstil för Excel-dokument, såsom teckensnitt, färg, justering, kant, etc. Style-objektet innehåller alla stilattribut (teckensnitt, talformat, justering och så vidare) som egenskaper.

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
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [Style()](#Style--) | Initierar en ny instans av klassen [Style](../../com.aspose.cells/style). |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [copy(Style style)](#copy-com.aspose.cells.Style-) | Kopierar data från ett annat stilobjekt |
| [equals(Object obj)](#equals-java.lang.Object-) | Bestämmer om två Style-instansers är lika. |
| [getBackgroundArgbColor()](#getBackgroundArgbColor--) | Hämtar bakgrundsfärgen med ett 32-bitars ARGB-värde. |
| [getBackgroundColor()](#getBackgroundColor--) | Hämtar en stils bakgrundsfärg. |
| [getBackgroundThemeColor()](#getBackgroundThemeColor--) | Hämtar bakgrundens temafärg. |
| [getBorders()](#getBorders--) | Hämtar [BorderCollection](../../com.aspose.cells/bordercollection) för stilen. |
| [getBottomBorder()](#getBottomBorder--) | Hämtar den nedre kanten. |
| [getClass()](#getClass--) |  |
| [getCultureCustom()](#getCultureCustom--) | Hämtar den kulturberoende mönsterssträngen för talformat. |
| [getCustom()](#getCustom--) | Representerar den anpassade talformatsträngen för detta stilobjekt. |
| [getFont()](#getFont--) | Hämtar ett [getFont()](../../com.aspose.cells/style\#getFont--)‑objekt. |
| [getForegroundArgbColor()](#getForegroundArgbColor--) | Hämtar förgrundsfärgen med ett 32-bitars ARGB‑värde. |
| [getForegroundColor()](#getForegroundColor--) | Hämtar en stils förgrundsfärg. |
| [getForegroundThemeColor()](#getForegroundThemeColor--) | Hämtar förgrundens temafärg. |
| [getHorizontalAlignment()](#getHorizontalAlignment--) | Hämtar den horisontella justeringstypen för texten i en cell. |
| [getIndentLevel()](#getIndentLevel--) | Representerar indenteringsnivån för cellen eller området. |
| [getInvariantCustom()](#getInvariantCustom--) | Hämtar den kulturoberoende mönsterssträngen för talformat. |
| [getLeftBorder()](#getLeftBorder--) | Hämtar den vänstra kanten. |
| [getName()](#getName--) | Hämtar namnet på stilen. |
| [getNumber()](#getNumber--) | Hämtar visningsformatet för tal och datum. |
| [getParentStyle()](#getParentStyle--) | Hämtar förälderstilen för den här stilen. |
| [getPattern()](#getPattern--) | Hämtar cellens bakgrundsmönstertyp. |
| [getQuotePrefix()](#getQuotePrefix--) | Anger om cellens värde börjar med ett enkelt citattecken. |
| [getRightBorder()](#getRightBorder--) | Hämtar den högra kanten. |
| [getRotationAngle()](#getRotationAngle--) | Representerar textrotationsvinkeln. |
| [getShrinkToFit()](#getShrinkToFit--) | Representerar om text automatiskt krymper för att passa i den tillgängliga kolumnbredden. |
| [getTextDirection()](#getTextDirection--) | Representerar textens läsriktning. |
| [getTopBorder()](#getTopBorder--) | Hämtar den övre kanten. |
| [getTwoColorGradient()](#getTwoColorGradient--) | Hämta tvåfärgsgradientinställningen. |
| [getTwoColorGradientSetting()](#getTwoColorGradientSetting--) | Hämta tvåfärgsgradientinställningen. |
| [getVerticalAlignment()](#getVerticalAlignment--) | Hämtar den vertikala justeringstypen för text i en cell. |
| [hasBorders()](#hasBorders--) | Kontrollerar om kanter har ställts in för stilen. |
| [hashCode()](#hashCode--) | Fungerar som en hash-funktion för ett Style-objekt. |
| [isAlignmentApplied()](#isAlignmentApplied--) | Anger om justeringsformatering ska tillämpas. |
| [isBorderApplied()](#isBorderApplied--) | Anger om kantformatering ska tillämpas. |
| [isCheckBox()](#isCheckBox--) | Anger om det är en stil för kryssruta |
| [isDateTime()](#isDateTime--) | Anger om talformatet är ett datumformat. |
| [isFillApplied()](#isFillApplied--) | Anger om fyllnadsformatering ska tillämpas. |
| [isFontApplied()](#isFontApplied--) | Anger om teckensnittsformatering ska tillämpas. |
| [isFormulaHidden()](#isFormulaHidden--) | Representerar om formeln kommer att döljas när kalkylbladet är skyddat. |
| [isGradient()](#isGradient--) | Anger om cellskuggning är ett gradientmönster. |
| [isJustifyDistributed()](#isJustifyDistributed--) | Anger om cellerna ska ha justerad eller fördelad justering på den sista textraden. |
| [isLocked()](#isLocked--) | Hämtar ett värde som indikerar om en cell kan modifieras eller inte. |
| [isModified(int modifyFlag)](#isModified-int-) | Kontrollerar om de angivna egenskaperna för stilen har modifierats. |
| [isNumberFormatApplied()](#isNumberFormatApplied--) | Anger om talformatering ska tillämpas. |
| [isPercent()](#isPercent--) | Anger om talformatet är ett procentformat. |
| [isProtectionApplied()](#isProtectionApplied--) | Anger om skyddsformatering ska tillämpas. |
| [isTextWrapped()](#isTextWrapped--) | Hämtar ett värde som indikerar om texten i en cell är radbruten. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAlignmentApplied(boolean value)](#setAlignmentApplied-boolean-) | Anger om justeringsformatering ska tillämpas. |
| [setBackgroundArgbColor(int value)](#setBackgroundArgbColor-int-) | Ställer in bakgrundsfärgen med ett 32-bitars ARGB‑värde. |
| [setBackgroundColor(Color value)](#setBackgroundColor-com.aspose.cells.Color-) | Ställer in en stils bakgrundsfärg. |
| [setBackgroundThemeColor(ThemeColor value)](#setBackgroundThemeColor-com.aspose.cells.ThemeColor-) | Ställer in bakgrundens temafärg. |
| [setBorder(int borderType, int borderStyle, CellsColor borderColor)](#setBorder-int-int-com.aspose.cells.CellsColor-) | Ställer in stilens kanter. |
| [setBorder(int borderType, int borderStyle, Color borderColor)](#setBorder-int-int-com.aspose.cells.Color-) | Ställer in stilens kanter. |
| [setBorderApplied(boolean value)](#setBorderApplied-boolean-) | Anger om kantformatering ska tillämpas. |
| [setCheckBox(boolean value)](#setCheckBox-boolean-) | Anger om det är en stil för kryssruta |
| [setCultureCustom(String value)](#setCultureCustom-java.lang.String-) | Ställer in den kulturspecifika mönsterssträngen för talformat. |
| [setCustom(String value)](#setCustom-java.lang.String-) | Representerar den anpassade talformatsträngen för detta stilobjekt. |
| [setCustom(String custom, boolean builtinPreference)](#setCustom-java.lang.String-boolean-) | Ställer in den anpassade talformatsträngen för en cell. |
| [setFillApplied(boolean value)](#setFillApplied-boolean-) | Anger om fyllnadsformatering ska tillämpas. |
| [setFontApplied(boolean value)](#setFontApplied-boolean-) | Anger om teckensnittsformatering ska tillämpas. |
| [setForegroundArgbColor(int value)](#setForegroundArgbColor-int-) | Ställer in förgrundsfärgen med ett 32-bitars ARGB‑värde. |
| [setForegroundColor(Color value)](#setForegroundColor-com.aspose.cells.Color-) | Ställer in en stils förgrundsfärg. |
| [setForegroundThemeColor(ThemeColor value)](#setForegroundThemeColor-com.aspose.cells.ThemeColor-) | Ställer in förgrundens temafärg. |
| [setFormulaHidden(boolean value)](#setFormulaHidden-boolean-) | Representerar om formeln kommer att döljas när kalkylbladet är skyddat. |
| [setGradient(boolean value)](#setGradient-boolean-) | Anger om cellskuggning är ett gradientmönster. |
| [setHorizontalAlignment(int value)](#setHorizontalAlignment-int-) | Ställer in den horisontella justeringstypen för texten i en cell. |
| [setIndentLevel(int value)](#setIndentLevel-int-) | Representerar indenteringsnivån för cellen eller området. |
| [setJustifyDistributed(boolean value)](#setJustifyDistributed-boolean-) | Anger om cellerna ska ha justerad eller fördelad justering på den sista textraden. |
| [setLocked(boolean value)](#setLocked-boolean-) | Ställer in ett värde som indikerar om en cell kan modifieras eller inte. |
| [setName(String value)](#setName-java.lang.String-) | Ställer in stilens namn. |
| [setNumber(int value)](#setNumber-int-) | Ställer in visningsformatet för tal och datum. |
| [setNumberFormatApplied(boolean value)](#setNumberFormatApplied-boolean-) | Anger om talformatering ska tillämpas. |
| [setOutlineBorders(int borderStyle, CellsColor borderColor)](#setOutlineBorders-int-com.aspose.cells.CellsColor-) | Ställ in konturkanterna |
| [setOutlineBorders(int borderStyle, Color borderColor)](#setOutlineBorders-int-com.aspose.cells.Color-) | Ställ in konturkanterna |
| [setPattern(int value)](#setPattern-int-) | Ställer in cellens bakgrundsmönstertyp. |
| [setPatternColor(int pattern, Color color1, Color color2)](#setPatternColor-int-com.aspose.cells.Color-com.aspose.cells.Color-) | Ställer in bakgrundsfärgen. |
| [setProtectionApplied(boolean value)](#setProtectionApplied-boolean-) | Anger om skyddsformatering ska tillämpas. |
| [setQuotePrefix(boolean value)](#setQuotePrefix-boolean-) | Anger om cellens värde börjar med ett enkelt citattecken. |
| [setRotationAngle(int value)](#setRotationAngle-int-) | Representerar textrotationsvinkeln. |
| [setShrinkToFit(boolean value)](#setShrinkToFit-boolean-) | Representerar om text automatiskt krymper för att passa i den tillgängliga kolumnbredden. |
| [setTextDirection(int value)](#setTextDirection-int-) | Representerar textens läsriktning. |
| [setTextWrapped(boolean value)](#setTextWrapped-boolean-) | Ställer in ett värde som indikerar om texten i en cell är radbruten. |
| [setTwoColorGradient(Color color1, Color color2, int gradientStyleType, int variant)](#setTwoColorGradient-com.aspose.cells.Color-com.aspose.cells.Color-int-int-) | Ställer in den angivna fyllningen till en tvåfärgsgradient. |
| [setVerticalAlignment(int value)](#setVerticalAlignment-int-) | Ställer in den vertikala justeringstypen för texten i en cell. |
| [toJson()](#toJson--) | Konvertera [Style](../../com.aspose.cells/style) till JSON‑strukturdatan. |
| [toString()](#toString--) |  |
| [update()](#update--) | Applicera den namngivna stilen på cellernas stilar som använder denna namngivna stil. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### Style() {#Style--}
```
public Style()
```


Initierar en ny instans av klassen [Style](../../com.aspose.cells/style).

**Remarks**

OBS: Denna konstruktor är nu föråldrad. Använd istället CellsFactory.CreateStyle()‑metoden. Denna egenskap kommer att tas bort 6 månader senare sedan oktober 2016. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### copy(Style style) {#copy-com.aspose.cells.Style-}
```
public void copy(Style style)
```


Kopierar data från ett annat stilobjekt

**Remarks**

Denna metod kopierar inte stilens namn. Om du vill kopiera namnet, anropa följande kod efter att ha kopierat stilen: destStyle.Name = style.Name.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | Källstilobjekt |

### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Bestämmer om två Style-instansers är lika.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| obj | java.lang.Object | Stil‑objektet att jämföra med det aktuella Stil‑objektet. |

**Returns:**
boolean - sant om det angivna objektet är lika med det aktuella objektet; annars falskt.
### getBackgroundArgbColor() {#getBackgroundArgbColor--}
```
public int getBackgroundArgbColor()
```


Hämtar bakgrundsfärgen med ett 32-bitars ARGB-värde.

**Returns:**
int
### getBackgroundColor() {#getBackgroundColor--}
```
public Color getBackgroundColor()
```


Hämtar en stils bakgrundsfärg.

**Remarks**

Om du vill ange en cells färg, använd egenskapen Style.ForegroundColor. Endast om cellstils mönster är annat än ingen eller solid kommer denna egenskap att ha effekt.

**Returns:**
[Color](../../com.aspose.cells/color)
### getBackgroundThemeColor() {#getBackgroundThemeColor--}
```
public ThemeColor getBackgroundThemeColor()
```


Hämtar bakgrundens temafärg.

**Remarks**

Om bakgrundsfärgen inte är en temafärg returneras NULL.

**Returns:**
[ThemeColor](../../com.aspose.cells/themecolor)
### getBorders() {#getBorders--}
```
public BorderCollection getBorders()
```


Hämtar [BorderCollection](../../com.aspose.cells/bordercollection) för stilen.

**Returns:**
[BorderCollection](../../com.aspose.cells/bordercollection)
### getBottomBorder() {#getBottomBorder--}
```
public Border getBottomBorder()
```


Hämtar den nedre kanten.

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


Hämtar det kulturberoende mönstersträngen för talformat. Om inget talformat har angetts för detta objekt returneras null. Om talformatet är inbyggt returneras mönstersträngen som motsvarar det inbyggda talet.

**Remarks**

För inbyggt talformat är både mönsterinnehållet (t.ex. ett inbyggt datumformat är "m/d/y" för vissa språkversioner, men för andra blir det "d/m/y") och formatavgränsaren (t.ex. vissa språkversioner använder ett annat tecken än 'y' för att representera årsdelen i datumformat) kulturberoende; för ett användarspecificerat anpassat format ändras endast formatavgränsarna enligt kulturen, övriga delar av formateringsmönstret modifieras inte.

**Returns:**
java.lang.String
### getCustom() {#getCustom--}
```
public String getCustom()
```


Representerar den anpassade talformatsträngen för detta stilobjekt. Om det anpassade talformatet inte är angivet (t.ex. talformatet är inbyggt) returneras "".

**Remarks**

Den returnerade anpassade strängen är kulturoberoende.

**Returns:**
java.lang.String
### getFont() {#getFont--}
```
public Font getFont()
```


Hämtar ett [getFont()](../../com.aspose.cells/style\#getFont--)‑objekt.

**Returns:**
[Font](../../com.aspose.cells/font)
### getForegroundArgbColor() {#getForegroundArgbColor--}
```
public int getForegroundArgbColor()
```


Hämtar förgrundsfärgen med ett 32-bitars ARGB‑värde.

**Returns:**
int
### getForegroundColor() {#getForegroundColor--}
```
public Color getForegroundColor()
```


Hämtar en stils förgrundsfärg.

**Remarks**

Det betyder ingen färginställning om Color.Empty returneras.

**Returns:**
[Color](../../com.aspose.cells/color)
### getForegroundThemeColor() {#getForegroundThemeColor--}
```
public ThemeColor getForegroundThemeColor()
```


Hämtar förgrundens temafärg.

**Remarks**

Om förgrundsfärgen inte är en temafärg returneras NULL.

**Returns:**
[ThemeColor](../../com.aspose.cells/themecolor)
### getHorizontalAlignment() {#getHorizontalAlignment--}
```
public int getHorizontalAlignment()
```


Hämtar den horisontella justeringstypen för texten i en cell.

Se [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Returns:**
int
### getIndentLevel() {#getIndentLevel--}
```
public int getIndentLevel()
```


Representerar indenteringsnivån för cellen eller området. Kan endast vara ett heltal mellan 0 och 250.

**Remarks**

Om horisontell justeringstyp för text är inställd på ett värde annat än vänster eller höger återställs indenteringsnivån till noll.

**Returns:**
int
### getInvariantCustom() {#getInvariantCustom--}
```
public String getInvariantCustom()
```


Hämtar den kulturoberoende mönstersträngen för talformat. Om inget talformat har angetts för detta objekt returneras null. Om talformatet är inbyggt returneras mönstersträngen som motsvarar det inbyggda talet.

**Remarks**

För inbyggda talformat är det returnerade mönsterinnehållet fortfarande kulturberoende, till exempel returnerar vissa språkversioner "m/d/y" och andra "d/m/y". Skillnaden från [getCultureCustom()](../../com.aspose.cells/style\#getCultureCustom--) är (det är också vad kulturoberoende betyder): formatavgränsare och separatorer behålls som standard, så '/' används alltid som datum‑ och tidsseparator och "y" alltid används för "år"‑delen oavsett vilket annat specialtecken som används för den specifika språkversionen.

**Returns:**
java.lang.String
### getLeftBorder() {#getLeftBorder--}
```
public Border getLeftBorder()
```


Hämtar den vänstra kanten.

**Returns:**
[Border](../../com.aspose.cells/border)
### getName() {#getName--}
```
public String getName()
```


Hämtar namnet på stilen.

**Returns:**
java.lang.String
### getNumber() {#getNumber--}
```
public int getNumber()
```


Hämtar visningsformatet för tal och datum. Formateringsmönstren skiljer sig åt mellan olika regioner.

**Remarks**

Till exempel, formateringsmönstren som representeras av siffror för regionen en\_US:

| Värde | Typ | Formateringssträng |
| ----- | ---------- | ---------------------------------------------------- |
| 0 | General | `General` |
| 1 | Decimal | `0` |
| 2 | Decimal | `0.00` |
| 3 | Decimal | `#,##0` |
| 4 | Decimal | `#,##0.00` |
| 5 | Currency | `$#,##0_);($#,##0)` |
| 6 | Currency | `$#,##0_);[Red](../$#,##0)` |
| 7 | Currency | `$#,##0.00_);($#,##0.00)` |
| 8 | Currency | `$#,##0.00_);[Red](../$#,##0.00)` |
| 9 | Percentage | `0%` |
| 10 | Percentage | `0.00%` |
| 11 | Scientific | `0.00E+00` |
| 12 | Fraction | `# ?/?` |
| 13 | Fraction | `# ??/??` |
| 14 | Date | `m/d/yyyy` |
| 15 | Date | `d-mmm-yy` |
| 16 | Date | `d-mmm` |
| 17 | Date | `mmm-yy` |
| 18 | Time | `h:mm FM/EM` |
| 19 | Time | `h:mm:ss FM/EM` |
| 20 | Time | `h:mm` |
| 21 | Time | `h:mm:ss` |
| 22 | Time | `m/d/yyyy h:mm` |
| 37 | Accounting | `#,##0_);(#,##0)` |
| 38 | Accounting | `#,##0_);[Röd](../#,##0)` |
| 39 | Accounting | `#,##0.00_);(#,##0.00)` |
| 40 | Accounting | `#,##0.00_);[Röd](../#,##0.00)` |
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


Hämtar förälderstilen för den här stilen.

**Returns:**
[Style](../../com.aspose.cells/style)
### getPattern() {#getPattern--}
```
public int getPattern()
```


Hämtar cellens bakgrundsmönstertyp.

Se [BackgroundType](../../com.aspose.cells/backgroundtype).

**Returns:**
int
### getQuotePrefix() {#getQuotePrefix--}
```
public boolean getQuotePrefix()
```


Anger om cellens värde börjar med ett enkelt citattecken.

**Returns:**
boolean
### getRightBorder() {#getRightBorder--}
```
public Border getRightBorder()
```


Hämtar den högra kanten.

**Returns:**
[Border](../../com.aspose.cells/border)
### getRotationAngle() {#getRotationAngle--}
```
public int getRotationAngle()
```


Representerar textrotationsvinkeln.

**Remarks**

0: Inte roterad.

255: Från topp till botten.

\-90: Nedåt.

90: Uppåt.

Du kan ange 255 eller ett värde mellan -90 och 90.

**Returns:**
int
### getShrinkToFit() {#getShrinkToFit--}
```
public boolean getShrinkToFit()
```


Representerar om text automatiskt krymper för att passa i den tillgängliga kolumnbredden.

**Returns:**
boolean
### getTextDirection() {#getTextDirection--}
```
public int getTextDirection()
```


Representerar textens läsriktning.

Se [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Returns:**
int
### getTopBorder() {#getTopBorder--}
```
public Border getTopBorder()
```


Hämtar den övre kanten.

**Returns:**
[Border](../../com.aspose.cells/border)
### getTwoColorGradient() {#getTwoColorGradient--}
```
public Object[] getTwoColorGradient()
```


Hämta tvåfärgsgradientinställningen.

**Remarks**

OBS: Denna metod är nu föråldrad. Använd istället metoden Style.GetTwoColorGradientSetting(). Denna egenskap kommer att tas bort 12 månader senare sedan december 2022. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Returns:**
java.lang.Object[] - Returnerar alla inställningar för tvåfärgsgradient [0] : Color1 [1] : Color2 [2] : GradientStyleType [3] : Variant
### getTwoColorGradientSetting() {#getTwoColorGradientSetting--}
```
public TwoColorGradient getTwoColorGradientSetting()
```


Hämta tvåfärgsgradientinställningen.

**Returns:**
[TwoColorGradient](../../com.aspose.cells/twocolorgradient)
### getVerticalAlignment() {#getVerticalAlignment--}
```
public int getVerticalAlignment()
```


Hämtar den vertikala justeringstypen för text i en cell.

Se [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Returns:**
int
### hasBorders() {#hasBorders--}
```
public boolean hasBorders()
```


Kontrollerar om kanter har ställts in för stilen.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public int hashCode()
```


Fungerar som en hash-funktion för ett Style-objekt.

**Remarks**

Denna metod är endast för internt bruk.

**Returns:**
int - En hashkod för det aktuella objektet.
### isAlignmentApplied() {#isAlignmentApplied--}
```
public boolean isAlignmentApplied()
```


Anger om justeringsformatering ska tillämpas.

**Remarks**

Endast för namngiven stil.

**Returns:**
boolean
### isBorderApplied() {#isBorderApplied--}
```
public boolean isBorderApplied()
```


Anger om kantformatering ska tillämpas.

**Remarks**

Endast för namngiven stil.

**Returns:**
boolean
### isCheckBox() {#isCheckBox--}
```
public boolean isCheckBox()
```


Anger om det är en stil för kryssruta

**Returns:**
boolean
### isDateTime() {#isDateTime--}
```
public boolean isDateTime()
```


Anger om talformatet är ett datumformat.

**Returns:**
boolean
### isFillApplied() {#isFillApplied--}
```
public boolean isFillApplied()
```


Anger om fyllnadsformatering ska tillämpas.

**Remarks**

Endast för namngiven stil.

**Returns:**
boolean
### isFontApplied() {#isFontApplied--}
```
public boolean isFontApplied()
```


Anger om teckensnittsformatering ska tillämpas.

**Remarks**

Endast för namngiven stil.

**Returns:**
boolean
### isFormulaHidden() {#isFormulaHidden--}
```
public boolean isFormulaHidden()
```


Representerar om formeln kommer att döljas när kalkylbladet är skyddat.

**Returns:**
boolean
### isGradient() {#isGradient--}
```
public boolean isGradient()
```


Anger om cellskuggning är ett gradientmönster.

**Returns:**
boolean
### isJustifyDistributed() {#isJustifyDistributed--}
```
public boolean isJustifyDistributed()
```


Anger om cellerna ska ha justerad eller fördelad justering på den sista textraden.

**Remarks**

Detta är typiskt för östasiatiska justeringar men inte i andra sammanhang. Fungerar endast när horisontell justering är fördelad.

**Returns:**
boolean
### isLocked() {#isLocked--}
```
public boolean isLocked()
```


Hämtar ett värde som indikerar om en cell kan modifieras eller inte.

**Remarks**

Låsning av celler har ingen effekt om inte kalkylbladet är skyddat.

**Returns:**
boolean
### isModified(int modifyFlag) {#isModified-int-}
```
public boolean isModified(int modifyFlag)
```


Kontrollerar om de angivna egenskaperna för stilen har ändrats. Används för stil av ConditionalFormattings för att kontrollera om de angivna egenskaperna för denna stil ska användas när ConditionalFormattings tillämpas på en cell.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| modifyFlag | int | [StyleModifyFlag](../../com.aspose.cells/stylemodifyflag). Flaggor för ändrad stil |

**Returns:**
boolean - sant om de angivna egenskaperna har ändrats
### isNumberFormatApplied() {#isNumberFormatApplied--}
```
public boolean isNumberFormatApplied()
```


Anger om talformatering ska tillämpas.

**Remarks**

Endast för namngiven stil.

**Returns:**
boolean
### isPercent() {#isPercent--}
```
public boolean isPercent()
```


Anger om talformatet är ett procentformat.

**Returns:**
boolean
### isProtectionApplied() {#isProtectionApplied--}
```
public boolean isProtectionApplied()
```


Anger om skyddsformatering ska tillämpas.

**Remarks**

Endast för namngiven stil.

**Returns:**
boolean
### isTextWrapped() {#isTextWrapped--}
```
public boolean isTextWrapped()
```


Hämtar ett värde som indikerar om texten i en cell är radbruten.

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


Anger om justeringsformatering ska tillämpas.

**Remarks**

Endast för namngiven stil.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setBackgroundArgbColor(int value) {#setBackgroundArgbColor-int-}
```
public void setBackgroundArgbColor(int value)
```


Ställer in bakgrundsfärgen med ett 32-bitars ARGB‑värde.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setBackgroundColor(Color value) {#setBackgroundColor-com.aspose.cells.Color-}
```
public void setBackgroundColor(Color value)
```


Ställer in en stils bakgrundsfärg.

**Remarks**

Om du vill ange en cells färg, använd egenskapen Style.ForegroundColor. Endast om cellstils mönster är annat än ingen eller solid kommer denna egenskap att ha effekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setBackgroundThemeColor(ThemeColor value) {#setBackgroundThemeColor-com.aspose.cells.ThemeColor-}
```
public void setBackgroundThemeColor(ThemeColor value)
```


Ställer in bakgrundens temafärg.

**Remarks**

Om bakgrundsfärgen inte är en temafärg returneras NULL.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [ThemeColor](../../com.aspose.cells/themecolor) |  |

### setBorder(int borderType, int borderStyle, CellsColor borderColor) {#setBorder-int-int-com.aspose.cells.CellsColor-}
```
public boolean setBorder(int borderType, int borderStyle, CellsColor borderColor)
```


Ställer in stilens kanter.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| borderType | int | [BorderType](../../com.aspose.cells/bordertype). Den/det/de kant(er) som ska sättas, kan vara en kombination av [BorderType](../../com.aspose.cells/bordertype). |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). Stilen på kanten. |
| borderColor | [CellsColor](../../com.aspose.cells/cellscolor) | Färgen på kanten. |

**Returns:**
boolean - Om de aktuella kantinställningarna har ändrats.
### setBorder(int borderType, int borderStyle, Color borderColor) {#setBorder-int-int-com.aspose.cells.Color-}
```
public boolean setBorder(int borderType, int borderStyle, Color borderColor)
```


Ställer in stilens kanter.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| borderType | int | [BorderType](../../com.aspose.cells/bordertype). Den/det/de kant(er) som ska sättas, kan vara en kombination av [BorderType](../../com.aspose.cells/bordertype). |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). Stilen på kanten. |
| borderColor | [Color](../../com.aspose.cells/color) | Färgen på kanten. |

**Returns:**
boolean - Om de aktuella kantinställningarna har ändrats.
### setBorderApplied(boolean value) {#setBorderApplied-boolean-}
```
public void setBorderApplied(boolean value)
```


Anger om kantformatering ska tillämpas.

**Remarks**

Endast för namngiven stil.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setCheckBox(boolean value) {#setCheckBox-boolean-}
```
public void setCheckBox(boolean value)
```


Anger om det är en stil för kryssruta

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setCultureCustom(String value) {#setCultureCustom-java.lang.String-}
```
public void setCultureCustom(String value)
```


Ställer in det kulturberoende mönstersträngen för talformat. Om inget talformat har satts för detta objekt returneras null. Om talformatet är inbyggt returneras mönstersträngen som motsvarar det inbyggda talet.

**Remarks**

För inbyggt talformat är både mönsterinnehållet (t.ex. ett inbyggt datumformat är "m/d/y" för vissa språkversioner, men för andra blir det "d/m/y") och formatavgränsaren (t.ex. vissa språkversioner använder ett annat tecken än 'y' för att representera årsdelen i datumformat) kulturberoende; för ett användarspecificerat anpassat format ändras endast formatavgränsarna enligt kulturen, övriga delar av formateringsmönstret modifieras inte.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setCustom(String value) {#setCustom-java.lang.String-}
```
public void setCustom(String value)
```


Representerar den anpassade talformatsträngen för detta stilobjekt. Om det anpassade talformatet inte är angivet (t.ex. talformatet är inbyggt) returneras "".

**Remarks**

Den returnerade anpassade strängen är kulturoberoende.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setCustom(String custom, boolean builtinPreference) {#setCustom-java.lang.String-boolean-}
```
public void setCustom(String custom, boolean builtinPreference)
```


Ställer in den anpassade talformatsträngen för en cell.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| anpassad | java.lang.String | Anpassad talformatsträng, bör vara ett InvariantCulture-mönster. |
| builtinPreference | boolean | Om den angivna anpassade talformatsträngen matchar ett av de inbyggda talformaten som motsvarar de aktuella regionala inställningarna, huruvida talformatet ska sättas som inbyggt istället för anpassat. |

### setFillApplied(boolean value) {#setFillApplied-boolean-}
```
public void setFillApplied(boolean value)
```


Anger om fyllnadsformatering ska tillämpas.

**Remarks**

Endast för namngiven stil.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setFontApplied(boolean value) {#setFontApplied-boolean-}
```
public void setFontApplied(boolean value)
```


Anger om teckensnittsformatering ska tillämpas.

**Remarks**

Endast för namngiven stil.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setForegroundArgbColor(int value) {#setForegroundArgbColor-int-}
```
public void setForegroundArgbColor(int value)
```


Ställer in förgrundsfärgen med ett 32-bitars ARGB‑värde.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setForegroundColor(Color value) {#setForegroundColor-com.aspose.cells.Color-}
```
public void setForegroundColor(Color value)
```


Ställer in en stils förgrundsfärg.

**Remarks**

Det betyder ingen färginställning om Color.Empty returneras.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setForegroundThemeColor(ThemeColor value) {#setForegroundThemeColor-com.aspose.cells.ThemeColor-}
```
public void setForegroundThemeColor(ThemeColor value)
```


Ställer in förgrundens temafärg.

**Remarks**

Om förgrundsfärgen inte är en temafärg returneras NULL.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [ThemeColor](../../com.aspose.cells/themecolor) |  |

### setFormulaHidden(boolean value) {#setFormulaHidden-boolean-}
```
public void setFormulaHidden(boolean value)
```


Representerar om formeln kommer att döljas när kalkylbladet är skyddat.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setGradient(boolean value) {#setGradient-boolean-}
```
public void setGradient(boolean value)
```


Anger om cellskuggning är ett gradientmönster.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setHorizontalAlignment(int value) {#setHorizontalAlignment-int-}
```
public void setHorizontalAlignment(int value)
```


Ställer in den horisontella justeringstypen för texten i en cell.

Se [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setIndentLevel(int value) {#setIndentLevel-int-}
```
public void setIndentLevel(int value)
```


Representerar indenteringsnivån för cellen eller området. Kan endast vara ett heltal mellan 0 och 250.

**Remarks**

Om horisontell justeringstyp för text är inställd på ett värde annat än vänster eller höger återställs indenteringsnivån till noll.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setJustifyDistributed(boolean value) {#setJustifyDistributed-boolean-}
```
public void setJustifyDistributed(boolean value)
```


Anger om cellerna ska ha justerad eller fördelad justering på den sista textraden.

**Remarks**

Detta är typiskt för östasiatiska justeringar men inte i andra sammanhang. Fungerar endast när horisontell justering är fördelad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


Ställer in ett värde som indikerar om en cell kan modifieras eller inte.

**Remarks**

Låsning av celler har ingen effekt om inte kalkylbladet är skyddat.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Ställer in stilens namn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setNumber(int value) {#setNumber-int-}
```
public void setNumber(int value)
```


Ställer in visningsformatet för tal och datum. Formateringsmönstren skiljer sig åt mellan olika regioner.

**Remarks**

Till exempel, formateringsmönstren som representeras av siffror för regionen en\_US:

| Värde | Typ | Formateringssträng |
| ----- | ---------- | ---------------------------------------------------- |
| 0 | General | `General` |
| 1 | Decimal | `0` |
| 2 | Decimal | `0.00` |
| 3 | Decimal | `#,##0` |
| 4 | Decimal | `#,##0.00` |
| 5 | Currency | `$#,##0_);($#,##0)` |
| 6 | Currency | `$#,##0_);[Red](../$#,##0)` |
| 7 | Currency | `$#,##0.00_);($#,##0.00)` |
| 8 | Currency | `$#,##0.00_);[Red](../$#,##0.00)` |
| 9 | Percentage | `0%` |
| 10 | Percentage | `0.00%` |
| 11 | Scientific | `0.00E+00` |
| 12 | Fraction | `# ?/?` |
| 13 | Fraction | `# ??/??` |
| 14 | Date | `m/d/yyyy` |
| 15 | Date | `d-mmm-yy` |
| 16 | Date | `d-mmm` |
| 17 | Date | `mmm-yy` |
| 18 | Time | `h:mm FM/EM` |
| 19 | Time | `h:mm:ss FM/EM` |
| 20 | Time | `h:mm` |
| 21 | Time | `h:mm:ss` |
| 22 | Time | `m/d/yyyy h:mm` |
| 37 | Accounting | `#,##0_);(#,##0)` |
| 38 | Accounting | `#,##0_);[Röd](../#,##0)` |
| 39 | Accounting | `#,##0.00_);(#,##0.00)` |
| 40 | Accounting | `#,##0.00_);[Röd](../#,##0.00)` |
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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setNumberFormatApplied(boolean value) {#setNumberFormatApplied-boolean-}
```
public void setNumberFormatApplied(boolean value)
```


Anger om talformatering ska tillämpas.

**Remarks**

Endast för namngiven stil.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setOutlineBorders(int borderStyle, CellsColor borderColor) {#setOutlineBorders-int-com.aspose.cells.CellsColor-}
```
public void setOutlineBorders(int borderStyle, CellsColor borderColor)
```


Ställ in konturkanterna

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). Typen av kanter. |
| borderColor | [CellsColor](../../com.aspose.cells/cellscolor) | Färgen på kanterna |

### setOutlineBorders(int borderStyle, Color borderColor) {#setOutlineBorders-int-com.aspose.cells.Color-}
```
public void setOutlineBorders(int borderStyle, Color borderColor)
```


Ställ in konturkanterna

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). Typen av kanter. |
| borderColor | [Color](../../com.aspose.cells/color) | Färgen på kanterna |

### setPattern(int value) {#setPattern-int-}
```
public void setPattern(int value)
```


Ställer in cellens bakgrundsmönstertyp.

Se [BackgroundType](../../com.aspose.cells/backgroundtype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setPatternColor(int pattern, Color color1, Color color2) {#setPatternColor-int-com.aspose.cells.Color-com.aspose.cells.Color-}
```
public void setPatternColor(int pattern, Color color1, Color color2)
```


Ställer in bakgrundsfärgen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pattern | int | [BackgroundType](../../com.aspose.cells/backgroundtype). Mönstret. |
| color1 | [Color](../../com.aspose.cells/color) | Förgrundsfärgen. |
| color2 | [Color](../../com.aspose.cells/color) | Bakgrundsfärgen. Fungerar endast när mönstret inte är BackgroundType.None och BackgroundType.Solid. |

### setProtectionApplied(boolean value) {#setProtectionApplied-boolean-}
```
public void setProtectionApplied(boolean value)
```


Anger om skyddsformatering ska tillämpas.

**Remarks**

Endast för namngiven stil.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setQuotePrefix(boolean value) {#setQuotePrefix-boolean-}
```
public void setQuotePrefix(boolean value)
```


Anger om cellens värde börjar med ett enkelt citattecken.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setRotationAngle(int value) {#setRotationAngle-int-}
```
public void setRotationAngle(int value)
```


Representerar textrotationsvinkeln.

**Remarks**

0: Inte roterad.

255: Från topp till botten.

\-90: Nedåt.

90: Uppåt.

Du kan ange 255 eller ett värde mellan -90 och 90.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setShrinkToFit(boolean value) {#setShrinkToFit-boolean-}
```
public void setShrinkToFit(boolean value)
```


Representerar om text automatiskt krymper för att passa i den tillgängliga kolumnbredden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setTextDirection(int value) {#setTextDirection-int-}
```
public void setTextDirection(int value)
```


Representerar textens läsriktning.

Se [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setTextWrapped(boolean value) {#setTextWrapped-boolean-}
```
public void setTextWrapped(boolean value)
```


Ställer in ett värde som indikerar om texten i en cell är radbruten.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setTwoColorGradient(Color color1, Color color2, int gradientStyleType, int variant) {#setTwoColorGradient-com.aspose.cells.Color-com.aspose.cells.Color-int-int-}
```
public void setTwoColorGradient(Color color1, Color color2, int gradientStyleType, int variant)
```


Ställer in den angivna fyllningen till en tvåfärgsgradient.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| color1 | [Color](../../com.aspose.cells/color) | En gradientfärg. |
| color2 | [Color](../../com.aspose.cells/color) | Två gradientfärger. |
| gradientStyleType | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). Gradientskuggningsstil. |
| variant | int | Gradientvarianten. Kan vara ett värde från 1 till 4, vilket motsvarar en av de fyra varianterna på fliken Gradient i dialogrutan Fill Effects. Om stilen är GradientStyle.FromCenter, kan Variant-argumentet endast vara 1 eller 2. |

### setVerticalAlignment(int value) {#setVerticalAlignment-int-}
```
public void setVerticalAlignment(int value)
```


Ställer in den vertikala justeringstypen för texten i en cell.

Se [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### toJson() {#toJson--}
```
public String toJson()
```


Konvertera [Style](../../com.aspose.cells/style) till JSON‑strukturdatan.

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


Applicera den namngivna stilen på cellernas stilar som använder denna namngivna stil. Det fungerar som att klicka på \"ok\"-knappen efter att du har avslutat modifieringen av stilen. Gäller endast för namngiven stil.

### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

