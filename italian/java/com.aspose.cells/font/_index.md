---
title: "Font"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Incapsula l'oggetto font utilizzato in un foglio di calcolo."
type: docs
url: /it/java/com.aspose.cells/font/
---

**Inheritance:**
java.lang.Object
```
public class Font
```

Incapsula l'oggetto font utilizzato in un foglio di calcolo.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //Obtaining the reference of the newly added worksheet by passing its sheet index
         Worksheet worksheet = workbook.getWorksheets().get(0);
 
         //Accessing the "A1" cell from the worksheet
         Cell cell = worksheet.getCells().get("A1");
 
         //Adding some value to the "A1" cell
         cell.putValue("Hello Aspose!");
 
         Font font = cell.getStyle().getFont();
 
         //Setting the font name to "Times New Roman"
         font.setName("Times New Roman");
 
         //Setting font size to 14
         font.setSize(14);
 
         //setting font color as Red
         font.setColor(com.aspose.cells.Color.getRed());           
 
         //Saving the Excel file
         workbook.save("dest.xls");
```
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Font font)](#equals-com.aspose.cells.Font-) | Verifica se due font sono uguali. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArgbColor()](#getArgbColor--) | Restituisce il colore con un valore ARGB a 32 bit. |
| [getCapsType()](#getCapsType--) | Ottiene il tipo di maiuscole del testo. |
| [getCharset()](#getCharset--) | Rappresenta il set di caratteri. |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | Ottiene il [Color](../../com.aspose.cells/color) del font. |
| [getDoubleSize()](#getDoubleSize--) | Ottiene la dimensione doppia del font. |
| [getName()](#getName--) | Ottiene il nome del [Font](../../com.aspose.cells/font). |
| [getSchemeType()](#getSchemeType--) | Restituisce il tipo di schema del carattere. |
| [getScriptOffset()](#getScriptOffset--) | Restituisce lo spostamento dello script,in unità di percentuale |
| [getSize()](#getSize--) | Restituisce la dimensione del carattere. |
| [getStrikeType()](#getStrikeType--) | Restituisce il tipo di barrato del testo. |
| [getThemeColor()](#getThemeColor--) | Ottiene il colore del tema. |
| [getUnderline()](#getUnderline--) | Restituisce il tipo di sottolineatura del carattere. |
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
| [setCapsType(int value)](#setCapsType-int-) | Imposta il tipo di maiuscole del testo. |
| [setCharset(int value)](#setCharset-int-) | Rappresenta il set di caratteri. |
| [setColor(Color value)](#setColor-com.aspose.cells.Color-) | Imposta il [Color](../../com.aspose.cells/color) del carattere. |
| [setDoubleSize(double value)](#setDoubleSize-double-) | Imposta la dimensione doppia del carattere. |
| [setItalic(boolean value)](#setItalic-boolean-) | Imposta un valore che indica se il carattere è in corsivo. |
| [setName(String value)](#setName-java.lang.String-) | Imposta il nome del [Font](../../com.aspose.cells/font). |
| [setName(String name, int type)](#setName-java.lang.String-int-) | Imposta il nome e lo schema del carattere. |
| [setNormalizeHeights(boolean value)](#setNormalizeHeights-boolean-) | Indica se la normalizzazione dell'altezza deve essere applicata al blocco di testo. |
| [setSchemeType(int value)](#setSchemeType-int-) | Imposta il tipo di schema del carattere. |
| [setScriptOffset(double value)](#setScriptOffset-double-) | Imposta lo spostamento dello script,in unità di percentuale |
| [setSize(int value)](#setSize-int-) | Imposta la dimensione del carattere. |
| [setStrikeType(int value)](#setStrikeType-int-) | Restituisce il tipo di barrato del testo. |
| [setStrikeout(boolean value)](#setStrikeout-boolean-) | Imposta un valore che indica se il carattere è barrato singolo. |
| [setSubscript(boolean value)](#setSubscript-boolean-) | Imposta un valore che indica se il carattere è in pedice. |
| [setSuperscript(boolean value)](#setSuperscript-boolean-) | Imposta un valore che indica se il carattere è in apice. |
| [setThemeColor(ThemeColor value)](#setThemeColor-com.aspose.cells.ThemeColor-) | Imposta il colore del tema. |
| [setUnderline(int value)](#setUnderline-int-) | Imposta il tipo di sottolineatura del carattere. |
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


Ottiene il tipo di maiuscole del testo.

Vedi [TextCapsType](../../com.aspose.cells/textcapstype).

**Remarks**

Solo per i font di forme o grafici. NOTA: Questo membro è ora obsoleto. Invece, utilizzare la proprietà [TextOptions.getCapsType()](../../com.aspose.cells/textoptions\#getCapsType--). Questa proprietà sarà rimossa 12 mesi dopo, a partire da gennaio 2026. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

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
### getName() {#getName--}
```
public String getName()
```


Ottiene il nome del [Font](../../com.aspose.cells/font).

**Remarks**

Se questa proprietà viene usata per impostare il nome del font, il [getSchemeType()](../../com.aspose.cells/font\#getSchemeType--) verrà aggiornato a [FontSchemeType.NONE](../../com.aspose.cells/fontschemetype\#NONE).

**Returns:**
java.lang.String
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
### getSize() {#getSize--}
```
public int getSize()
```


Restituisce la dimensione del carattere.

**Returns:**
int
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

Solo per i font di forme o grafici. NOTA: Questo membro è ora obsoleto. Invece, utilizzare la proprietà [TextOptions.isNormalizeHeights()](../../com.aspose.cells/textoptions\#isNormalizeHeights--). Questa proprietà sarà rimossa 12 mesi dopo, a partire da gennaio 2026. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

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


Imposta il tipo di maiuscole del testo.

Vedi [TextCapsType](../../com.aspose.cells/textcapstype).

**Remarks**

Solo per i font di forme o grafici. NOTA: Questo membro è ora obsoleto. Invece, utilizzare la proprietà [TextOptions.getCapsType()](../../com.aspose.cells/textoptions\#getCapsType--). Questa proprietà sarà rimossa 12 mesi dopo, a partire da gennaio 2026. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

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

### setItalic(boolean value) {#setItalic-boolean-}
```
public void setItalic(boolean value)
```


Imposta un valore che indica se il carattere è in corsivo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Imposta il nome del [Font](../../com.aspose.cells/font).

**Remarks**

Se questa proprietà viene usata per impostare il nome del font, il [getSchemeType()](../../com.aspose.cells/font\#getSchemeType--) verrà aggiornato a [FontSchemeType.NONE](../../com.aspose.cells/fontschemetype\#NONE).

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

Solo per i font di forme o grafici. NOTA: Questo membro è ora obsoleto. Invece, utilizzare la proprietà [TextOptions.isNormalizeHeights()](../../com.aspose.cells/textoptions\#isNormalizeHeights--). Questa proprietà sarà rimossa 12 mesi dopo, a partire da gennaio 2026. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

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

