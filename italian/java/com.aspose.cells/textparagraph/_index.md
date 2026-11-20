---
title: "TextParagraph"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta l'impostazione del paragrafo di testo."
type: docs
url: /it/java/com.aspose.cells/textparagraph/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.FontSetting](../../com.aspose.cells/fontsetting)
```
public class TextParagraph extends FontSetting
```

Rappresenta l'impostazione del paragrafo di testo.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAlignmentType()](#getAlignmentType--) | Ottiene il tipo di allineamento orizzontale del testo del paragrafo. |
| [getBullet()](#getBullet--) | Ottiene il punto elenco. |
| [getChildren()](#getChildren--) | Ottiene tutte le sequenze di testo in questo paragrafo. |
| [getClass()](#getClass--) |  |
| [getDefaultTabSize()](#getDefaultTabSize--) | Ottiene la dimensione predefinita per un carattere di tabulazione all'interno di questo paragrafo. |
| [getFirstLineIndent()](#getFirstLineIndent--) | Specifica la dimensione dell'indentazione che verrà applicata alla prima riga di testo del paragrafo. |
| [getFont()](#getFont--) | Restituisce il carattere di questo oggetto. |
| [getFontAlignType()](#getFontAlignType--) | Determina dove verticalmente su una riga di testo le parole effettive sono posizionate. |
| [getLeftMargin()](#getLeftMargin--) | Specifica il margine sinistro del paragrafo. |
| [getLength()](#getLength--) | Ottiene la lunghezza dei caratteri. |
| [getLineSpace()](#getLineSpace--) | Ottiene la quantità di spazio bianco verticale che verrà utilizzato all'interno di un paragrafo. |
| [getLineSpaceSizeType()](#getLineSpaceSizeType--) | Ottiene la quantità di spazio bianco verticale che verrà utilizzato all'interno di un paragrafo. |
| [getRightMargin()](#getRightMargin--) | Specifica il margine destro del paragrafo. |
| [getSpaceAfter()](#getSpaceAfter--) | Ottiene la quantità di spazio bianco verticale che sarà presente dopo un paragrafo. |
| [getSpaceAfterSizeType()](#getSpaceAfterSizeType--) | Ottiene la quantità di spazio bianco verticale che sarà presente dopo un paragrafo. |
| [getSpaceBefore()](#getSpaceBefore--) | Ottiene la quantità di spazio bianco verticale che sarà presente prima di un paragrafo. |
| [getSpaceBeforeSizeType()](#getSpaceBeforeSizeType--) | Ottiene la quantità di spazio bianco verticale che sarà presente prima di un paragrafo. |
| [getStartIndex()](#getStartIndex--) | Ottiene l'indice di inizio dei caratteri. |
| [getStops()](#getStops--) | Ottiene l'elenco delle tabulazioni. |
| [getTextOptions()](#getTextOptions--) | Restituisce le opzioni di testo. |
| [getType()](#getType--) | Ottiene il tipo di nodo di testo. |
| [hashCode()](#hashCode--) |  |
| [isEastAsianLineBreak()](#isEastAsianLineBreak--) | Specifica se una parola dell'Est asiatico può essere divisa a metà e riportata alla riga successiva senza aggiungere un trattino. |
| [isHangingPunctuation()](#isHangingPunctuation--) | Specifica se la punteggiatura deve essere forzatamente posizionata su una riga di testo o spostata su una riga diversa. |
| [isLatinLineBreak()](#isLatinLineBreak--) | Specifica se una parola latina può essere divisa a metà e riportata alla riga successiva senza aggiungere un trattino. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAlignmentType(int value)](#setAlignmentType-int-) | Imposta il tipo di allineamento orizzontale del testo del paragrafo. |
| [setDefaultTabSize(double value)](#setDefaultTabSize-double-) | Imposta la dimensione predefinita per un carattere di tabulazione all'interno di questo paragrafo. |
| [setEastAsianLineBreak(boolean value)](#setEastAsianLineBreak-boolean-) | Specifica se una parola dell'Est asiatico può essere divisa a metà e riportata alla riga successiva senza aggiungere un trattino. |
| [setFirstLineIndent(double value)](#setFirstLineIndent-double-) | Specifica la dimensione dell'indentazione che verrà applicata alla prima riga di testo del paragrafo. |
| [setFontAlignType(int value)](#setFontAlignType-int-) | Determina dove verticalmente su una riga di testo le parole effettive sono posizionate. |
| [setHangingPunctuation(boolean value)](#setHangingPunctuation-boolean-) | Specifica se la punteggiatura deve essere forzatamente posizionata su una riga di testo o spostata su una riga diversa. |
| [setLatinLineBreak(boolean value)](#setLatinLineBreak-boolean-) | Specifica se una parola latina può essere divisa a metà e riportata alla riga successiva senza aggiungere un trattino. |
| [setLeftMargin(double value)](#setLeftMargin-double-) | Specifica il margine sinistro del paragrafo. |
| [setLineSpace(double value)](#setLineSpace-double-) | Imposta la quantità di spazio bianco verticale che verrà utilizzato all'interno di un paragrafo. |
| [setLineSpaceSizeType(int value)](#setLineSpaceSizeType-int-) | Imposta la quantità di spazio bianco verticale che verrà utilizzato all'interno di un paragrafo. |
| [setRightMargin(double value)](#setRightMargin-double-) | Specifica il margine destro del paragrafo. |
| [setSpaceAfter(double value)](#setSpaceAfter-double-) | Imposta la quantità di spazio bianco verticale che sarà presente dopo un paragrafo. |
| [setSpaceAfterSizeType(int value)](#setSpaceAfterSizeType-int-) | Imposta la quantità di spazio bianco verticale che sarà presente dopo un paragrafo. |
| [setSpaceBefore(double value)](#setSpaceBefore-double-) | Imposta la quantità di spazio bianco verticale che sarà presente prima di un paragrafo. |
| [setSpaceBeforeSizeType(int value)](#setSpaceBeforeSizeType-int-) | Imposta la quantità di spazio bianco verticale che sarà presente prima di un paragrafo. |
| [setWordArtStyle(int style)](#setWordArtStyle-int-) | Imposta lo stile WordArt predefinito. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getAlignmentType() {#getAlignmentType--}
```
public int getAlignmentType()
```


Ottiene il tipo di allineamento orizzontale del testo del paragrafo.

Vedi [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Returns:**
int
### getBullet() {#getBullet--}
```
public Bullet getBullet()
```


Ottiene il punto elenco.

**Returns:**
[Bullet](../../com.aspose.cells/bullet)
### getChildren() {#getChildren--}
```
public FontSetting[] getChildren()
```


Ottiene tutte le sequenze di testo in questo paragrafo. Se questo paragrafo è vuoto, restituisce lo stesso paragrafo.

**Returns:**
com.aspose.cells.FontSetting[]
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDefaultTabSize() {#getDefaultTabSize--}
```
public double getDefaultTabSize()
```


Ottiene la dimensione predefinita per un carattere di tabulazione all'interno di questo paragrafo.

**Returns:**
double
### getFirstLineIndent() {#getFirstLineIndent--}
```
public double getFirstLineIndent()
```


Specifica la dimensione dell'indentazione che verrà applicata alla prima riga di testo del paragrafo.

**Returns:**
double
### getFont() {#getFont--}
```
public Font getFont()
```


Restituisce il carattere di questo oggetto.

**Returns:**
[Font](../../com.aspose.cells/font)
### getFontAlignType() {#getFontAlignType--}
```
public int getFontAlignType()
```


Determina dove verticalmente su una riga di testo le parole effettive sono posizionate. Questo riguarda il posizionamento verticale dei caratteri rispetto alle linee di base.

Vedi [TextFontAlignType](../../com.aspose.cells/textfontaligntype).

**Returns:**
int
### getLeftMargin() {#getLeftMargin--}
```
public double getLeftMargin()
```


Specifica il margine sinistro del paragrafo.

**Returns:**
double
### getLength() {#getLength--}
```
public int getLength()
```


Ottiene la lunghezza dei caratteri.

**Returns:**
int
### getLineSpace() {#getLineSpace--}
```
public double getLineSpace()
```


Ottiene la quantità di spazio bianco verticale che verrà utilizzato all'interno di un paragrafo.

**Returns:**
double
### getLineSpaceSizeType() {#getLineSpaceSizeType--}
```
public int getLineSpaceSizeType()
```


Ottiene la quantità di spazio bianco verticale che verrà utilizzato all'interno di un paragrafo.

Vedi [LineSpaceSizeType](../../com.aspose.cells/linespacesizetype).

**Returns:**
int
### getRightMargin() {#getRightMargin--}
```
public double getRightMargin()
```


Specifica il margine destro del paragrafo.

**Returns:**
double
### getSpaceAfter() {#getSpaceAfter--}
```
public double getSpaceAfter()
```


Ottiene la quantità di spazio bianco verticale che sarà presente dopo un paragrafo.

**Returns:**
double
### getSpaceAfterSizeType() {#getSpaceAfterSizeType--}
```
public int getSpaceAfterSizeType()
```


Ottiene la quantità di spazio bianco verticale che sarà presente dopo un paragrafo.

Vedi [LineSpaceSizeType](../../com.aspose.cells/linespacesizetype).

**Returns:**
int
### getSpaceBefore() {#getSpaceBefore--}
```
public double getSpaceBefore()
```


Ottiene la quantità di spazio bianco verticale che sarà presente prima di un paragrafo.

**Returns:**
double
### getSpaceBeforeSizeType() {#getSpaceBeforeSizeType--}
```
public int getSpaceBeforeSizeType()
```


Ottiene la quantità di spazio bianco verticale che sarà presente prima di un paragrafo.

Vedi [LineSpaceSizeType](../../com.aspose.cells/linespacesizetype).

**Returns:**
int
### getStartIndex() {#getStartIndex--}
```
public int getStartIndex()
```


Ottiene l'indice di inizio dei caratteri.

**Returns:**
int
### getStops() {#getStops--}
```
public TextTabStopCollection getStops()
```


Ottiene l'elenco delle tabulazioni.

**Returns:**
[TextTabStopCollection](../../com.aspose.cells/texttabstopcollection)
### getTextOptions() {#getTextOptions--}
```
public TextOptions getTextOptions()
```


Restituisce le opzioni di testo.

**Returns:**
[TextOptions](../../com.aspose.cells/textoptions)
### getType() {#getType--}
```
public int getType()
```


Ottiene il tipo di nodo di testo.

Vedi [TextNodeType](../../com.aspose.cells/textnodetype).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isEastAsianLineBreak() {#isEastAsianLineBreak--}
```
public boolean isEastAsianLineBreak()
```


Specifica se una parola dell'Est asiatico può essere divisa a metà e riportata alla riga successiva senza aggiungere un trattino.

**Returns:**
boolean
### isHangingPunctuation() {#isHangingPunctuation--}
```
public boolean isHangingPunctuation()
```


Specifica se la punteggiatura deve essere forzatamente posizionata su una riga di testo o spostata su una riga diversa.

**Returns:**
boolean
### isLatinLineBreak() {#isLatinLineBreak--}
```
public boolean isLatinLineBreak()
```


Specifica se una parola latina può essere divisa a metà e riportata alla riga successiva senza aggiungere un trattino.

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




### setAlignmentType(int value) {#setAlignmentType-int-}
```
public void setAlignmentType(int value)
```


Imposta il tipo di allineamento orizzontale del testo del paragrafo.

Vedi [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setDefaultTabSize(double value) {#setDefaultTabSize-double-}
```
public void setDefaultTabSize(double value)
```


Imposta la dimensione predefinita per un carattere di tabulazione all'interno di questo paragrafo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setEastAsianLineBreak(boolean value) {#setEastAsianLineBreak-boolean-}
```
public void setEastAsianLineBreak(boolean value)
```


Specifica se una parola dell'Est asiatico può essere divisa a metà e riportata alla riga successiva senza aggiungere un trattino.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setFirstLineIndent(double value) {#setFirstLineIndent-double-}
```
public void setFirstLineIndent(double value)
```


Specifica la dimensione dell'indentazione che verrà applicata alla prima riga di testo del paragrafo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setFontAlignType(int value) {#setFontAlignType-int-}
```
public void setFontAlignType(int value)
```


Determina dove verticalmente su una riga di testo le parole effettive sono posizionate. Questo riguarda il posizionamento verticale dei caratteri rispetto alle linee di base.

Vedi [TextFontAlignType](../../com.aspose.cells/textfontaligntype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setHangingPunctuation(boolean value) {#setHangingPunctuation-boolean-}
```
public void setHangingPunctuation(boolean value)
```


Specifica se la punteggiatura deve essere forzatamente posizionata su una riga di testo o spostata su una riga diversa.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setLatinLineBreak(boolean value) {#setLatinLineBreak-boolean-}
```
public void setLatinLineBreak(boolean value)
```


Specifica se una parola latina può essere divisa a metà e riportata alla riga successiva senza aggiungere un trattino.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setLeftMargin(double value) {#setLeftMargin-double-}
```
public void setLeftMargin(double value)
```


Specifica il margine sinistro del paragrafo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setLineSpace(double value) {#setLineSpace-double-}
```
public void setLineSpace(double value)
```


Imposta la quantità di spazio bianco verticale che verrà utilizzato all'interno di un paragrafo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setLineSpaceSizeType(int value) {#setLineSpaceSizeType-int-}
```
public void setLineSpaceSizeType(int value)
```


Imposta la quantità di spazio bianco verticale che verrà utilizzato all'interno di un paragrafo.

Vedi [LineSpaceSizeType](../../com.aspose.cells/linespacesizetype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setRightMargin(double value) {#setRightMargin-double-}
```
public void setRightMargin(double value)
```


Specifica il margine destro del paragrafo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setSpaceAfter(double value) {#setSpaceAfter-double-}
```
public void setSpaceAfter(double value)
```


Imposta la quantità di spazio bianco verticale che sarà presente dopo un paragrafo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setSpaceAfterSizeType(int value) {#setSpaceAfterSizeType-int-}
```
public void setSpaceAfterSizeType(int value)
```


Imposta la quantità di spazio bianco verticale che sarà presente dopo un paragrafo.

Vedi [LineSpaceSizeType](../../com.aspose.cells/linespacesizetype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setSpaceBefore(double value) {#setSpaceBefore-double-}
```
public void setSpaceBefore(double value)
```


Imposta la quantità di spazio bianco verticale che sarà presente prima di un paragrafo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setSpaceBeforeSizeType(int value) {#setSpaceBeforeSizeType-int-}
```
public void setSpaceBeforeSizeType(int value)
```


Imposta la quantità di spazio bianco verticale che sarà presente prima di un paragrafo.

Vedi [LineSpaceSizeType](../../com.aspose.cells/linespacesizetype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setWordArtStyle(int style) {#setWordArtStyle-int-}
```
public void setWordArtStyle(int style)
```


Imposta lo stile WordArt predefinito.

**Remarks**

Solo per il testo di forma/grafico.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| style | int | [PresetWordArtStyle](../../com.aspose.cells/presetwordartstyle). Lo stile WordArt predefinito. |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
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

