---
title: "Style"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta lo stile di visualizzazione di documenti Excel, come carattere, colore, allineamento, bordo, ecc."
type: docs
url: /it/java/com.aspose.cells/style/
---

**Inheritance:**
java.lang.Object
```
public class Style
```

Rappresenta lo stile di visualizzazione di un documento Excel, come carattere, colore, allineamento, bordo, ecc. L'oggetto Style contiene tutti gli attributi di stile (carattere, formato numerico, allineamento e così via) come proprietà.

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
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [Style()](#Style--) | Inizializza una nuova istanza della classe [Style](../../com.aspose.cells/style). |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [copy(Style style)](#copy-com.aspose.cells.Style-) | Copia i dati da un altro oggetto style |
| [equals(Object obj)](#equals-java.lang.Object-) | Determina se due istanze di Style sono uguali. |
| [getBackgroundArgbColor()](#getBackgroundArgbColor--) | Ottiene il colore di sfondo con un valore ARGB a 32 bit. |
| [getBackgroundColor()](#getBackgroundColor--) | Ottiene il colore di sfondo di uno style. |
| [getBackgroundThemeColor()](#getBackgroundThemeColor--) | Ottiene il colore del tema di sfondo. |
| [getBorders()](#getBorders--) | Ottiene la [BorderCollection](../../com.aspose.cells/bordercollection) dello style. |
| [getBottomBorder()](#getBottomBorder--) | Ottiene il bordo inferiore. |
| [getClass()](#getClass--) |  |
| [getCultureCustom()](#getCultureCustom--) | Ottiene la stringa di modello dipendente dalla cultura per il formato numerico. |
| [getCustom()](#getCustom--) | Rappresenta la stringa di formato numerico personalizzato di questo oggetto style. |
| [getFont()](#getFont--) | Ottiene un oggetto [getFont()](../../com.aspose.cells/style\#getFont--). |
| [getForegroundArgbColor()](#getForegroundArgbColor--) | Ottiene il colore di primo piano con un valore ARGB a 32 bit. |
| [getForegroundColor()](#getForegroundColor--) | Ottiene il colore di primo piano di uno style. |
| [getForegroundThemeColor()](#getForegroundThemeColor--) | Ottiene il colore del tema in primo piano. |
| [getHorizontalAlignment()](#getHorizontalAlignment--) | Ottiene il tipo di allineamento orizzontale del testo in una cella. |
| [getIndentLevel()](#getIndentLevel--) | Rappresenta il livello di rientro per la cella o l'intervallo. |
| [getInvariantCustom()](#getInvariantCustom--) | Ottiene la stringa di modello indipendente dalla cultura per il formato numerico. |
| [getLeftBorder()](#getLeftBorder--) | Ottiene il bordo sinistro. |
| [getName()](#getName--) | Ottiene il nome dello stile. |
| [getNumber()](#getNumber--) | Ottiene il formato di visualizzazione di numeri e date. |
| [getParentStyle()](#getParentStyle--) | Ottiene lo stile genitore di questo stile. |
| [getPattern()](#getPattern--) | Ottiene il tipo di modello di sfondo della cella. |
| [getQuotePrefix()](#getQuotePrefix--) | Indica se il valore della cella inizia con un apice singolo. |
| [getRightBorder()](#getRightBorder--) | Ottiene il bordo destro. |
| [getRotationAngle()](#getRotationAngle--) | Rappresenta l'angolo di rotazione del testo. |
| [getShrinkToFit()](#getShrinkToFit--) | Rappresenta se il testo si riduce automaticamente per adattarsi alla larghezza di colonna disponibile. |
| [getTextDirection()](#getTextDirection--) | Rappresenta l'ordine di lettura del testo. |
| [getTopBorder()](#getTopBorder--) | Ottiene il bordo superiore. |
| [getTwoColorGradient()](#getTwoColorGradient--) | Ottieni l'impostazione del gradiente a due colori. |
| [getTwoColorGradientSetting()](#getTwoColorGradientSetting--) | Ottieni l'impostazione del gradiente a due colori. |
| [getVerticalAlignment()](#getVerticalAlignment--) | Ottiene il tipo di allineamento verticale del testo in una cella. |
| [hasBorders()](#hasBorders--) | Verifica se sono stati impostati bordi per lo stile. |
| [hashCode()](#hashCode--) | Funziona come funzione hash per un oggetto Style. |
| [isAlignmentApplied()](#isAlignmentApplied--) | Indica se la formattazione dell'allineamento deve essere applicata. |
| [isBorderApplied()](#isBorderApplied--) | Indica se la formattazione del bordo deve essere applicata. |
| [isCheckBox()](#isCheckBox--) | Indica se è uno stile di casella di controllo |
| [isDateTime()](#isDateTime--) | Indica se il formato numerico è un formato data. |
| [isFillApplied()](#isFillApplied--) | Indica se la formattazione di riempimento deve essere applicata. |
| [isFontApplied()](#isFontApplied--) | Indica se la formattazione del carattere deve essere applicata. |
| [isFormulaHidden()](#isFormulaHidden--) | Rappresenta se la formula sarà nascosta quando il foglio di lavoro è protetto. |
| [isGradient()](#isGradient--) | Indica se l'ombreggiatura della cella è un motivo gradiente. |
| [isJustifyDistributed()](#isJustifyDistributed--) | Indica se l'allineamento giustificato o distribuito delle celle dovrebbe essere usato sull'ultima riga di testo. |
| [isLocked()](#isLocked--) | Ottiene un valore che indica se una cella può essere modificata o meno. |
| [isModified(int modifyFlag)](#isModified-int-) | Verifica se le proprietà specificate dello stile sono state modificate. |
| [isNumberFormatApplied()](#isNumberFormatApplied--) | Indica se la formattazione dei numeri dovrebbe essere applicata. |
| [isPercent()](#isPercent--) | Indica se il formato numerico è un formato percentuale. |
| [isProtectionApplied()](#isProtectionApplied--) | Indica se la formattazione di protezione dovrebbe essere applicata. |
| [isTextWrapped()](#isTextWrapped--) | Ottiene un valore che indica se il testo all'interno di una cella è a capo. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAlignmentApplied(boolean value)](#setAlignmentApplied-boolean-) | Indica se la formattazione dell'allineamento deve essere applicata. |
| [setBackgroundArgbColor(int value)](#setBackgroundArgbColor-int-) | Imposta il colore di sfondo con un valore ARGB a 32 bit. |
| [setBackgroundColor(Color value)](#setBackgroundColor-com.aspose.cells.Color-) | Imposta il colore di sfondo di uno stile. |
| [setBackgroundThemeColor(ThemeColor value)](#setBackgroundThemeColor-com.aspose.cells.ThemeColor-) | Imposta il colore del tema di sfondo. |
| [setBorder(int borderType, int borderStyle, CellsColor borderColor)](#setBorder-int-int-com.aspose.cells.CellsColor-) | Imposta i bordi dello stile. |
| [setBorder(int borderType, int borderStyle, Color borderColor)](#setBorder-int-int-com.aspose.cells.Color-) | Imposta i bordi dello stile. |
| [setBorderApplied(boolean value)](#setBorderApplied-boolean-) | Indica se la formattazione del bordo deve essere applicata. |
| [setCheckBox(boolean value)](#setCheckBox-boolean-) | Indica se è uno stile di casella di controllo |
| [setCultureCustom(String value)](#setCultureCustom-java.lang.String-) | Imposta la stringa di modello dipendente dalla cultura per il formato numerico. |
| [setCustom(String value)](#setCustom-java.lang.String-) | Rappresenta la stringa di formato numerico personalizzato di questo oggetto style. |
| [setCustom(String custom, boolean builtinPreference)](#setCustom-java.lang.String-boolean-) | Imposta la stringa di formato numerico personalizzato di una cella. |
| [setFillApplied(boolean value)](#setFillApplied-boolean-) | Indica se la formattazione di riempimento deve essere applicata. |
| [setFontApplied(boolean value)](#setFontApplied-boolean-) | Indica se la formattazione del carattere deve essere applicata. |
| [setForegroundArgbColor(int value)](#setForegroundArgbColor-int-) | Imposta il colore di primo piano con un valore ARGB a 32 bit. |
| [setForegroundColor(Color value)](#setForegroundColor-com.aspose.cells.Color-) | Imposta il colore di primo piano di uno stile. |
| [setForegroundThemeColor(ThemeColor value)](#setForegroundThemeColor-com.aspose.cells.ThemeColor-) | Imposta il colore del tema di primo piano. |
| [setFormulaHidden(boolean value)](#setFormulaHidden-boolean-) | Rappresenta se la formula sarà nascosta quando il foglio di lavoro è protetto. |
| [setGradient(boolean value)](#setGradient-boolean-) | Indica se l'ombreggiatura della cella è un motivo gradiente. |
| [setHorizontalAlignment(int value)](#setHorizontalAlignment-int-) | Imposta il tipo di allineamento orizzontale del testo in una cella. |
| [setIndentLevel(int value)](#setIndentLevel-int-) | Rappresenta il livello di rientro per la cella o l'intervallo. |
| [setJustifyDistributed(boolean value)](#setJustifyDistributed-boolean-) | Indica se l'allineamento giustificato o distribuito delle celle dovrebbe essere usato sull'ultima riga di testo. |
| [setLocked(boolean value)](#setLocked-boolean-) | Imposta un valore che indica se una cella può essere modificata o meno. |
| [setName(String value)](#setName-java.lang.String-) | Imposta il nome dello stile. |
| [setNumber(int value)](#setNumber-int-) | Imposta il formato di visualizzazione di numeri e date. |
| [setNumberFormatApplied(boolean value)](#setNumberFormatApplied-boolean-) | Indica se la formattazione dei numeri dovrebbe essere applicata. |
| [setOutlineBorders(int borderStyle, CellsColor borderColor)](#setOutlineBorders-int-com.aspose.cells.CellsColor-) | Imposta i bordi di contorno |
| [setOutlineBorders(int borderStyle, Color borderColor)](#setOutlineBorders-int-com.aspose.cells.Color-) | Imposta i bordi di contorno |
| [setPattern(int value)](#setPattern-int-) | Imposta il tipo di motivo di sfondo della cella. |
| [setPatternColor(int pattern, Color color1, Color color2)](#setPatternColor-int-com.aspose.cells.Color-com.aspose.cells.Color-) | Imposta il colore di sfondo. |
| [setProtectionApplied(boolean value)](#setProtectionApplied-boolean-) | Indica se la formattazione di protezione dovrebbe essere applicata. |
| [setQuotePrefix(boolean value)](#setQuotePrefix-boolean-) | Indica se il valore della cella inizia con un apice singolo. |
| [setRotationAngle(int value)](#setRotationAngle-int-) | Rappresenta l'angolo di rotazione del testo. |
| [setShrinkToFit(boolean value)](#setShrinkToFit-boolean-) | Rappresenta se il testo si riduce automaticamente per adattarsi alla larghezza di colonna disponibile. |
| [setTextDirection(int value)](#setTextDirection-int-) | Rappresenta l'ordine di lettura del testo. |
| [setTextWrapped(boolean value)](#setTextWrapped-boolean-) | Imposta un valore che indica se il testo all'interno di una cella è a capo. |
| [setTwoColorGradient(Color color1, Color color2, int gradientStyleType, int variant)](#setTwoColorGradient-com.aspose.cells.Color-com.aspose.cells.Color-int-int-) | Imposta il riempimento specificato a un gradiente a due colori. |
| [setVerticalAlignment(int value)](#setVerticalAlignment-int-) | Imposta il tipo di allineamento verticale del testo in una cella. |
| [toJson()](#toJson--) | Converti [Style](../../com.aspose.cells/style) in dati struct JSON. |
| [toString()](#toString--) |  |
| [update()](#update--) | Applica lo stile denominato agli stili delle celle che utilizzano questo stile denominato. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### Style() {#Style--}
```
public Style()
```


Inizializza una nuova istanza della classe [Style](../../com.aspose.cells/style).

**Remarks**

NOTA: Questo costruttore è ora obsoleto. Invece, si prega di utilizzare il metodo CellsFactory.CreateStyle(). Questa proprietà sarà rimossa 6 mesi dopo, a partire da ottobre 2016. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### copy(Style style) {#copy-com.aspose.cells.Style-}
```
public void copy(Style style)
```


Copia i dati da un altro oggetto style

**Remarks**

Questo metodo non copia il nome dello stile. Se vuoi copiare il nome, si prega di chiamare i seguenti codici dopo aver copiato lo stile: destStyle.Name = style.Name.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | Oggetto Style di origine |

### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Determina se due istanze di Style sono uguali.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| obj | java.lang.Object | L'oggetto Style da confrontare con l'oggetto Style corrente. |

**Returns:**
boolean - true se l'Object specificato è uguale all'Object corrente; altrimenti, false.
### getBackgroundArgbColor() {#getBackgroundArgbColor--}
```
public int getBackgroundArgbColor()
```


Ottiene il colore di sfondo con un valore ARGB a 32 bit.

**Returns:**
int
### getBackgroundColor() {#getBackgroundColor--}
```
public Color getBackgroundColor()
```


Ottiene il colore di sfondo di uno style.

**Remarks**

Se vuoi impostare il colore di una cella, si prega di utilizzare la proprietà Style.ForegroundColor. Solo se il modello di stile della cella è diverso da nessuno o solido, questa proprietà avrà effetto.

**Returns:**
[Color](../../com.aspose.cells/color)
### getBackgroundThemeColor() {#getBackgroundThemeColor--}
```
public ThemeColor getBackgroundThemeColor()
```


Ottiene il colore del tema di sfondo.

**Remarks**

Se il colore di sfondo non è un colore tema, verrà restituito NULL.

**Returns:**
[ThemeColor](../../com.aspose.cells/themecolor)
### getBorders() {#getBorders--}
```
public BorderCollection getBorders()
```


Ottiene la [BorderCollection](../../com.aspose.cells/bordercollection) dello style.

**Returns:**
[BorderCollection](../../com.aspose.cells/bordercollection)
### getBottomBorder() {#getBottomBorder--}
```
public Border getBottomBorder()
```


Ottiene il bordo inferiore.

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


Restituisce la stringa di modello dipendente dalla cultura per il formato numerico. Se non è stato impostato alcun formato numerico per questo oggetto, verrà restituito null. Se il formato numerico è incorporato, verrà restituita la stringa di modello corrispondente al numero incorporato.

**Remarks**

Per i formati numerici incorporati, sia il contenuto del modello (ad esempio, un formato data incorporato è \"m/d/y\" per alcune località, ma per altre località diventa \"d/m/y\") sia il specificatore di formato (ad esempio, alcune località usano un carattere diverso da 'y' per rappresentare la parte dell'anno nella formattazione delle date) sono dipendenti dalla cultura; per i formati personalizzati specificati dall'utente, solo i specificatori di formato vengono modificati in base alla cultura, le altre parti del modello di formattazione non verranno modificate.

**Returns:**
java.lang.String
### getCustom() {#getCustom--}
```
public String getCustom()
```


Rappresenta la stringa del formato numerico personalizzato di questo oggetto style. Se il formato numerico personalizzato non è impostato (ad esempio, il formato numerico è incorporato), verrà restituita \"\".

**Remarks**

La stringa personalizzata restituita è indipendente dalla cultura.

**Returns:**
java.lang.String
### getFont() {#getFont--}
```
public Font getFont()
```


Ottiene un oggetto [getFont()](../../com.aspose.cells/style\#getFont--).

**Returns:**
[Font](../../com.aspose.cells/font)
### getForegroundArgbColor() {#getForegroundArgbColor--}
```
public int getForegroundArgbColor()
```


Ottiene il colore di primo piano con un valore ARGB a 32 bit.

**Returns:**
int
### getForegroundColor() {#getForegroundColor--}
```
public Color getForegroundColor()
```


Ottiene il colore di primo piano di uno style.

**Remarks**

Significa nessuna impostazione di colore se viene restituito Color.Empty.

**Returns:**
[Color](../../com.aspose.cells/color)
### getForegroundThemeColor() {#getForegroundThemeColor--}
```
public ThemeColor getForegroundThemeColor()
```


Ottiene il colore del tema in primo piano.

**Remarks**

Se il colore di primo piano non è un colore di tema, NULL verrà restituito.

**Returns:**
[ThemeColor](../../com.aspose.cells/themecolor)
### getHorizontalAlignment() {#getHorizontalAlignment--}
```
public int getHorizontalAlignment()
```


Ottiene il tipo di allineamento orizzontale del testo in una cella.

Vedi [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Returns:**
int
### getIndentLevel() {#getIndentLevel--}
```
public int getIndentLevel()
```


Rappresenta il livello di rientro per la cella o l'intervallo. Può essere solo un intero da 0 a 250.

**Remarks**

Se il tipo di allineamento orizzontale del testo è impostato su un valore diverso da sinistra o destra, il livello di rientro verrà reimpostato a zero.

**Returns:**
int
### getInvariantCustom() {#getInvariantCustom--}
```
public String getInvariantCustom()
```


Restituisce la stringa di modello indipendente dalla cultura per il formato numerico. Se non è stato impostato alcun formato numerico per questo oggetto, verrà restituito null. Se il formato numerico è incorporato, verrà restituita la stringa di modello corrispondente al numero incorporato.

**Remarks**

Per i formati numerici incorporati, il contenuto del modello restituito è ancora dipendente dalla cultura, ad esempio, per alcune località restituisce \"m/d/y\" e per altre località restituisce \"d/m/y\". La differenza rispetto a [getCultureCustom()](../../com.aspose.cells/style\#getCultureCustom--) è (che è anche ciò che significa indipendente dalla cultura): i specificatori di formato e i separatori sono mantenuti come standard, ad esempio '/' sarà sempre usato come separatore di data/ora e \"y\" sarà sempre usato come parte \"anno\" indipendentemente da quale altro carattere speciale sia usato per la specifica località.

**Returns:**
java.lang.String
### getLeftBorder() {#getLeftBorder--}
```
public Border getLeftBorder()
```


Ottiene il bordo sinistro.

**Returns:**
[Border](../../com.aspose.cells/border)
### getName() {#getName--}
```
public String getName()
```


Ottiene il nome dello stile.

**Returns:**
java.lang.String
### getNumber() {#getNumber--}
```
public int getNumber()
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
### getParentStyle() {#getParentStyle--}
```
public Style getParentStyle()
```


Ottiene lo stile genitore di questo stile.

**Returns:**
[Style](../../com.aspose.cells/style)
### getPattern() {#getPattern--}
```
public int getPattern()
```


Ottiene il tipo di modello di sfondo della cella.

Vedi [BackgroundType](../../com.aspose.cells/backgroundtype).

**Returns:**
int
### getQuotePrefix() {#getQuotePrefix--}
```
public boolean getQuotePrefix()
```


Indica se il valore della cella inizia con un apice singolo.

**Returns:**
boolean
### getRightBorder() {#getRightBorder--}
```
public Border getRightBorder()
```


Ottiene il bordo destro.

**Returns:**
[Border](../../com.aspose.cells/border)
### getRotationAngle() {#getRotationAngle--}
```
public int getRotationAngle()
```


Rappresenta l'angolo di rotazione del testo.

**Remarks**

0: Non ruotato.

255: Dall'alto verso il basso.

\-90: Verso il basso.

90: Verso l'alto.

È possibile impostare 255 o un valore compreso tra -90 e 90.

**Returns:**
int
### getShrinkToFit() {#getShrinkToFit--}
```
public boolean getShrinkToFit()
```


Rappresenta se il testo si riduce automaticamente per adattarsi alla larghezza di colonna disponibile.

**Returns:**
boolean
### getTextDirection() {#getTextDirection--}
```
public int getTextDirection()
```


Rappresenta l'ordine di lettura del testo.

Vedi [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Returns:**
int
### getTopBorder() {#getTopBorder--}
```
public Border getTopBorder()
```


Ottiene il bordo superiore.

**Returns:**
[Border](../../com.aspose.cells/border)
### getTwoColorGradient() {#getTwoColorGradient--}
```
public Object[] getTwoColorGradient()
```


Ottieni l'impostazione del gradiente a due colori.

**Remarks**

NOTA: Questo metodo è ora obsoleto. Invece, si prega di utilizzare il metodo Style.GetTwoColorGradientSetting(). Questa proprietà sarà rimossa 12 mesi dopo, a partire da dicembre 2022. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

**Returns:**
java.lang.Object[] - Restituisce tutte le impostazioni sul gradiente a due colori [0] : Color1 [1] : Color2 [2] : GradientStyleType [3] : Variant
### getTwoColorGradientSetting() {#getTwoColorGradientSetting--}
```
public TwoColorGradient getTwoColorGradientSetting()
```


Ottieni l'impostazione del gradiente a due colori.

**Returns:**
[TwoColorGradient](../../com.aspose.cells/twocolorgradient)
### getVerticalAlignment() {#getVerticalAlignment--}
```
public int getVerticalAlignment()
```


Ottiene il tipo di allineamento verticale del testo in una cella.

Vedi [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Returns:**
int
### hasBorders() {#hasBorders--}
```
public boolean hasBorders()
```


Verifica se sono stati impostati bordi per lo stile.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public int hashCode()
```


Funziona come funzione hash per un oggetto Style.

**Remarks**

Questo metodo è solo per uso interno.

**Returns:**
int - Un codice hash per l'oggetto corrente.
### isAlignmentApplied() {#isAlignmentApplied--}
```
public boolean isAlignmentApplied()
```


Indica se la formattazione dell'allineamento deve essere applicata.

**Remarks**

Solo per stile denominato.

**Returns:**
boolean
### isBorderApplied() {#isBorderApplied--}
```
public boolean isBorderApplied()
```


Indica se la formattazione del bordo deve essere applicata.

**Remarks**

Solo per stile denominato.

**Returns:**
boolean
### isCheckBox() {#isCheckBox--}
```
public boolean isCheckBox()
```


Indica se è uno stile di casella di controllo

**Returns:**
boolean
### isDateTime() {#isDateTime--}
```
public boolean isDateTime()
```


Indica se il formato numerico è un formato data.

**Returns:**
boolean
### isFillApplied() {#isFillApplied--}
```
public boolean isFillApplied()
```


Indica se la formattazione di riempimento deve essere applicata.

**Remarks**

Solo per stile denominato.

**Returns:**
boolean
### isFontApplied() {#isFontApplied--}
```
public boolean isFontApplied()
```


Indica se la formattazione del carattere deve essere applicata.

**Remarks**

Solo per stile denominato.

**Returns:**
boolean
### isFormulaHidden() {#isFormulaHidden--}
```
public boolean isFormulaHidden()
```


Rappresenta se la formula sarà nascosta quando il foglio di lavoro è protetto.

**Returns:**
boolean
### isGradient() {#isGradient--}
```
public boolean isGradient()
```


Indica se l'ombreggiatura della cella è un motivo gradiente.

**Returns:**
boolean
### isJustifyDistributed() {#isJustifyDistributed--}
```
public boolean isJustifyDistributed()
```


Indica se l'allineamento giustificato o distribuito delle celle dovrebbe essere usato sull'ultima riga di testo.

**Remarks**

Questo è tipico per gli allineamenti dell'Asia orientale ma non è tipico in altri contesti. Funziona solo quando l'allineamento orizzontale è distribuito.

**Returns:**
boolean
### isLocked() {#isLocked--}
```
public boolean isLocked()
```


Ottiene un valore che indica se una cella può essere modificata o meno.

**Remarks**

Bloccare le celle non ha effetto a meno che il foglio di lavoro non sia protetto.

**Returns:**
boolean
### isModified(int modifyFlag) {#isModified-int-}
```
public boolean isModified(int modifyFlag)
```


Verifica se le proprietà specificate dello stile sono state modificate. Utilizzato per lo stile dei ConditionalFormattings per verificare se le proprietà specificate di questo stile devono essere usate durante l'applicazione dei ConditionalFormattings su una cella.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| modifyFlag | int | [StyleModifyFlag](../../com.aspose.cells/stylemodifyflag). Flag di modifica dello stile |

**Returns:**
boolean - vero se le proprietà specificate sono state modificate
### isNumberFormatApplied() {#isNumberFormatApplied--}
```
public boolean isNumberFormatApplied()
```


Indica se la formattazione dei numeri dovrebbe essere applicata.

**Remarks**

Solo per stile denominato.

**Returns:**
boolean
### isPercent() {#isPercent--}
```
public boolean isPercent()
```


Indica se il formato numerico è un formato percentuale.

**Returns:**
boolean
### isProtectionApplied() {#isProtectionApplied--}
```
public boolean isProtectionApplied()
```


Indica se la formattazione di protezione dovrebbe essere applicata.

**Remarks**

Solo per stile denominato.

**Returns:**
boolean
### isTextWrapped() {#isTextWrapped--}
```
public boolean isTextWrapped()
```


Ottiene un valore che indica se il testo all'interno di una cella è a capo.

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


Indica se la formattazione dell'allineamento deve essere applicata.

**Remarks**

Solo per stile denominato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setBackgroundArgbColor(int value) {#setBackgroundArgbColor-int-}
```
public void setBackgroundArgbColor(int value)
```


Imposta il colore di sfondo con un valore ARGB a 32 bit.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setBackgroundColor(Color value) {#setBackgroundColor-com.aspose.cells.Color-}
```
public void setBackgroundColor(Color value)
```


Imposta il colore di sfondo di uno stile.

**Remarks**

Se vuoi impostare il colore di una cella, si prega di utilizzare la proprietà Style.ForegroundColor. Solo se il modello di stile della cella è diverso da nessuno o solido, questa proprietà avrà effetto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setBackgroundThemeColor(ThemeColor value) {#setBackgroundThemeColor-com.aspose.cells.ThemeColor-}
```
public void setBackgroundThemeColor(ThemeColor value)
```


Imposta il colore del tema di sfondo.

**Remarks**

Se il colore di sfondo non è un colore tema, verrà restituito NULL.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [ThemeColor](../../com.aspose.cells/themecolor) |  |

### setBorder(int borderType, int borderStyle, CellsColor borderColor) {#setBorder-int-int-com.aspose.cells.CellsColor-}
```
public boolean setBorder(int borderType, int borderStyle, CellsColor borderColor)
```


Imposta i bordi dello stile.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| borderType | int | [BorderType](../../com.aspose.cells/bordertype). Il(i) bordo(i) da impostare, può essere una combinazione di [BorderType](../../com.aspose.cells/bordertype). |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). Lo stile del bordo. |
| borderColor | [CellsColor](../../com.aspose.cells/cellscolor) | Il colore del bordo. |

**Returns:**
boolean - Se le impostazioni attuali del bordo sono state modificate.
### setBorder(int borderType, int borderStyle, Color borderColor) {#setBorder-int-int-com.aspose.cells.Color-}
```
public boolean setBorder(int borderType, int borderStyle, Color borderColor)
```


Imposta i bordi dello stile.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| borderType | int | [BorderType](../../com.aspose.cells/bordertype). Il(i) bordo(i) da impostare, può essere una combinazione di [BorderType](../../com.aspose.cells/bordertype). |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). Lo stile del bordo. |
| borderColor | [Color](../../com.aspose.cells/color) | Il colore del bordo. |

**Returns:**
boolean - Se le impostazioni attuali del bordo sono state modificate.
### setBorderApplied(boolean value) {#setBorderApplied-boolean-}
```
public void setBorderApplied(boolean value)
```


Indica se la formattazione del bordo deve essere applicata.

**Remarks**

Solo per stile denominato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setCheckBox(boolean value) {#setCheckBox-boolean-}
```
public void setCheckBox(boolean value)
```


Indica se è uno stile di casella di controllo

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setCultureCustom(String value) {#setCultureCustom-java.lang.String-}
```
public void setCultureCustom(String value)
```


Imposta la stringa di modello dipendente dalla cultura per il formato numerico. Se non è stato impostato alcun formato numerico per questo oggetto, verrà restituito null. Se il formato numerico è incorporato, verrà restituita la stringa di modello corrispondente al numero incorporato.

**Remarks**

Per i formati numerici incorporati, sia il contenuto del modello (ad esempio, un formato data incorporato è \"m/d/y\" per alcune località, ma per altre località diventa \"d/m/y\") sia il specificatore di formato (ad esempio, alcune località usano un carattere diverso da 'y' per rappresentare la parte dell'anno nella formattazione delle date) sono dipendenti dalla cultura; per i formati personalizzati specificati dall'utente, solo i specificatori di formato vengono modificati in base alla cultura, le altre parti del modello di formattazione non verranno modificate.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setCustom(String value) {#setCustom-java.lang.String-}
```
public void setCustom(String value)
```


Rappresenta la stringa del formato numerico personalizzato di questo oggetto style. Se il formato numerico personalizzato non è impostato (ad esempio, il formato numerico è incorporato), verrà restituita \"\".

**Remarks**

La stringa personalizzata restituita è indipendente dalla cultura.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setCustom(String custom, boolean builtinPreference) {#setCustom-java.lang.String-boolean-}
```
public void setCustom(String custom, boolean builtinPreference)
```


Imposta la stringa di formato numerico personalizzato di una cella.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| personalizzato | java.lang.String | Stringa di formato numerico personalizzato, dovrebbe essere un modello InvariantCulture. |
| builtinPreference | boolean | Se la stringa di formato numerico personalizzata fornita corrisponde a uno dei formati numerici incorporati corrispondenti alle impostazioni regionali correnti, impostare il formato numerico come incorporato invece che personalizzato. |

### setFillApplied(boolean value) {#setFillApplied-boolean-}
```
public void setFillApplied(boolean value)
```


Indica se la formattazione di riempimento deve essere applicata.

**Remarks**

Solo per stile denominato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setFontApplied(boolean value) {#setFontApplied-boolean-}
```
public void setFontApplied(boolean value)
```


Indica se la formattazione del carattere deve essere applicata.

**Remarks**

Solo per stile denominato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setForegroundArgbColor(int value) {#setForegroundArgbColor-int-}
```
public void setForegroundArgbColor(int value)
```


Imposta il colore di primo piano con un valore ARGB a 32 bit.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setForegroundColor(Color value) {#setForegroundColor-com.aspose.cells.Color-}
```
public void setForegroundColor(Color value)
```


Imposta il colore di primo piano di uno stile.

**Remarks**

Significa nessuna impostazione di colore se viene restituito Color.Empty.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setForegroundThemeColor(ThemeColor value) {#setForegroundThemeColor-com.aspose.cells.ThemeColor-}
```
public void setForegroundThemeColor(ThemeColor value)
```


Imposta il colore del tema di primo piano.

**Remarks**

Se il colore di primo piano non è un colore di tema, NULL verrà restituito.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [ThemeColor](../../com.aspose.cells/themecolor) |  |

### setFormulaHidden(boolean value) {#setFormulaHidden-boolean-}
```
public void setFormulaHidden(boolean value)
```


Rappresenta se la formula sarà nascosta quando il foglio di lavoro è protetto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setGradient(boolean value) {#setGradient-boolean-}
```
public void setGradient(boolean value)
```


Indica se l'ombreggiatura della cella è un motivo gradiente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setHorizontalAlignment(int value) {#setHorizontalAlignment-int-}
```
public void setHorizontalAlignment(int value)
```


Imposta il tipo di allineamento orizzontale del testo in una cella.

Vedi [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setIndentLevel(int value) {#setIndentLevel-int-}
```
public void setIndentLevel(int value)
```


Rappresenta il livello di rientro per la cella o l'intervallo. Può essere solo un intero da 0 a 250.

**Remarks**

Se il tipo di allineamento orizzontale del testo è impostato su un valore diverso da sinistra o destra, il livello di rientro verrà reimpostato a zero.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setJustifyDistributed(boolean value) {#setJustifyDistributed-boolean-}
```
public void setJustifyDistributed(boolean value)
```


Indica se l'allineamento giustificato o distribuito delle celle dovrebbe essere usato sull'ultima riga di testo.

**Remarks**

Questo è tipico per gli allineamenti dell'Asia orientale ma non è tipico in altri contesti. Funziona solo quando l'allineamento orizzontale è distribuito.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


Imposta un valore che indica se una cella può essere modificata o meno.

**Remarks**

Bloccare le celle non ha effetto a meno che il foglio di lavoro non sia protetto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Imposta il nome dello stile.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setNumber(int value) {#setNumber-int-}
```
public void setNumber(int value)
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

### setNumberFormatApplied(boolean value) {#setNumberFormatApplied-boolean-}
```
public void setNumberFormatApplied(boolean value)
```


Indica se la formattazione dei numeri dovrebbe essere applicata.

**Remarks**

Solo per stile denominato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setOutlineBorders(int borderStyle, CellsColor borderColor) {#setOutlineBorders-int-com.aspose.cells.CellsColor-}
```
public void setOutlineBorders(int borderStyle, CellsColor borderColor)
```


Imposta i bordi di contorno

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). Il tipo di bordi. |
| borderColor | [CellsColor](../../com.aspose.cells/cellscolor) | Il colore dei bordi |

### setOutlineBorders(int borderStyle, Color borderColor) {#setOutlineBorders-int-com.aspose.cells.Color-}
```
public void setOutlineBorders(int borderStyle, Color borderColor)
```


Imposta i bordi di contorno

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| borderStyle | int | [CellBorderType](../../com.aspose.cells/cellbordertype). Il tipo di bordi. |
| borderColor | [Color](../../com.aspose.cells/color) | Il colore dei bordi |

### setPattern(int value) {#setPattern-int-}
```
public void setPattern(int value)
```


Imposta il tipo di motivo di sfondo della cella.

Vedi [BackgroundType](../../com.aspose.cells/backgroundtype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setPatternColor(int pattern, Color color1, Color color2) {#setPatternColor-int-com.aspose.cells.Color-com.aspose.cells.Color-}
```
public void setPatternColor(int pattern, Color color1, Color color2)
```


Imposta il colore di sfondo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pattern | int | [BackgroundType](../../com.aspose.cells/backgroundtype). Il modello. |
| color1 | [Color](../../com.aspose.cells/color) | Il colore di primo piano. |
| color2 | [Color](../../com.aspose.cells/color) | Il colore di sfondo. Funziona solo quando il modello non è BackgroundType.None e BackgroundType.Solid. |

### setProtectionApplied(boolean value) {#setProtectionApplied-boolean-}
```
public void setProtectionApplied(boolean value)
```


Indica se la formattazione di protezione dovrebbe essere applicata.

**Remarks**

Solo per stile denominato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setQuotePrefix(boolean value) {#setQuotePrefix-boolean-}
```
public void setQuotePrefix(boolean value)
```


Indica se il valore della cella inizia con un apice singolo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setRotationAngle(int value) {#setRotationAngle-int-}
```
public void setRotationAngle(int value)
```


Rappresenta l'angolo di rotazione del testo.

**Remarks**

0: Non ruotato.

255: Dall'alto verso il basso.

\-90: Verso il basso.

90: Verso l'alto.

È possibile impostare 255 o un valore compreso tra -90 e 90.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setShrinkToFit(boolean value) {#setShrinkToFit-boolean-}
```
public void setShrinkToFit(boolean value)
```


Rappresenta se il testo si riduce automaticamente per adattarsi alla larghezza di colonna disponibile.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setTextDirection(int value) {#setTextDirection-int-}
```
public void setTextDirection(int value)
```


Rappresenta l'ordine di lettura del testo.

Vedi [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setTextWrapped(boolean value) {#setTextWrapped-boolean-}
```
public void setTextWrapped(boolean value)
```


Imposta un valore che indica se il testo all'interno di una cella è a capo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setTwoColorGradient(Color color1, Color color2, int gradientStyleType, int variant) {#setTwoColorGradient-com.aspose.cells.Color-com.aspose.cells.Color-int-int-}
```
public void setTwoColorGradient(Color color1, Color color2, int gradientStyleType, int variant)
```


Imposta il riempimento specificato a un gradiente a due colori.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| color1 | [Color](../../com.aspose.cells/color) | Un colore di gradiente. |
| color2 | [Color](../../com.aspose.cells/color) | Due colori del gradiente. |
| gradientStyleType | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). Stile di sfumatura del gradiente. |
| variante | int | La variante del gradiente. Può essere un valore da 1 a 4, corrispondente a una delle quattro varianti nella scheda Gradiente nella finestra di dialogo Effetti di riempimento. Se lo stile è GradientStyle.FromCenter, l'argomento Variant può essere solo 1 o 2. |

### setVerticalAlignment(int value) {#setVerticalAlignment-int-}
```
public void setVerticalAlignment(int value)
```


Imposta il tipo di allineamento verticale del testo in una cella.

Vedi [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### toJson() {#toJson--}
```
public String toJson()
```


Converti [Style](../../com.aspose.cells/style) in dati struct JSON.

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


Applica lo stile denominato agli stili delle celle che utilizzano questo stile denominato. Funziona come fare clic sul pulsante \"ok\" dopo aver terminato la modifica dello stile. Si applica solo agli stili denominati.

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

