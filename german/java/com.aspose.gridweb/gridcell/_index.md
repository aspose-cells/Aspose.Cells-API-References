---
title: "GridCell"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt ein Zellenobjekt dar."
type: docs
url: /de/java/com.aspose.gridweb/gridcell/
---

**Inheritance:**
java.lang.Object
```
public class GridCell
```

Stellt ein Zellenobjekt dar.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [containsExternalLink()](#containsExternalLink--) | Gibt an, ob diese Zelle einen externen Link enthält. |
| [copy(GridCell source)](#copy-com.aspose.gridweb.GridCell-) | Kopiert Daten aus einer Quellzelle. |
| [copyStyle(GridTableItemStyle style)](#copyStyle-com.aspose.gridweb.GridTableItemStyle-) | Kopiere den Stil und setze den Stil für die Zelle. |
| [createComment(String note, String author, boolean isvisible)](#createComment-java.lang.String-java.lang.String-boolean-) | Erstellt ein Kommentarobjekt für eine Zelle. |
| [createValidation(int validationType, boolean isRequried)](#createValidation-int-boolean-) | Erstellt ein Validierungsobjekt für eine Zelle. |
| [equals(Object obj)](#equals-java.lang.Object-) | Prüft, ob dieses Objekt sich auf dieselbe Zelle wie ein anderes Zellenobjekt bezieht. |
| [getBoolValue()](#getBoolValue--) | Ermittelt den booleschen Wert, der in der Zelle enthalten ist. |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | Ermittelt die Spaltennummer (nullbasiert) der Zelle. |
| [getComment()](#getComment--) | Hole das Kommentarobjekt dieser Zelle. |
| [getDateValue()](#getDateValue--) | Ermittelt den DateTime-Wert, der in der Zelle enthalten ist. |
| [getDisplayStringValue()](#getDisplayStringValue--) | Liefert den formatierten Zeichenkettenwert dieser Zelle. |
| [getDoubleValue()](#getDoubleValue--) | Ermittelt den Double-Wert, der in der Zelle enthalten ist. |
| [getFloatValue()](#getFloatValue--) | Ermittelt den Float-Wert, der in der Zelle enthalten ist. |
| [getFormula()](#getFormula--) | Liefert eine Formel des [GridCell](../../com.aspose.gridweb/gridcell). |
| [getHtmlString()](#getHtmlString--) | Liefert die HTML-Zeichenkette, die Daten und einige Formatierungen in dieser Zelle enthält. |
| [getIntValue()](#getIntValue--) | Ermittelt den Integer-Wert, der in der Zelle enthalten ist. |
| [getName()](#getName--) | Liefert den Namen der Zelle. |
| [getRow()](#getRow--) | Ruft die Zeilennummer (nullbasiert) der Zelle ab. |
| [getStringValue()](#getStringValue--) | Ruft den Zeichenkettenwert ab, der in der Zelle enthalten ist. |
| [getStyle()](#getStyle--) | Liefert eine Kopie des Zellenstils. Setze den Stil für die Zelle. |
| [getType()](#getType--) | Gibt den Zellenwerttyp zurück, die Bedeutung kann in GridCellValueType.java nachgelesen werden. |
| [getValue()](#getValue--) | Ruft den in dieser Zelle enthaltenen Wert ab. |
| [getWidthOfValue()](#getWidthOfValue--) | Ruft die Breite des Wertes in Pixeln ab. |
| [hashCode()](#hashCode--) | Dient als Hash-Funktion für einen bestimmten Typ. |
| [isErrorValue()](#isErrorValue--) | Prüft, ob eine Formel ein Ergebnis korrekt auswerten kann. |
| [isFormula()](#isFormula--) | Gibt an, ob die angegebene Zelle eine Formel enthält. |
| [isStyleSet()](#isStyleSet--) | Gibt an, ob der Stil der Zelle festgelegt ist. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [putValue(boolean param_boolean)](#putValue-boolean-) | Schreibt einen booleschen Wert in die Zelle. |
| [putValue(DateTime param_date)](#putValue-com.aspose.gridweb.DateTime-) | Schreibt einen DateTime-Wert in die Zelle. |
| [putValue(double param_double)](#putValue-double-) | Schreibt einen double-Wert in die Zelle. |
| [putValue(int param_int)](#putValue-int-) | Setzt einen int-Wert in die Zelle. |
| [putValue(Object objectValue)](#putValue-java.lang.Object-) | Setzt einen Objektwert in die Zelle, gleich wie setValue(Object param\_object). |
| [putValue(String param_string)](#putValue-java.lang.String-) | Setzt einen String-Wert in die Zelle. |
| [putValue(String stringValue, boolean isConverted)](#putValue-java.lang.String-boolean-) | Schreibt einen Zeichenkettenwert in die Zelle und konvertiert den Wert bei Bedarf in einen anderen Datentyp. |
| [putValue(String stringValue, boolean isConverted, boolean setStyle)](#putValue-java.lang.String-boolean-boolean-) | Schreibt einen Wert in die Zelle; bei Bedarf wird der Wert in einen anderen Datentyp konvertiert und das Zahlenformat der Zelle zurückgesetzt. |
| [putValueAndSetFormatByValue(String stringValue)](#putValueAndSetFormatByValue-java.lang.String-) | Setzt den Zellenwert mit einem String-Wert und legt das Zellenformat anhand dieses Wertes fest. |
| [removeComment()](#removeComment--) | Entfernt das Kommentarobjekt der Zelle. |
| [removeValidation()](#removeValidation--) | Entfernt das Validierungsobjekt der Zelle. |
| [setBorder(WebBorderStyle borderStyle)](#setBorder-com.aspose.gridweb.WebBorderStyle-) | Setzt Rahmen (oben, unten, links und rechts) für eine Zelle, alle Rahmen haben denselben Rahmenstil. |
| [setCustom(String custom)](#setCustom-java.lang.String-) | Setzt das benutzerdefinierte Format, null oder leere Zeichenkette bedeutet kein benutzerdefiniertes Format. |
| [setFormula(String value)](#setFormula-java.lang.String-) | Setzt eine Formel des [GridCell](../../com.aspose.gridweb/gridcell). |
| [setFormula(String formula, Object value)](#setFormula-java.lang.String-java.lang.Object-) | Setze die Formel und den Wert der Formel. |
| [setHtmlString(String value)](#setHtmlString-java.lang.String-) | Setzt die HTML-Zeichenkette, die Daten und einige Formatierungen in dieser Zelle enthält. |
| [setNumberType(int numbertype)](#setNumberType-int-) | Lege das Anzeigeformat von Zahlen und Daten fest |
| [setStyle(GridTableItemStyle value)](#setStyle-com.aspose.gridweb.GridTableItemStyle-) | Liefert eine Kopie des Zellenstils. Setze den Stil für die Zelle. |
| [setValue(Object value)](#setValue-java.lang.Object-) | Ruft den in dieser Zelle enthaltenen Wert ab. |
| [toString()](#toString--) | Gibt eine Zeichenkette zurück, die das aktuelle Cell-Objekt darstellt. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### containsExternalLink() {#containsExternalLink--}
```
public boolean containsExternalLink()
```


Gibt an, ob diese Zelle einen externen Link enthält. Gilt nur, wenn die Zelle eine Formelzelle ist.

**Returns:**
boolean
### copy(GridCell source) {#copy-com.aspose.gridweb.GridCell-}
```
public void copy(GridCell source)
```


Kopiert Daten aus einer Quellzelle.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| source | [GridCell](../../com.aspose.gridweb/gridcell) | Quelle [GridCell](../../com.aspose.gridweb/gridcell) Objekt. |

### copyStyle(GridTableItemStyle style) {#copyStyle-com.aspose.gridweb.GridTableItemStyle-}
```
public void copyStyle(GridTableItemStyle style)
```


Kopiere den Stil und setze den Stil für die Zelle.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| style | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) | Der Quellstil. |

### createComment(String note, String author, boolean isvisible) {#createComment-java.lang.String-java.lang.String-boolean-}
```
public GridComment createComment(String note, String author, boolean isvisible)
```


Erstellt ein Kommentarobjekt für eine Zelle.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Hinweis | java.lang.String | Kommentarhinweis. |
| Autor | java.lang.String | Kommentarautor. |
| isvisible | boolean | ob der Kommentar sichtbar ist. |

**Returns:**
[GridComment](../../com.aspose.gridweb/gridcomment) - GridComment object
### createValidation(int validationType, boolean isRequried) {#createValidation-int-boolean-}
```
public GridValidation createValidation(int validationType, boolean isRequried)
```


Erstellt ein Validierungsobjekt für eine Zelle.

**Example**

```
         GridWeb GridWeb1 = new GridWeb();
         GridWorksheet sheet = GridWeb1.getActiveSheet();
         GridValidation v = sheet.getCells().get("A1").createValidation(GridValidationType.CUSTOM_EXPRESSION, true);
         		// Sets to number validation expression.
         		v.setRegEx("\\d+");
```

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| validationType | int | [GridValidationType](../../com.aspose.gridweb/gridvalidationtype). Validierungstyp. |
| isRequried | boolean | Ob der Zellenwert erforderlich ist. |

**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation) - 
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Prüft, ob dieses Objekt sich auf dieselbe Zelle wie ein anderes Zellenobjekt bezieht.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| obj | java.lang.Object | ein weiteres GridCell-Objekt |

**Returns:**
boolean - true, wenn zwei Zellenobjekte auf dieselbe Zelle verweisen.
### getBoolValue() {#getBoolValue--}
```
public boolean getBoolValue()
```


Ermittelt den booleschen Wert, der in der Zelle enthalten ist.

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


Ermittelt die Spaltennummer (nullbasiert) der Zelle.

**Returns:**
int
### getComment() {#getComment--}
```
public GridComment getComment()
```


Hole das Kommentarobjekt dieser Zelle.

**Returns:**
[GridComment](../../com.aspose.gridweb/gridcomment)
### getDateValue() {#getDateValue--}
```
public DateTime getDateValue()
```


Ermittelt den DateTime-Wert, der in der Zelle enthalten ist.

**Returns:**
[DateTime](../../com.aspose.gridweb/datetime)
### getDisplayStringValue() {#getDisplayStringValue--}
```
public String getDisplayStringValue()
```


Liefert den formatierten Zeichenkettenwert dieser Zelle.

**Returns:**
java.lang.String
### getDoubleValue() {#getDoubleValue--}
```
public double getDoubleValue()
```


Ermittelt den Double-Wert, der in der Zelle enthalten ist.

**Returns:**
double
### getFloatValue() {#getFloatValue--}
```
public float getFloatValue()
```


Ermittelt den Float-Wert, der in der Zelle enthalten ist.

**Returns:**
float
### getFormula() {#getFormula--}
```
public String getFormula()
```


Liefert eine Formel des [GridCell](../../com.aspose.gridweb/gridcell).

**Remarks**

Eine Formelzeichenkette beginnt immer mit einem Gleichheitszeichen (=). Und bitte verwenden Sie immer ein Komma (,) als Parametertrennzeichen, zum Beispiel "=SUM(A1, E1, H2)".

Der Benutzer kann jede Formel in der Workbook-Designer-Datei festlegen. Aspose.Cells behält alle Formeln bei. Wenn der Benutzer diese Eigenschaft verwendet, um einer Zelle eine Formel zuzuweisen, wird ein großer Teil der integrierten Workbook-Funktionen unterstützt. Und es kommt noch mehr. Wenn Sie spezielle Anforderungen an die integrierten Workbook-Funktionen haben, lassen Sie es uns bitte wissen.

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


Liefert die HTML-Zeichenkette, die Daten und einige Formatierungen in dieser Zelle enthält.

**Returns:**
java.lang.String
### getIntValue() {#getIntValue--}
```
public int getIntValue()
```


Ermittelt den Integer-Wert, der in der Zelle enthalten ist.

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


Liefert den Namen der Zelle. Zum Beispiel: A1, F102.

**Returns:**
java.lang.String
### getRow() {#getRow--}
```
public int getRow()
```


Ruft die Zeilennummer (nullbasiert) der Zelle ab.

**Returns:**
int
### getStringValue() {#getStringValue--}
```
public String getStringValue()
```


Ruft den Zeichenkettenwert ab, der in der Zelle enthalten ist.

**Returns:**
java.lang.String
### getStyle() {#getStyle--}
```
public GridTableItemStyle getStyle()
```


Liefert eine Kopie des Zellenstils. Setze den Stil für die Zelle.

**Returns:**
[GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) - Style object.
### getType() {#getType--}
```
public int getType()
```


Gibt den Zellenwerttyp zurück, die Bedeutung kann in GridCellValueType.java nachgelesen werden.

**Returns:**
int
### getValue() {#getValue--}
```
public Object getValue()
```


Ruft den in dieser Zelle enthaltenen Wert ab.

**Remarks**

Möglicher Typ:

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


Ruft die Breite des Wertes in Pixeln ab.

**Returns:**
int -
### hashCode() {#hashCode--}
```
public int hashCode()
```


Dient als Hash-Funktion für einen bestimmten Typ.

**Returns:**
int – Ein Hashcode für das aktuelle GridCell-Objekt.
### isErrorValue() {#isErrorValue--}
```
public boolean isErrorValue()
```


Prüft, ob eine Formel ein Ergebnis korrekt auswerten kann.

**Remarks**

Gilt nur für Formelzellen.

**Returns:**
boolean
### isFormula() {#isFormula--}
```
public boolean isFormula()
```


Gibt an, ob die angegebene Zelle eine Formel enthält.

**Returns:**
boolean
### isStyleSet() {#isStyleSet--}
```
public boolean isStyleSet()
```


Gibt an, ob der Stil der Zelle gesetzt ist. Wenn false zurückgegeben wird, bedeutet dies, dass diese Zelle ein Standardzellenformat hat.

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


Schreibt einen booleschen Wert in die Zelle.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| param_boolean | boolean | Eingabewert |

### putValue(DateTime param_date) {#putValue-com.aspose.gridweb.DateTime-}
```
public void putValue(DateTime param_date)
```


Schreibt einen DateTime-Wert in die Zelle.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| param_date | [DateTime](../../com.aspose.gridweb/datetime) | Eingabewert |

### putValue(double param_double) {#putValue-double-}
```
public void putValue(double param_double)
```


Schreibt einen double-Wert in die Zelle.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| param_double | double | Eingabewert |

### putValue(int param_int) {#putValue-int-}
```
public void putValue(int param_int)
```


Setzt einen int-Wert in die Zelle.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| param_int | int | Eingabewert |

### putValue(Object objectValue) {#putValue-java.lang.Object-}
```
public void putValue(Object objectValue)
```


Setzt einen Objektwert in die Zelle, gleich wie setValue(Object param\_object).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| objectValue | java.lang.Object | Eingabewert |

### putValue(String param_string) {#putValue-java.lang.String-}
```
public void putValue(String param_string)
```


Setzt einen String-Wert in die Zelle.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| param_string | java.lang.String | Eingabewert |

### putValue(String stringValue, boolean isConverted) {#putValue-java.lang.String-boolean-}
```
public void putValue(String stringValue, boolean isConverted)
```


Schreibt einen Zeichenkettenwert in die Zelle und konvertiert den Wert bei Bedarf in einen anderen Datentyp.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stringValue | java.lang.String | Eingabewert |
| isConverted | boolean | True: in einen anderen Datentyp konvertiert, falls zutreffend. |

### putValue(String stringValue, boolean isConverted, boolean setStyle) {#putValue-java.lang.String-boolean-boolean-}
```
public void putValue(String stringValue, boolean isConverted, boolean setStyle)
```


Schreibt einen Wert in die Zelle; bei Bedarf wird der Wert in einen anderen Datentyp konvertiert und das Zahlenformat der Zelle zurückgesetzt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stringValue | java.lang.String | Eingabewert |
| isConverted | boolean | True: in einen anderen Datentyp konvertiert, falls zutreffend. |
| setStyle | boolean | True: das Zahlenformat auf den Zellenstil setzen, wenn in einen anderen Datentyp konvertiert wird |

### putValueAndSetFormatByValue(String stringValue) {#putValueAndSetFormatByValue-java.lang.String-}
```
public void putValueAndSetFormatByValue(String stringValue)
```


Setzt den Zellenwert mit einem String-Wert und legt das Zellenformat anhand dieses Wertes fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stringValue | java.lang.String | Eingabewert. |

### removeComment() {#removeComment--}
```
public void removeComment()
```


Entfernt das Kommentarobjekt der Zelle.

### removeValidation() {#removeValidation--}
```
public void removeValidation()
```


Entfernt das Validierungsobjekt der Zelle.

### setBorder(WebBorderStyle borderStyle) {#setBorder-com.aspose.gridweb.WebBorderStyle-}
```
public void setBorder(WebBorderStyle borderStyle)
```


Setzt Rahmen (oben, unten, links und rechts) für eine Zelle, alle Rahmen haben denselben Rahmenstil.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| borderStyle | [WebBorderStyle](../../com.aspose.gridweb/webborderstyle) | Der Randstil. |

### setCustom(String custom) {#setCustom-java.lang.String-}
```
public void setCustom(String custom)
```


Setzt das benutzerdefinierte Format, null oder leere Zeichenkette bedeutet kein benutzerdefiniertes Format.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| benutzerdefiniert | java.lang.String | die benutzerdefinierte Zeichenkettenpräsentation |

### setFormula(String value) {#setFormula-java.lang.String-}
```
public void setFormula(String value)
```


Setzt eine Formel des [GridCell](../../com.aspose.gridweb/gridcell).

**Remarks**

Eine Formelzeichenkette beginnt immer mit einem Gleichheitszeichen (=). Und bitte verwenden Sie immer ein Komma (,) als Parametertrennzeichen, zum Beispiel "=SUM(A1, E1, H2)".

Der Benutzer kann jede Formel in der Workbook-Designer-Datei festlegen. Aspose.Cells behält alle Formeln bei. Wenn der Benutzer diese Eigenschaft verwendet, um einer Zelle eine Formel zuzuweisen, wird ein großer Teil der integrierten Workbook-Funktionen unterstützt. Und es kommt noch mehr. Wenn Sie spezielle Anforderungen an die integrierten Workbook-Funktionen haben, lassen Sie es uns bitte wissen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setFormula(String formula, Object value) {#setFormula-java.lang.String-java.lang.Object-}
```
public void setFormula(String formula, Object value)
```


Setze die Formel und den Wert der Formel.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| formula | java.lang.String | Die Formel. |
| Wert | java.lang.Object | Der Wert der Formel. |

### setHtmlString(String value) {#setHtmlString-java.lang.String-}
```
public void setHtmlString(String value)
```


Setzt die HTML-Zeichenkette, die Daten und einige Formatierungen in dieser Zelle enthält.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setNumberType(int numbertype) {#setNumberType-int-}
```
public void setNumberType(int numbertype)
```


Lege das Anzeigeformat von Zahlen und Daten fest

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| numbertype | int | der Wert des NumberType, siehe GridTableItemStyle.NumberType |

### setStyle(GridTableItemStyle value) {#setStyle-com.aspose.gridweb.GridTableItemStyle-}
```
public void setStyle(GridTableItemStyle value)
```


Liefert eine Kopie des Zellenstils. Setze den Stil für die Zelle.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) |  |

### setValue(Object value) {#setValue-java.lang.Object-}
```
public void setValue(Object value)
```


Ruft den in dieser Zelle enthaltenen Wert ab.

**Remarks**

Möglicher Typ:

null,

Boolean,

DateTime,

Double,

Integer

String.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.Object |  |

### toString() {#toString--}
```
public String toString()
```


Gibt eine Zeichenkette zurück, die das aktuelle Cell-Objekt darstellt.

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

