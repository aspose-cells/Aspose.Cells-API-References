---
title: "GridTableItemStyle"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Ereditato da System.Web.UI.WebControls.TableItemStyle."
type: docs
url: /it/java/com.aspose.gridweb/gridtableitemstyle/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.WebStyle](../../com.aspose.gridweb/webstyle), [com.aspose.gridweb.WebTableItemStyle](../../com.aspose.gridweb/webtableitemstyle)
```
public class GridTableItemStyle extends WebTableItemStyle
```

Ereditato da System.Web.UI.WebControls.TableItemStyle. Incapsula gli stili di una WebCell.

**Example**

```
         GridWeb GridWeb1 = new GridWeb();
         GridWorksheetCollection sheets = GridWeb1.getWorkSheets();
 
         GridWorksheet sheet = sheets.add("demo1");
 
         sheet.getCells().get(0,0).putValue("Demo Text");
         GridTableItemStyle style = sheet.getCells().get(0, 0).getStyle();
 
         style.getFont().setSize(FontUnit.Point(72));
         style.setWrap(false);
 
         style.setBackColor(Color.getGray());
         	style.setBorderStyle(com.aspose.gridweb.BorderStyle.Solid);
         style.setBorderWidth(Unit.Pixel(1));
         style.setBorderColor(Color.getSilver());
         style.getRightBorderStyle().setBorderColor(Color.getBlack());
         	style.getRightBorderStyle().setBorderStyle(com.aspose.gridweb.BorderStyle.Solid);
         	style.getRightBorderStyle().setBorderWidth(Unit.Pixel(1));
         style.getBottomBorderStyle().setBorderColor(Color.getBlack());
         style.getBottomBorderStyle().setBorderStyle(com.aspose.gridweb.BorderStyle.Solid);
         style.getBottomBorderStyle().setBorderWidth(Unit.Pixel(1));
         sheet.getCells().get(0, 0).setStyle(style);
```
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [GridTableItemStyle()](#GridTableItemStyle--) | Costruttore predefinito. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [copyFrom(WebStyle s)](#copyFrom-com.aspose.gridweb.WebStyle-) | Copia da un altro oggetto di stile. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackColor()](#getBackColor--) | Ottiene il BackColor nello stile |
| [getBackImageAttributes()](#getBackImageAttributes--) | Attributi dell'immagine di sfondo. |
| [getBackImageUrl()](#getBackImageUrl--) | URL dell'immagine di sfondo. |
| [getBorderColor()](#getBorderColor--) | Ottiene il BorderColor nello stile |
| [getBorderStyle()](#getBorderStyle--) | Ottiene il BorderStyle nello stile |
| [getBorderWidth()](#getBorderWidth--) | Ottiene il BorderWidth nello stile |
| [getBottomBorderStyle()](#getBottomBorderStyle--) | Specifica lo stile del bordo inferiore della cella. |
| [getClass()](#getClass--) |  |
| [getCssClass()](#getCssClass--) | Ottiene il CssClass nello stile |
| [getCustom()](#getCustom--) | Ottiene il formato personalizzato, null o stringa vuota indica nessun formato personalizzato. |
| [getFont()](#getFont--) | Ottiene il Font nello stile |
| [getForeColor()](#getForeColor--) | Ottiene il ForeColor nello stile |
| [getHeight()](#getHeight--) | Ottiene l'Height nello stile |
| [getHorizontalAlign()](#getHorizontalAlign--) | Ottiene l'HorizontalAlign nello stile |
| [getIndentLevel()](#getIndentLevel--) | Ottiene il livello di rientro. |
| [getLeftBorderStyle()](#getLeftBorderStyle--) | Specifica lo stile del bordo sinistro della cella. |
| [getNumberType()](#getNumberType--) | Ottiene il formato di visualizzazione di numeri e date. |
| [getQuotePrefix()](#getQuotePrefix--) | Indica se il valore della cella inizia con un apice singolo. |
| [getRightBorderStyle()](#getRightBorderStyle--) | Specifica lo stile del bordo destro della cella. |
| [getRotationAngle()](#getRotationAngle--) | Ottiene l'attributo Rotazione. |
| [getTopBorderStyle()](#getTopBorderStyle--) | Specifica lo stile del bordo superiore della cella. |
| [getVerticalAlign()](#getVerticalAlign--) | Ottiene l'allineamento verticale nello stile |
| [getWidth()](#getWidth--) | Ottiene la Width nello stile |
| [getWrap()](#getWrap--) | Ottiene l'opzione di a capo nello stile |
| [hashCode()](#hashCode--) | Funziona come funzione hash per un tipo specifico, adatta all'uso in algoritmi di hashing e strutture dati come una tabella hash. |
| [isLocked()](#isLocked--) | Ottiene un valore che indica se una cella può essere modificata o meno quando il foglio di lavoro è protetto. |
| [mergeWith(WebStyle s)](#mergeWith-com.aspose.gridweb.WebStyle-) | Unisce con un altro oggetto di stile. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBackColor(Color value)](#setBackColor-com.aspose.gridweb.Color-) | Imposta il BackColor nello stile |
| [setBackImageAttributes(String value)](#setBackImageAttributes-java.lang.String-) | Attributi dell'immagine di sfondo. |
| [setBackImageUrl(String value)](#setBackImageUrl-java.lang.String-) | URL dell'immagine di sfondo. |
| [setBorderColor(Color value)](#setBorderColor-com.aspose.gridweb.Color-) | Imposta il BorderColor nello stile |
| [setBorderStyle(int value)](#setBorderStyle-int-) | Imposta il BorderStyle nello stile |
| [setBorderWidth(Unit value)](#setBorderWidth-com.aspose.gridweb.Unit-) | Imposta il BorderWidth nello stile |
| [setBottomBorderStyle(WebBorderStyle value)](#setBottomBorderStyle-com.aspose.gridweb.WebBorderStyle-) | Specifica lo stile del bordo inferiore della cella. |
| [setCssClass(String value)](#setCssClass-java.lang.String-) | Imposta il CssClass nello stile |
| [setCustom(String value)](#setCustom-java.lang.String-) | Imposta il formato personalizzato, null o stringa vuota indica nessun formato personalizzato. |
| [setForeColor(Color value)](#setForeColor-com.aspose.gridweb.Color-) | Imposta il ForeColor nello stile |
| [setHeight(Unit value)](#setHeight-com.aspose.gridweb.Unit-) | Imposta l'Height nello stile |
| [setHorizontalAlign(int value)](#setHorizontalAlign-int-) | Imposta l'HorizontalAlign nello stile |
| [setIndentLevel(int value)](#setIndentLevel-int-) | Imposta il livello di rientro. |
| [setLeftBorderStyle(WebBorderStyle value)](#setLeftBorderStyle-com.aspose.gridweb.WebBorderStyle-) | Specifica lo stile del bordo sinistro della cella. |
| [setLocked(boolean value)](#setLocked-boolean-) | Imposta un valore che indica se una cella può essere modificata o non quando il foglio di lavoro è protetto. |
| [setNumberType(int value)](#setNumberType-int-) | Imposta il formato di visualizzazione di numeri e date. |
| [setQuotePrefix(boolean value)](#setQuotePrefix-boolean-) | Indica se il valore della cella inizia con un apice singolo. |
| [setRightBorderStyle(WebBorderStyle value)](#setRightBorderStyle-com.aspose.gridweb.WebBorderStyle-) | Specifica lo stile del bordo destro della cella. |
| [setRotationAngle(short value)](#setRotationAngle-short-) | Imposta l'attributo Rotazione. |
| [setTopBorderStyle(WebBorderStyle value)](#setTopBorderStyle-com.aspose.gridweb.WebBorderStyle-) | Specifica lo stile del bordo superiore della cella. |
| [setVerticalAlign(int value)](#setVerticalAlign-int-) | Imposta l'allineamento verticale nello stile |
| [setWidth(Unit value)](#setWidth-com.aspose.gridweb.Unit-) | Imposta la Width nello stile |
| [setWrap(boolean value)](#setWrap-boolean-) | Imposta l'opzione di a capo nello stile |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridTableItemStyle() {#GridTableItemStyle--}
```
public GridTableItemStyle()
```


Costruttore predefinito.

### copyFrom(WebStyle s) {#copyFrom-com.aspose.gridweb.WebStyle-}
```
public void copyFrom(WebStyle s)
```


Copia da un altro oggetto di stile.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| s | [WebStyle](../../com.aspose.gridweb/webstyle) | un altro oggetto stile |

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
### getBackColor() {#getBackColor--}
```
public Color getBackColor()
```


Ottiene il BackColor nello stile

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getBackImageAttributes() {#getBackImageAttributes--}
```
public String getBackImageAttributes()
```


Attributi dell'immagine di sfondo.

**Returns:**
java.lang.String
### getBackImageUrl() {#getBackImageUrl--}
```
public String getBackImageUrl()
```


URL dell'immagine di sfondo.

**Returns:**
java.lang.String
### getBorderColor() {#getBorderColor--}
```
public Color getBorderColor()
```


Ottiene il BorderColor nello stile

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getBorderStyle() {#getBorderStyle--}
```
public int getBorderStyle()
```


Ottiene il BorderStyle nello stile

Vedi [BorderStyle](../../com.aspose.gridweb/borderstyle).

**Returns:**
int
### getBorderWidth() {#getBorderWidth--}
```
public Unit getBorderWidth()
```


Ottiene il BorderWidth nello stile

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### getBottomBorderStyle() {#getBottomBorderStyle--}
```
public WebBorderStyle getBottomBorderStyle()
```


Specifica lo stile del bordo inferiore della cella.

**Returns:**
[WebBorderStyle](../../com.aspose.gridweb/webborderstyle)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCssClass() {#getCssClass--}
```
public String getCssClass()
```


Ottiene il CssClass nello stile

**Returns:**
java.lang.String
### getCustom() {#getCustom--}
```
public String getCustom()
```


Ottiene il formato personalizzato, null o stringa vuota indica nessun formato personalizzato.

**Returns:**
java.lang.String
### getFont() {#getFont--}
```
public FontInfo getFont()
```


Ottiene il Font nello stile

**Returns:**
[FontInfo](../../com.aspose.gridweb/fontinfo)
### getForeColor() {#getForeColor--}
```
public Color getForeColor()
```


Ottiene il ForeColor nello stile

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getHeight() {#getHeight--}
```
public Unit getHeight()
```


Ottiene l'Height nello stile

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### getHorizontalAlign() {#getHorizontalAlign--}
```
public int getHorizontalAlign()
```


Ottiene l'HorizontalAlign nello stile

Vedi [HorizontalAlign](../../com.aspose.gridweb/horizontalalign).

**Returns:**
int
### getIndentLevel() {#getIndentLevel--}
```
public int getIndentLevel()
```


Ottiene il livello di rientro.

**Remarks**

**Returns:**
int
### getLeftBorderStyle() {#getLeftBorderStyle--}
```
public WebBorderStyle getLeftBorderStyle()
```


Specifica lo stile del bordo sinistro della cella.

**Returns:**
[WebBorderStyle](../../com.aspose.gridweb/webborderstyle)
### getNumberType() {#getNumberType--}
```
public int getNumberType()
```


Restituisce il formato di visualizzazione di numeri e date. I modelli di formattazione variano per diverse regioni.

**Remarks**

Ad esempio, i modelli di formattazione rappresentati da numeri per la regione en\_US:

| Valore | Tipo | Stringa di formato |
| ----- | ---------- | ---------------------------------------------------- |
| 0 | General | `General` |
| 1 | Decimal | `0` |
| 2 | Decimal | `0.00` |
| 3 | Decimal | `#,##0` |
| 4 | Decimal | `#,##0.00` |
| 5 | Currency | `$#,##0_);($#,##0)` |
| 6 | Currency | `$#,##0_);[Rosso](../$#,##0)` |
| 7 | Currency | `$#,##0.00_);($#,##0.00)` |
| 8 | Currency | `$#,##0.00_);[Rosso](../$#,##0.00)` |
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
| 38 | Accounting | `#,##0_);[Rosso](../#,##0)` |
| 39 | Accounting | `#,##0.00_);(#,##0.00)` |
| 40 | Accounting | `#,##0.00_);[Rosso](../#,##0.00)` |
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
### getQuotePrefix() {#getQuotePrefix--}
```
public boolean getQuotePrefix()
```


Indica se il valore della cella inizia con un apice singolo.

**Returns:**
boolean
### getRightBorderStyle() {#getRightBorderStyle--}
```
public WebBorderStyle getRightBorderStyle()
```


Specifica lo stile del bordo destro della cella.

**Returns:**
[WebBorderStyle](../../com.aspose.gridweb/webborderstyle)
### getRotationAngle() {#getRotationAngle--}
```
public short getRotationAngle()
```


Ottiene l'attributo Rotazione.

**Remarks**

0: Non ruotato.

255: Dall'alto verso il basso.

\-90: Verso il basso.

90: Verso l'alto.

È possibile impostare 255 o un valore compreso tra -90 e 90.

**Returns:**
short
### getTopBorderStyle() {#getTopBorderStyle--}
```
public WebBorderStyle getTopBorderStyle()
```


Specifica lo stile del bordo superiore della cella.

**Returns:**
[WebBorderStyle](../../com.aspose.gridweb/webborderstyle)
### getVerticalAlign() {#getVerticalAlign--}
```
public int getVerticalAlign()
```


Ottiene l'allineamento verticale nello stile

Vedi [VerticalAlign](../../com.aspose.gridweb/verticalalign).

**Returns:**
int
### getWidth() {#getWidth--}
```
public Unit getWidth()
```


Ottiene la Width nello stile

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### getWrap() {#getWrap--}
```
public boolean getWrap()
```


Ottiene l'opzione di a capo nello stile

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public int hashCode()
```


Funziona come funzione hash per un tipo specifico, adatta all'uso in algoritmi di hashing e strutture dati come una tabella hash.

**Returns:**
int - Un codice hash per lo stile corrente.
### isLocked() {#isLocked--}
```
public boolean isLocked()
```


Restituisce un valore che indica se una cella può essere modificata o meno quando il foglio di lavoro è protetto. Quando il foglio di lavoro è protetto e IsLocked è true, la cella non può essere modificata. Quando il foglio di lavoro è protetto e IsLocked è false, la cella può essere modificata.

**Returns:**
boolean
### mergeWith(WebStyle s) {#mergeWith-com.aspose.gridweb.WebStyle-}
```
public void mergeWith(WebStyle s)
```


Unisce con un altro oggetto di stile.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| s | [WebStyle](../../com.aspose.gridweb/webstyle) | un altro oggetto stile |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setBackColor(Color value) {#setBackColor-com.aspose.gridweb.Color-}
```
public void setBackColor(Color value)
```


Imposta il BackColor nello stile

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setBackImageAttributes(String value) {#setBackImageAttributes-java.lang.String-}
```
public void setBackImageAttributes(String value)
```


Attributi dell'immagine di sfondo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setBackImageUrl(String value) {#setBackImageUrl-java.lang.String-}
```
public void setBackImageUrl(String value)
```


URL dell'immagine di sfondo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setBorderColor(Color value) {#setBorderColor-com.aspose.gridweb.Color-}
```
public void setBorderColor(Color value)
```


Imposta il BorderColor nello stile

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setBorderStyle(int value) {#setBorderStyle-int-}
```
public void setBorderStyle(int value)
```


Imposta il BorderStyle nello stile

Vedi [BorderStyle](../../com.aspose.gridweb/borderstyle).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setBorderWidth(Unit value) {#setBorderWidth-com.aspose.gridweb.Unit-}
```
public void setBorderWidth(Unit value)
```


Imposta il BorderWidth nello stile

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

### setBottomBorderStyle(WebBorderStyle value) {#setBottomBorderStyle-com.aspose.gridweb.WebBorderStyle-}
```
public void setBottomBorderStyle(WebBorderStyle value)
```


Specifica lo stile del bordo inferiore della cella.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [WebBorderStyle](../../com.aspose.gridweb/webborderstyle) |  |

### setCssClass(String value) {#setCssClass-java.lang.String-}
```
public void setCssClass(String value)
```


Imposta il CssClass nello stile

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setCustom(String value) {#setCustom-java.lang.String-}
```
public void setCustom(String value)
```


Imposta il formato personalizzato, null o stringa vuota indica nessun formato personalizzato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setForeColor(Color value) {#setForeColor-com.aspose.gridweb.Color-}
```
public void setForeColor(Color value)
```


Imposta il ForeColor nello stile

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setHeight(Unit value) {#setHeight-com.aspose.gridweb.Unit-}
```
public void setHeight(Unit value)
```


Imposta l'Height nello stile

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

### setHorizontalAlign(int value) {#setHorizontalAlign-int-}
```
public void setHorizontalAlign(int value)
```


Imposta l'HorizontalAlign nello stile

Vedi [HorizontalAlign](../../com.aspose.gridweb/horizontalalign).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setIndentLevel(int value) {#setIndentLevel-int-}
```
public void setIndentLevel(int value)
```


Imposta il livello di rientro.

**Remarks**

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setLeftBorderStyle(WebBorderStyle value) {#setLeftBorderStyle-com.aspose.gridweb.WebBorderStyle-}
```
public void setLeftBorderStyle(WebBorderStyle value)
```


Specifica lo stile del bordo sinistro della cella.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [WebBorderStyle](../../com.aspose.gridweb/webborderstyle) |  |

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


Imposta un valore che indica se una cella può essere modificata o non quando il foglio di lavoro è protetto. Quando il foglio di lavoro è protetto e IsLocked è true, la cella non può essere modificata. Quando il foglio di lavoro è protetto e IsLocked è false, la cella può essere modificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setNumberType(int value) {#setNumberType-int-}
```
public void setNumberType(int value)
```


Imposta il formato di visualizzazione di numeri e date. I modelli di formattazione sono diversi per le varie regioni.

**Remarks**

Ad esempio, i modelli di formattazione rappresentati da numeri per la regione en\_US:

| Valore | Tipo | Stringa di formato |
| ----- | ---------- | ---------------------------------------------------- |
| 0 | General | `General` |
| 1 | Decimal | `0` |
| 2 | Decimal | `0.00` |
| 3 | Decimal | `#,##0` |
| 4 | Decimal | `#,##0.00` |
| 5 | Currency | `$#,##0_);($#,##0)` |
| 6 | Currency | `$#,##0_);[Rosso](../$#,##0)` |
| 7 | Currency | `$#,##0.00_);($#,##0.00)` |
| 8 | Currency | `$#,##0.00_);[Rosso](../$#,##0.00)` |
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
| 38 | Accounting | `#,##0_);[Rosso](../#,##0)` |
| 39 | Accounting | `#,##0.00_);(#,##0.00)` |
| 40 | Accounting | `#,##0.00_);[Rosso](../#,##0.00)` |
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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setQuotePrefix(boolean value) {#setQuotePrefix-boolean-}
```
public void setQuotePrefix(boolean value)
```


Indica se il valore della cella inizia con un apice singolo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setRightBorderStyle(WebBorderStyle value) {#setRightBorderStyle-com.aspose.gridweb.WebBorderStyle-}
```
public void setRightBorderStyle(WebBorderStyle value)
```


Specifica lo stile del bordo destro della cella.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [WebBorderStyle](../../com.aspose.gridweb/webborderstyle) |  |

### setRotationAngle(short value) {#setRotationAngle-short-}
```
public void setRotationAngle(short value)
```


Imposta l'attributo Rotazione.

**Remarks**

0: Non ruotato.

255: Dall'alto verso il basso.

\-90: Verso il basso.

90: Verso l'alto.

È possibile impostare 255 o un valore compreso tra -90 e 90.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | short |  |

### setTopBorderStyle(WebBorderStyle value) {#setTopBorderStyle-com.aspose.gridweb.WebBorderStyle-}
```
public void setTopBorderStyle(WebBorderStyle value)
```


Specifica lo stile del bordo superiore della cella.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [WebBorderStyle](../../com.aspose.gridweb/webborderstyle) |  |

### setVerticalAlign(int value) {#setVerticalAlign-int-}
```
public void setVerticalAlign(int value)
```


Imposta l'allineamento verticale nello stile

Vedi [VerticalAlign](../../com.aspose.gridweb/verticalalign).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setWidth(Unit value) {#setWidth-com.aspose.gridweb.Unit-}
```
public void setWidth(Unit value)
```


Imposta la Width nello stile

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Unit](../../com.aspose.gridweb/unit) |  |

### setWrap(boolean value) {#setWrap-boolean-}
```
public void setWrap(boolean value)
```


Imposta l'opzione di a capo nello stile

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

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

