---
title: "GridCell"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta un oggetto cella."
type: docs
url: /it/java/com.aspose.gridweb/gridcell/
---

**Inheritance:**
java.lang.Object
```
public class GridCell
```

Rappresenta un oggetto cella.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [containsExternalLink()](#containsExternalLink--) | Indica se questa cella contiene un collegamento esterno. |
| [copy(GridCell source)](#copy-com.aspose.gridweb.GridCell-) | Copia i dati da una cella di origine. |
| [copyStyle(GridTableItemStyle style)](#copyStyle-com.aspose.gridweb.GridTableItemStyle-) | copia lo stile e imposta lo stile per la cella |
| [createComment(String note, String author, boolean isvisible)](#createComment-java.lang.String-java.lang.String-boolean-) | Crea un oggetto commento per una cella. |
| [createValidation(int validationType, boolean isRequried)](#createValidation-int-boolean-) | Crea un oggetto di convalida per una cella. |
| [equals(Object obj)](#equals-java.lang.Object-) | Verifica se questo oggetto si riferisce alla stessa cella di un altro oggetto cella. |
| [getBoolValue()](#getBoolValue--) | Ottiene il valore booleano contenuto nella cella. |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | Ottiene il numero della colonna (basato su zero) della cella. |
| [getComment()](#getComment--) | Ottieni l'oggetto commento su questa cella |
| [getDateValue()](#getDateValue--) | Ottiene il valore DateTime contenuto nella cella. |
| [getDisplayStringValue()](#getDisplayStringValue--) | Ottiene il valore stringa formattato di questa cella. |
| [getDoubleValue()](#getDoubleValue--) | Ottiene il valore double contenuto nella cella. |
| [getFloatValue()](#getFloatValue--) | Ottiene il valore float contenuto nella cella. |
| [getFormula()](#getFormula--) | Ottiene una formula della [GridCell](../../com.aspose.gridweb/gridcell). |
| [getHtmlString()](#getHtmlString--) | Ottiene la stringa HTML che contiene dati e alcune formattazioni in questa cella. |
| [getIntValue()](#getIntValue--) | Restituisce il valore intero contenuto nella cella. |
| [getName()](#getName--) | Restituisce il nome della cella. |
| [getRow()](#getRow--) | Restituisce il numero di riga (basato su zero) della cella. |
| [getStringValue()](#getStringValue--) | Restituisce il valore stringa contenuto nella cella. |
| [getStyle()](#getStyle--) | Ottiene la copia dello stile della cella. imposta lo stile per la cella. |
| [getType()](#getType--) | restituisce il tipo di valore della cella, il significato può essere visto in GridCellValueType.java |
| [getValue()](#getValue--) | Restituisce il valore contenuto in questa cella. |
| [getWidthOfValue()](#getWidthOfValue--) | Restituisce la larghezza del valore in unità di pixel. |
| [hashCode()](#hashCode--) | Funziona come funzione hash per un tipo specifico. |
| [isErrorValue()](#isErrorValue--) | Verifica se una formula può valutare correttamente un risultato. |
| [isFormula()](#isFormula--) | Rappresenta se la cella specificata contiene una formula. |
| [isStyleSet()](#isStyleSet--) | Indica se lo stile della cella è impostato. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [putValue(boolean param_boolean)](#putValue-boolean-) | Inserisce un valore booleano nella cella. |
| [putValue(DateTime param_date)](#putValue-com.aspose.gridweb.DateTime-) | Inserisce un valore DateTime nella cella. |
| [putValue(double param_double)](#putValue-double-) | Inserisce un valore double nella cella. |
| [putValue(int param_int)](#putValue-int-) | Inserisce un valore intero nella cella. |
| [putValue(Object objectValue)](#putValue-java.lang.Object-) | Inserisce un valore oggetto nella cella. stesso di setValue(Object param\_object) |
| [putValue(String param_string)](#putValue-java.lang.String-) | Inserisce un valore String nella cella. |
| [putValue(String stringValue, boolean isConverted)](#putValue-java.lang.String-boolean-) | Inserisce un valore stringa nella cella e converte il valore in un altro tipo di dati, se appropriato. |
| [putValue(String stringValue, boolean isConverted, boolean setStyle)](#putValue-java.lang.String-boolean-boolean-) | Inserisce un valore nella cella; se opportuno il valore verrà convertito in un altro tipo di dato e il formato numerico della cella verrà ripristinato. |
| [putValueAndSetFormatByValue(String stringValue)](#putValueAndSetFormatByValue-java.lang.String-) | Imposta il valore della cella con un valore stringa e imposta il formato della cella in base a questo valore. |
| [removeComment()](#removeComment--) | Rimuove l'oggetto commento della cella. |
| [removeValidation()](#removeValidation--) | Rimuove l'oggetto di convalida della cella. |
| [setBorder(WebBorderStyle borderStyle)](#setBorder-com.aspose.gridweb.WebBorderStyle-) | Imposta i bordi (superiore, inferiore, sinistro e destro) per una cella, tutti i bordi hanno lo stesso stile di bordo. |
| [setCustom(String custom)](#setCustom-java.lang.String-) | imposta il formato personalizzato, null o stringa vuota significa nessun formato personalizzato. |
| [setFormula(String value)](#setFormula-java.lang.String-) | Imposta una formula della [GridCell](../../com.aspose.gridweb/gridcell). |
| [setFormula(String formula, Object value)](#setFormula-java.lang.String-java.lang.Object-) | Imposta la formula e il valore della formula. |
| [setHtmlString(String value)](#setHtmlString-java.lang.String-) | Imposta la stringa HTML che contiene dati e alcune formattazioni in questa cella. |
| [setNumberType(int numbertype)](#setNumberType-int-) | imposta il formato di visualizzazione di numeri e date |
| [setStyle(GridTableItemStyle value)](#setStyle-com.aspose.gridweb.GridTableItemStyle-) | Ottiene la copia dello stile della cella. imposta lo stile per la cella. |
| [setValue(Object value)](#setValue-java.lang.Object-) | Restituisce il valore contenuto in questa cella. |
| [toString()](#toString--) | Restituisce una stringa che rappresenta l'oggetto Cell corrente. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### containsExternalLink() {#containsExternalLink--}
```
public boolean containsExternalLink()
```


Indica se questa cella contiene un collegamento esterno. Si applica solo quando la cella è una cella formula.

**Returns:**
boolean
### copy(GridCell source) {#copy-com.aspose.gridweb.GridCell-}
```
public void copy(GridCell source)
```


Copia i dati da una cella di origine.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| source | [GridCell](../../com.aspose.gridweb/gridcell) | Oggetto sorgente [GridCell](../../com.aspose.gridweb/gridcell). |

### copyStyle(GridTableItemStyle style) {#copyStyle-com.aspose.gridweb.GridTableItemStyle-}
```
public void copyStyle(GridTableItemStyle style)
```


copia lo stile e imposta lo stile per la cella

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| style | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) | Lo stile di origine. |

### createComment(String note, String author, boolean isvisible) {#createComment-java.lang.String-java.lang.String-boolean-}
```
public GridComment createComment(String note, String author, boolean isvisible)
```


Crea un oggetto commento per una cella.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| nota | java.lang.String | nota commento. |
| autore | java.lang.String | autore del commento. |
| isvisible | boolean | se il commento è visibile. |

**Returns:**
[GridComment](../../com.aspose.gridweb/gridcomment) - GridComment object
### createValidation(int validationType, boolean isRequried) {#createValidation-int-boolean-}
```
public GridValidation createValidation(int validationType, boolean isRequried)
```


Crea un oggetto di convalida per una cella.

**Example**

```
         GridWeb GridWeb1 = new GridWeb();
         GridWorksheet sheet = GridWeb1.getActiveSheet();
         GridValidation v = sheet.getCells().get("A1").createValidation(GridValidationType.CUSTOM_EXPRESSION, true);
         		// Sets to number validation expression.
         		v.setRegEx("\\d+");
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| validationType | int | [GridValidationType](../../com.aspose.gridweb/gridvalidationtype). Tipo di convalida. |
| isRequried | boolean | Se il valore della cella è obbligatorio. |

**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation) - 
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Verifica se questo oggetto si riferisce alla stessa cella di un altro oggetto cella.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| obj | java.lang.Object | un altro oggetto GridCell |

**Returns:**
boolean - true se due oggetti cella si riferiscono alla stessa cella.
### getBoolValue() {#getBoolValue--}
```
public boolean getBoolValue()
```


Ottiene il valore booleano contenuto nella cella.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumn() {#getColumn--}
```
public int getColumn()
```


Ottiene il numero della colonna (basato su zero) della cella.

**Returns:**
int
### getComment() {#getComment--}
```
public GridComment getComment()
```


Ottieni l'oggetto commento su questa cella

**Returns:**
[GridComment](../../com.aspose.gridweb/gridcomment)
### getDateValue() {#getDateValue--}
```
public DateTime getDateValue()
```


Ottiene il valore DateTime contenuto nella cella.

**Returns:**
[DateTime](../../com.aspose.gridweb/datetime)
### getDisplayStringValue() {#getDisplayStringValue--}
```
public String getDisplayStringValue()
```


Ottiene il valore stringa formattato di questa cella.

**Returns:**
java.lang.String
### getDoubleValue() {#getDoubleValue--}
```
public double getDoubleValue()
```


Ottiene il valore double contenuto nella cella.

**Returns:**
double
### getFloatValue() {#getFloatValue--}
```
public float getFloatValue()
```


Ottiene il valore float contenuto nella cella.

**Returns:**
float
### getFormula() {#getFormula--}
```
public String getFormula()
```


Ottiene una formula della [GridCell](../../com.aspose.gridweb/gridcell).

**Remarks**

Una stringa di formula inizia sempre con il segno uguale (=). E si prega di utilizzare sempre la virgola (,) come delimitatore dei parametri, ad esempio "=SUM(A1, E1, H2)".

L'utente può impostare qualsiasi formula nel file del designer di Workbook. Aspose.Cells manterrà tutte le formule. Se l'utente utilizza questa proprietà per impostare una formula in una cella, è supportata la maggior parte delle funzioni integrate di Workbook. E ne arriveranno altre. Se hai esigenze particolari per le funzioni integrate di Workbook, faccelo sapere.

**Example**

```
         GridWeb GridWeb1 = new GridWeb();
         GridWorksheet sheet = GridWeb1.getActiveSheet();
         sheet.getCells().get("B6").setFormula("=SUM(B2:B5, E1) + sheet1!A1");
```

**Returns:**
java.lang.String
### getHtmlString() {#getHtmlString--}
```
public String getHtmlString()
```


Ottiene la stringa HTML che contiene dati e alcune formattazioni in questa cella.

**Returns:**
java.lang.String
### getIntValue() {#getIntValue--}
```
public int getIntValue()
```


Restituisce il valore intero contenuto nella cella.

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


Restituisce il nome della cella. Per esempio: A1, F102.

**Returns:**
java.lang.String
### getRow() {#getRow--}
```
public int getRow()
```


Restituisce il numero di riga (basato su zero) della cella.

**Returns:**
int
### getStringValue() {#getStringValue--}
```
public String getStringValue()
```


Restituisce il valore stringa contenuto nella cella.

**Returns:**
java.lang.String
### getStyle() {#getStyle--}
```
public GridTableItemStyle getStyle()
```


Ottiene la copia dello stile della cella. imposta lo stile per la cella.

**Returns:**
[GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) - Style object.
### getType() {#getType--}
```
public int getType()
```


restituisce il tipo di valore della cella, il significato può essere visto in GridCellValueType.java

**Returns:**
int
### getValue() {#getValue--}
```
public Object getValue()
```


Restituisce il valore contenuto in questa cella.

**Remarks**

Tipo possibile:

null,

Boolean,

DateTime,

Double,

Integer

String.

**Returns:**
java.lang.Object
### getWidthOfValue() {#getWidthOfValue--}
```
public int getWidthOfValue()
```


Restituisce la larghezza del valore in unità di pixel.

**Returns:**
int -
### hashCode() {#hashCode--}
```
public int hashCode()
```


Funziona come funzione hash per un tipo specifico.

**Returns:**
int - Un codice hash per l'oggetto GridCell corrente.
### isErrorValue() {#isErrorValue--}
```
public boolean isErrorValue()
```


Verifica se una formula può valutare correttamente un risultato.

**Remarks**

Si applica solo alle celle di formula.

**Returns:**
boolean
### isFormula() {#isFormula--}
```
public boolean isFormula()
```


Rappresenta se la cella specificata contiene una formula.

**Returns:**
boolean
### isStyleSet() {#isStyleSet--}
```
public boolean isStyleSet()
```


Indica se lo stile della cella è impostato. Se restituisce false, significa che questa cella ha un formato di cella predefinito.

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




### putValue(boolean param_boolean) {#putValue-boolean-}
```
public void putValue(boolean param_boolean)
```


Inserisce un valore booleano nella cella.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| param_boolean | boolean | Valore di input |

### putValue(DateTime param_date) {#putValue-com.aspose.gridweb.DateTime-}
```
public void putValue(DateTime param_date)
```


Inserisce un valore DateTime nella cella.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| param_date | [DateTime](../../com.aspose.gridweb/datetime) | Valore di input |

### putValue(double param_double) {#putValue-double-}
```
public void putValue(double param_double)
```


Inserisce un valore double nella cella.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| param_double | double | Valore di input |

### putValue(int param_int) {#putValue-int-}
```
public void putValue(int param_int)
```


Inserisce un valore intero nella cella.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| param_int | int | Valore di input |

### putValue(Object objectValue) {#putValue-java.lang.Object-}
```
public void putValue(Object objectValue)
```


Inserisce un valore oggetto nella cella. stesso di setValue(Object param\_object)

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| objectValue | java.lang.Object | valore di input |

### putValue(String param_string) {#putValue-java.lang.String-}
```
public void putValue(String param_string)
```


Inserisce un valore String nella cella.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| param_string | java.lang.String | Valore di input |

### putValue(String stringValue, boolean isConverted) {#putValue-java.lang.String-boolean-}
```
public void putValue(String stringValue, boolean isConverted)
```


Inserisce un valore stringa nella cella e converte il valore in un altro tipo di dati, se appropriato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stringValue | java.lang.String | Valore di input |
| isConverted | boolean | True: convertito in un altro tipo di dato se appropriato. |

### putValue(String stringValue, boolean isConverted, boolean setStyle) {#putValue-java.lang.String-boolean-boolean-}
```
public void putValue(String stringValue, boolean isConverted, boolean setStyle)
```


Inserisce un valore nella cella; se opportuno il valore verrà convertito in un altro tipo di dato e il formato numerico della cella verrà ripristinato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stringValue | java.lang.String | Valore di input |
| isConverted | boolean | True: convertito in un altro tipo di dato se appropriato. |
| setStyle | boolean | True: imposta il formato numerico nello stile della cella durante la conversione in un altro tipo di dato |

### putValueAndSetFormatByValue(String stringValue) {#putValueAndSetFormatByValue-java.lang.String-}
```
public void putValueAndSetFormatByValue(String stringValue)
```


Imposta il valore della cella con un valore stringa e imposta il formato della cella in base a questo valore.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stringValue | java.lang.String | Valore di input. |

### removeComment() {#removeComment--}
```
public void removeComment()
```


Rimuove l'oggetto commento della cella.

### removeValidation() {#removeValidation--}
```
public void removeValidation()
```


Rimuove l'oggetto di convalida della cella.

### setBorder(WebBorderStyle borderStyle) {#setBorder-com.aspose.gridweb.WebBorderStyle-}
```
public void setBorder(WebBorderStyle borderStyle)
```


Imposta i bordi (superiore, inferiore, sinistro e destro) per una cella, tutti i bordi hanno lo stesso stile di bordo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| borderStyle | [WebBorderStyle](../../com.aspose.gridweb/webborderstyle) | Lo stile del bordo. |

### setCustom(String custom) {#setCustom-java.lang.String-}
```
public void setCustom(String custom)
```


imposta il formato personalizzato, null o stringa vuota significa nessun formato personalizzato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| personalizzato | java.lang.String | la presentazione della stringa personalizzata |

### setFormula(String value) {#setFormula-java.lang.String-}
```
public void setFormula(String value)
```


Imposta una formula della [GridCell](../../com.aspose.gridweb/gridcell).

**Remarks**

Una stringa di formula inizia sempre con il segno uguale (=). E si prega di utilizzare sempre la virgola (,) come delimitatore dei parametri, ad esempio "=SUM(A1, E1, H2)".

L'utente può impostare qualsiasi formula nel file del designer di Workbook. Aspose.Cells manterrà tutte le formule. Se l'utente utilizza questa proprietà per impostare una formula in una cella, è supportata la maggior parte delle funzioni integrate di Workbook. E ne arriveranno altre. Se hai esigenze particolari per le funzioni integrate di Workbook, faccelo sapere.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setFormula(String formula, Object value) {#setFormula-java.lang.String-java.lang.Object-}
```
public void setFormula(String formula, Object value)
```


Imposta la formula e il valore della formula.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| formula | java.lang.String | La formula. |
| valore | java.lang.Object | Il valore della formula. |

### setHtmlString(String value) {#setHtmlString-java.lang.String-}
```
public void setHtmlString(String value)
```


Imposta la stringa HTML che contiene dati e alcune formattazioni in questa cella.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setNumberType(int numbertype) {#setNumberType-int-}
```
public void setNumberType(int numbertype)
```


imposta il formato di visualizzazione di numeri e date

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| numbertype | int | il valore del numbertype, vedi GridTableItemStyle.NumberType |

### setStyle(GridTableItemStyle value) {#setStyle-com.aspose.gridweb.GridTableItemStyle-}
```
public void setStyle(GridTableItemStyle value)
```


Ottiene la copia dello stile della cella. imposta lo stile per la cella.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) |  |

### setValue(Object value) {#setValue-java.lang.Object-}
```
public void setValue(Object value)
```


Restituisce il valore contenuto in questa cella.

**Remarks**

Tipo possibile:

null,

Boolean,

DateTime,

Double,

Integer

String.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.Object |  |

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

