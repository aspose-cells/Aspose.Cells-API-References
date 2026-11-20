---
title: "TextOptions"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta le opzioni di testo."
type: docs
url: /it/java/com.aspose.cells/textoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Font](../../com.aspose.cells/font)
```
public class TextOptions extends Font
```

Rappresenta le opzioni di testo.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Font font)](#equals-com.aspose.cells.Font-) | Verifica se due font sono uguali. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArgbColor()](#getArgbColor--) | Restituisce il colore con un valore ARGB a 32 bit. |
| [getCapsType()](#getCapsType--) | Ottiene il tipo di maiuscole per i testi della forma. |
| [getCharset()](#getCharset--) | Rappresenta il set di caratteri. |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | Ottiene il [Color](../../com.aspose.cells/color) del font. |
| [getDoubleSize()](#getDoubleSize--) | Ottiene la dimensione doppia del font. |
| [getFarEastName()](#getFarEastName--) | Ottiene il nome FarEast. |
| [getFill()](#getFill--) | Rappresenta il formato di riempimento del testo. |
| [getKerning()](#getKerning--) | Specifica la dimensione minima del font in cui avverrà il kerning dei caratteri per questo intervallo di testo. |
| [getLanguageCode()](#getLanguageCode--) | Ottiene la lingua dell'interfaccia utente. |
| [getLatinName()](#getLatinName--) | Ottiene il nome latino. |
| [getName()](#getName--) | Ottiene il nome della forma. |
| [getOutline()](#getOutline--) | Rappresenta il formato del contorno del testo. |
| [getSchemeType()](#getSchemeType--) | Restituisce il tipo di schema del carattere. |
| [getScriptOffset()](#getScriptOffset--) | Restituisce lo spostamento dello script,in unità di percentuale |
| [getShadow()](#getShadow--) | Rappresenta un oggetto [ShadowEffect](../../com.aspose.cells/shadoweffect) che specifica l'effetto di ombra per l'elemento del grafico o la forma. |
| [getSize()](#getSize--) | Restituisce la dimensione del carattere. |
| [getSpacing()](#getSpacing--) | Specifica la spaziatura tra i caratteri all'interno di un blocco di testo. |
| [getStrikeType()](#getStrikeType--) | Restituisce il tipo di barrato del testo. |
| [getThemeColor()](#getThemeColor--) | Ottiene il colore del tema. |
| [getUnderline()](#getUnderline--) | Restituisce il tipo di sottolineatura del carattere. |
| [getUnderlineColor()](#getUnderlineColor--) | Restituisce il colore della sottolineatura. |
| [hashCode()](#hashCode--) |  |
| [isBold()](#isBold--) | Restituisce un valore che indica se il carattere è in grassetto. |
| [isItalic()](#isItalic--) | Restituisce un valore che indica se il carattere è in corsivo. |
| [isNormalizeHeights()](#isNormalizeHeights--) | Indica se la normalizzazione dell'altezza deve essere applicata al blocco di testo. |
| [isStrikeout()](#isStrikeout--) | Restituisce un valore che indica se il carattere ha una singola barratura. |
| [isSubscript()](#isSubscript--) | Restituisce un valore che indica se il carattere è pedice. |
| [isSuperscript()](#isSuperscript--) | Restituisce un valore che indica se il carattere è apice. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setArgbColor(int value)](#setArgbColor-int-) | Imposta il colore con un valore ARGB a 32 bit. |
| [setBold(boolean value)](#setBold-boolean-) | Imposta un valore che indica se il carattere è in grassetto. |
| [setCapsType(int value)](#setCapsType-int-) | Imposta il tipo di maiuscole per i testi della forma. |
| [setCharset(int value)](#setCharset-int-) | Rappresenta il set di caratteri. |
| [setColor(Color value)](#setColor-com.aspose.cells.Color-) | Imposta il [Color](../../com.aspose.cells/color) del carattere. |
| [setDoubleSize(double value)](#setDoubleSize-double-) | Imposta la dimensione doppia del carattere. |
| [setFarEastName(String value)](#setFarEastName-java.lang.String-) | Imposta il nome FarEast. |
| [setItalic(boolean value)](#setItalic-boolean-) | Imposta un valore che indica se il carattere è in corsivo. |
| [setKerning(double value)](#setKerning-double-) | Specifica la dimensione minima del font in cui avverrà il kerning dei caratteri per questo intervallo di testo. |
| [setLanguageCode(int value)](#setLanguageCode-int-) | Imposta la lingua dell'interfaccia utente. |
| [setLatinName(String value)](#setLatinName-java.lang.String-) | Imposta il nome latino. |
| [setName(String value)](#setName-java.lang.String-) | Imposta il nome della forma. |
| [setName(String name, int type)](#setName-java.lang.String-int-) | Imposta il nome e lo schema del carattere. |
| [setNormalizeHeights(boolean value)](#setNormalizeHeights-boolean-) | Indica se la normalizzazione dell'altezza deve essere applicata al blocco di testo. |
| [setSchemeType(int value)](#setSchemeType-int-) | Imposta il tipo di schema del carattere. |
| [setScriptOffset(double value)](#setScriptOffset-double-) | Imposta lo spostamento dello script,in unità di percentuale |
| [setSize(int value)](#setSize-int-) | Imposta la dimensione del carattere. |
| [setSpacing(double value)](#setSpacing-double-) | Specifica la spaziatura tra i caratteri all'interno di un blocco di testo. |
| [setStrikeType(int value)](#setStrikeType-int-) | Restituisce il tipo di barrato del testo. |
| [setStrikeout(boolean value)](#setStrikeout-boolean-) | Imposta un valore che indica se il carattere è barrato singolo. |
| [setSubscript(boolean value)](#setSubscript-boolean-) | Imposta un valore che indica se il carattere è in pedice. |
| [setSuperscript(boolean value)](#setSuperscript-boolean-) | Imposta un valore che indica se il carattere è in apice. |
| [setThemeColor(ThemeColor value)](#setThemeColor-com.aspose.cells.ThemeColor-) | Imposta il colore del tema. |
| [setUnderline(int value)](#setUnderline-int-) | Imposta il tipo di sottolineatura del carattere. |
| [setUnderlineColor(CellsColor value)](#setUnderlineColor-com.aspose.cells.CellsColor-) | Imposta il colore della sottolineatura. |
| [toString()](#toString--) | Restituisce una stringa che rappresenta l'oggetto Cell corrente. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Font font) {#equals-com.aspose.cells.Font-}
```
public boolean equals(Font font)
```


Verifica se due font sono uguali.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| font | [Font](../../com.aspose.cells/font) | Oggetto carattere confrontato. |

**Returns:**
boolean - True se uguale all'oggetto carattere confrontato.
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getArgbColor() {#getArgbColor--}
```
public int getArgbColor()
```


Restituisce il colore con un valore ARGB a 32 bit.

**Returns:**
int
### getCapsType() {#getCapsType--}
```
public int getCapsType()
```


Ottiene il tipo di maiuscole per i testi della forma.

Vedi [TextCapsType](../../com.aspose.cells/textcapstype).

**Returns:**
int
### getCharset() {#getCharset--}
```
public int getCharset()
```


Rappresenta il set di caratteri.

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColor() {#getColor--}
```
public Color getColor()
```


Ottiene il [Color](../../com.aspose.cells/color) del font.

**Returns:**
[Color](../../com.aspose.cells/color)
### getDoubleSize() {#getDoubleSize--}
```
public double getDoubleSize()
```


Ottiene la dimensione doppia del font.

**Returns:**
double
### getFarEastName() {#getFarEastName--}
```
public String getFarEastName()
```


Ottiene il nome FarEast.

**Returns:**
java.lang.String
### getFill() {#getFill--}
```
public FillFormat getFill()
```


Rappresenta il formato di riempimento del testo.

**Returns:**
[FillFormat](../../com.aspose.cells/fillformat)
### getKerning() {#getKerning--}
```
public double getKerning()
```


Specifica la dimensione minima del font in cui avverrà il kerning dei caratteri per questo intervallo di testo.

**Returns:**
double
### getLanguageCode() {#getLanguageCode--}
```
public int getLanguageCode()
```


Ottiene la lingua dell'interfaccia utente.

Vedi [CountryCode](../../com.aspose.cells/countrycode).

**Returns:**
int
### getLatinName() {#getLatinName--}
```
public String getLatinName()
```


Ottiene il nome latino.

**Returns:**
java.lang.String
### getName() {#getName--}
```
public String getName()
```


Ottiene il nome della forma.

**Returns:**
java.lang.String
### getOutline() {#getOutline--}
```
public LineFormat getOutline()
```


Rappresenta il formato del contorno del testo.

**Returns:**
[LineFormat](../../com.aspose.cells/lineformat)
### getSchemeType() {#getSchemeType--}
```
public int getSchemeType()
```


Restituisce il tipo di schema del carattere.

Vedi [FontSchemeType](../../com.aspose.cells/fontschemetype).

**Returns:**
int
### getScriptOffset() {#getScriptOffset--}
```
public double getScriptOffset()
```


Restituisce lo spostamento dello script,in unità di percentuale

**Remarks**

Solo per forme e grafici.

**Returns:**
double
### getShadow() {#getShadow--}
```
public ShadowEffect getShadow()
```


Rappresenta un oggetto [ShadowEffect](../../com.aspose.cells/shadoweffect) che specifica l'effetto di ombra per l'elemento del grafico o la forma.

**Returns:**
[ShadowEffect](../../com.aspose.cells/shadoweffect)
### getSize() {#getSize--}
```
public int getSize()
```


Restituisce la dimensione del carattere.

**Returns:**
int
### getSpacing() {#getSpacing--}
```
public double getSpacing()
```


Specifica la spaziatura tra i caratteri all'interno di un blocco di testo.

**Returns:**
double
### getStrikeType() {#getStrikeType--}
```
public int getStrikeType()
```


Restituisce il tipo di barrato del testo.

Vedi [TextStrikeType](../../com.aspose.cells/textstriketype).

**Returns:**
int
### getThemeColor() {#getThemeColor--}
```
public ThemeColor getThemeColor()
```


Ottiene il colore del tema.

**Remarks**

Se il colore del carattere non è un colore del tema, verrà restituito NULL.

**Returns:**
[ThemeColor](../../com.aspose.cells/themecolor)
### getUnderline() {#getUnderline--}
```
public int getUnderline()
```


Restituisce il tipo di sottolineatura del carattere.

Vedi [FontUnderlineType](../../com.aspose.cells/fontunderlinetype).

**Returns:**
int
### getUnderlineColor() {#getUnderlineColor--}
```
public CellsColor getUnderlineColor()
```


Restituisce il colore della sottolineatura.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isBold() {#isBold--}
```
public boolean isBold()
```


Restituisce un valore che indica se il carattere è in grassetto.

**Returns:**
boolean
### isItalic() {#isItalic--}
```
public boolean isItalic()
```


Restituisce un valore che indica se il carattere è in corsivo.

**Returns:**
boolean
### isNormalizeHeights() {#isNormalizeHeights--}
```
public boolean isNormalizeHeights()
```


Indica se la normalizzazione dell'altezza deve essere applicata al blocco di testo.

**Remarks**

Solo per i caratteri di Forme o Grafici.

**Returns:**
boolean
### isStrikeout() {#isStrikeout--}
```
public boolean isStrikeout()
```


Restituisce un valore che indica se il carattere ha una singola barratura.

**Returns:**
boolean
### isSubscript() {#isSubscript--}
```
public boolean isSubscript()
```


Restituisce un valore che indica se il carattere è pedice.

**Returns:**
boolean
### isSuperscript() {#isSuperscript--}
```
public boolean isSuperscript()
```


Restituisce un valore che indica se il carattere è apice.

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




### setArgbColor(int value) {#setArgbColor-int-}
```
public void setArgbColor(int value)
```


Imposta il colore con un valore ARGB a 32 bit.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setBold(boolean value) {#setBold-boolean-}
```
public void setBold(boolean value)
```


Imposta un valore che indica se il carattere è in grassetto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setCapsType(int value) {#setCapsType-int-}
```
public void setCapsType(int value)
```


Imposta il tipo di maiuscole per i testi della forma.

Vedi [TextCapsType](../../com.aspose.cells/textcapstype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setCharset(int value) {#setCharset-int-}
```
public void setCharset(int value)
```


Rappresenta il set di caratteri.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setColor(Color value) {#setColor-com.aspose.cells.Color-}
```
public void setColor(Color value)
```


Imposta il [Color](../../com.aspose.cells/color) del carattere.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setDoubleSize(double value) {#setDoubleSize-double-}
```
public void setDoubleSize(double value)
```


Imposta la dimensione doppia del carattere.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setFarEastName(String value) {#setFarEastName-java.lang.String-}
```
public void setFarEastName(String value)
```


Imposta il nome FarEast.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setItalic(boolean value) {#setItalic-boolean-}
```
public void setItalic(boolean value)
```


Imposta un valore che indica se il carattere è in corsivo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setKerning(double value) {#setKerning-double-}
```
public void setKerning(double value)
```


Specifica la dimensione minima del font in cui avverrà il kerning dei caratteri per questo intervallo di testo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setLanguageCode(int value) {#setLanguageCode-int-}
```
public void setLanguageCode(int value)
```


Imposta la lingua dell'interfaccia utente.

Vedi [CountryCode](../../com.aspose.cells/countrycode).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setLatinName(String value) {#setLatinName-java.lang.String-}
```
public void setLatinName(String value)
```


Imposta il nome latino.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Imposta il nome della forma.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setName(String name, int type) {#setName-java.lang.String-int-}
```
public void setName(String name, int type)
```


Imposta il nome e lo schema del carattere.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | java.lang.String |  |
| type | int | [FontSchemeType](../../com.aspose.cells/fontschemetype). |

### setNormalizeHeights(boolean value) {#setNormalizeHeights-boolean-}
```
public void setNormalizeHeights(boolean value)
```


Indica se la normalizzazione dell'altezza deve essere applicata al blocco di testo.

**Remarks**

Solo per i caratteri di Forme o Grafici.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setSchemeType(int value) {#setSchemeType-int-}
```
public void setSchemeType(int value)
```


Imposta il tipo di schema del carattere.

Vedi [FontSchemeType](../../com.aspose.cells/fontschemetype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setScriptOffset(double value) {#setScriptOffset-double-}
```
public void setScriptOffset(double value)
```


Imposta lo spostamento dello script,in unità di percentuale

**Remarks**

Solo per forme e grafici.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setSize(int value) {#setSize-int-}
```
public void setSize(int value)
```


Imposta la dimensione del carattere.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setSpacing(double value) {#setSpacing-double-}
```
public void setSpacing(double value)
```


Specifica la spaziatura tra i caratteri all'interno di un blocco di testo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setStrikeType(int value) {#setStrikeType-int-}
```
public void setStrikeType(int value)
```


Restituisce il tipo di barrato del testo.

Vedi [TextStrikeType](../../com.aspose.cells/textstriketype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setStrikeout(boolean value) {#setStrikeout-boolean-}
```
public void setStrikeout(boolean value)
```


Imposta un valore che indica se il carattere è barrato singolo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setSubscript(boolean value) {#setSubscript-boolean-}
```
public void setSubscript(boolean value)
```


Imposta un valore che indica se il carattere è in pedice.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setSuperscript(boolean value) {#setSuperscript-boolean-}
```
public void setSuperscript(boolean value)
```


Imposta un valore che indica se il carattere è in apice.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setThemeColor(ThemeColor value) {#setThemeColor-com.aspose.cells.ThemeColor-}
```
public void setThemeColor(ThemeColor value)
```


Imposta il colore del tema.

**Remarks**

Se il colore del carattere non è un colore del tema, verrà restituito NULL.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [ThemeColor](../../com.aspose.cells/themecolor) |  |

### setUnderline(int value) {#setUnderline-int-}
```
public void setUnderline(int value)
```


Imposta il tipo di sottolineatura del carattere.

Vedi [FontUnderlineType](../../com.aspose.cells/fontunderlinetype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setUnderlineColor(CellsColor value) {#setUnderlineColor-com.aspose.cells.CellsColor-}
```
public void setUnderlineColor(CellsColor value)
```


Imposta il colore della sottolineatura.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

### toString() {#toString--}
```
public String toString()
```


Restituisce una stringa che rappresenta l'oggetto Cell corrente.

**Returns:**
java.lang.String -
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

