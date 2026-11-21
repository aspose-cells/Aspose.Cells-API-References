---
title: "GridCell"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar ett cellobjekt."
type: docs
url: /sv/java/com.aspose.gridweb/gridcell/
---

**Inheritance:**
java.lang.Object
```
public class GridCell
```

Representerar ett cellobjekt.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [containsExternalLink()](#containsExternalLink--) | Indikerar om den här cellen innehåller en extern länk. |
| [copy(GridCell source)](#copy-com.aspose.gridweb.GridCell-) | Kopierar data från en källcell. |
| [copyStyle(GridTableItemStyle style)](#copyStyle-com.aspose.gridweb.GridTableItemStyle-) | kopiera stilen och ange stilen för cellen |
| [createComment(String note, String author, boolean isvisible)](#createComment-java.lang.String-java.lang.String-boolean-) | Skapar ett kommentarsobjekt för en cell. |
| [createValidation(int validationType, boolean isRequried)](#createValidation-int-boolean-) | Skapar ett valideringsobjekt för en cell. |
| [equals(Object obj)](#equals-java.lang.Object-) | Kontrollerar om detta objekt refererar till samma cell som ett annat cellobjekt. |
| [getBoolValue()](#getBoolValue--) | Hämtar det booleska värdet som finns i cellen. |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | Hämtar kolumnnumret (nollbaserat) för cellen. |
| [getComment()](#getComment--) | Hämta kommentarsobjekt på den här cellen |
| [getDateValue()](#getDateValue--) | Hämtar DateTime‑värdet som finns i cellen. |
| [getDisplayStringValue()](#getDisplayStringValue--) | Hämtar det formaterade strängvärdet för den här cellen. |
| [getDoubleValue()](#getDoubleValue--) | Hämtar det dubbelvärde som finns i cellen. |
| [getFloatValue()](#getFloatValue--) | Hämtar flyttalsvärdet som finns i cellen. |
| [getFormula()](#getFormula--) | Hämtar en formel för [GridCell](../../com.aspose.gridweb/gridcell). |
| [getHtmlString()](#getHtmlString--) | Hämtar HTML-strängen som innehåller data och viss formatering i den här cellen. |
| [getIntValue()](#getIntValue--) | Hämtar heltalsvärdet som finns i cellen. |
| [getName()](#getName--) | Hämtar namnet på cellen. |
| [getRow()](#getRow--) | Hämtar radnumret (nollbaserat) för cellen. |
| [getStringValue()](#getStringValue--) | Hämtar strängvärdet som finns i cellen. |
| [getStyle()](#getStyle--) | Hämtar en kopia av cellstilen. Ange stilen för cellen. |
| [getType()](#getType--) | returnerar cellvärdestypen, betydelsen kan ses i GridCellValueType.java |
| [getValue()](#getValue--) | Hämtar värdet som finns i den här cellen. |
| [getWidthOfValue()](#getWidthOfValue--) | Hämtar bredden på värdet i enheten pixlar. |
| [hashCode()](#hashCode--) | Fungerar som en hash-funktion för en specifik typ. |
| [isErrorValue()](#isErrorValue--) | Kontrollerar om en formel kan utvärdera ett resultat korrekt. |
| [isFormula()](#isFormula--) | Representerar om den angivna cellen innehåller en formel. |
| [isStyleSet()](#isStyleSet--) | Anger om cellens stil är inställd. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [putValue(boolean param_boolean)](#putValue-boolean-) | Sätter ett booleskt värde i cellen. |
| [putValue(DateTime param_date)](#putValue-com.aspose.gridweb.DateTime-) | Sätter ett DateTime‑värde i cellen. |
| [putValue(double param_double)](#putValue-double-) | Lägger in ett dubbelvärde i cellen. |
| [putValue(int param_int)](#putValue-int-) | Sätter ett heltalsvärde i cellen. |
| [putValue(Object objectValue)](#putValue-java.lang.Object-) | Sätter ett objektvärde i cellen. samma som setValue(Object param\_object) |
| [putValue(String param_string)](#putValue-java.lang.String-) | Sätter ett strängvärde i cellen. |
| [putValue(String stringValue, boolean isConverted)](#putValue-java.lang.String-boolean-) | Lägger in ett strängvärde i cellen och konverterar värdet till en annan datatyp om det är lämpligt. |
| [putValue(String stringValue, boolean isConverted, boolean setStyle)](#putValue-java.lang.String-boolean-boolean-) | Lägger in ett värde i cellen, om det är lämpligt konverteras värdet till en annan datatyp och cellens talformat återställs. |
| [putValueAndSetFormatByValue(String stringValue)](#putValueAndSetFormatByValue-java.lang.String-) | Sätter cellens värde med ett strängvärde och anger cellformatet efter detta värde. |
| [removeComment()](#removeComment--) | Tar bort kommentarsobjektet från cellen. |
| [removeValidation()](#removeValidation--) | Tar bort valideringsobjektet från cellen. |
| [setBorder(WebBorderStyle borderStyle)](#setBorder-com.aspose.gridweb.WebBorderStyle-) | Sätter kanter (top,bottom,left and right) för en cell, alla kanter har samma kantstil. |
| [setCustom(String custom)](#setCustom-java.lang.String-) | sätter det anpassade formatet, null eller tom sträng betyder inget anpassat format. |
| [setFormula(String value)](#setFormula-java.lang.String-) | Sätter en formel för [GridCell](../../com.aspose.gridweb/gridcell). |
| [setFormula(String formula, Object value)](#setFormula-java.lang.String-java.lang.Object-) | Ställ in formeln och formelns värde. |
| [setHtmlString(String value)](#setHtmlString-java.lang.String-) | Sätter HTML-strängen som innehåller data och viss formatering i den här cellen. |
| [setNumberType(int numbertype)](#setNumberType-int-) | ange visningsformatet för tal och datum |
| [setStyle(GridTableItemStyle value)](#setStyle-com.aspose.gridweb.GridTableItemStyle-) | Hämtar en kopia av cellstilen. Ange stilen för cellen. |
| [setValue(Object value)](#setValue-java.lang.Object-) | Hämtar värdet som finns i den här cellen. |
| [toString()](#toString--) | Returnerar en sträng som representerar det aktuella Cell‑objektet. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### containsExternalLink() {#containsExternalLink--}
```
public boolean containsExternalLink()
```


Indikerar om den här cellen innehåller en extern länk. Gäller endast när cellen är en formelcell.

**Returns:**
boolean
### copy(GridCell source) {#copy-com.aspose.gridweb.GridCell-}
```
public void copy(GridCell source)
```


Kopierar data från en källcell.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| source | [GridCell](../../com.aspose.gridweb/gridcell) | Källobjektet [GridCell](../../com.aspose.gridweb/gridcell). |

### copyStyle(GridTableItemStyle style) {#copyStyle-com.aspose.gridweb.GridTableItemStyle-}
```
public void copyStyle(GridTableItemStyle style)
```


kopiera stilen och ange stilen för cellen

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| style | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) | Källstilen. |

### createComment(String note, String author, boolean isvisible) {#createComment-java.lang.String-java.lang.String-boolean-}
```
public GridComment createComment(String note, String author, boolean isvisible)
```


Skapar ett kommentarsobjekt för en cell.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| anteckning | java.lang.String | kommentaranteckning. |
| författare | java.lang.String | kommentarförfattare. |
| isvisible | boolean | om kommentaren är synlig. |

**Returns:**
[GridComment](../../com.aspose.gridweb/gridcomment) - GridComment object
### createValidation(int validationType, boolean isRequried) {#createValidation-int-boolean-}
```
public GridValidation createValidation(int validationType, boolean isRequried)
```


Skapar ett valideringsobjekt för en cell.

**Example**

```
         GridWeb GridWeb1 = new GridWeb();
         GridWorksheet sheet = GridWeb1.getActiveSheet();
         GridValidation v = sheet.getCells().get("A1").createValidation(GridValidationType.CUSTOM_EXPRESSION, true);
         		// Sets to number validation expression.
         		v.setRegEx("\\d+");
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| validationType | int | [GridValidationType](../../com.aspose.gridweb/gridvalidationtype). Valideringstyp. |
| isRequried | boolean | Om cellvärdet är obligatoriskt. |

**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation) - 
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Kontrollerar om detta objekt refererar till samma cell som ett annat cellobjekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| obj | java.lang.Object | ett annat GridCell-objekt |

**Returns:**
boolesk – true om två cellobjekt refererar till samma cell.
### getBoolValue() {#getBoolValue--}
```
public boolean getBoolValue()
```


Hämtar det booleska värdet som finns i cellen.

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


Hämtar kolumnnumret (nollbaserat) för cellen.

**Returns:**
int
### getComment() {#getComment--}
```
public GridComment getComment()
```


Hämta kommentarsobjekt på den här cellen

**Returns:**
[GridComment](../../com.aspose.gridweb/gridcomment)
### getDateValue() {#getDateValue--}
```
public DateTime getDateValue()
```


Hämtar DateTime‑värdet som finns i cellen.

**Returns:**
[DateTime](../../com.aspose.gridweb/datetime)
### getDisplayStringValue() {#getDisplayStringValue--}
```
public String getDisplayStringValue()
```


Hämtar det formaterade strängvärdet för den här cellen.

**Returns:**
java.lang.String
### getDoubleValue() {#getDoubleValue--}
```
public double getDoubleValue()
```


Hämtar det dubbelvärde som finns i cellen.

**Returns:**
double
### getFloatValue() {#getFloatValue--}
```
public float getFloatValue()
```


Hämtar flyttalsvärdet som finns i cellen.

**Returns:**
float
### getFormula() {#getFormula--}
```
public String getFormula()
```


Hämtar en formel för [GridCell](../../com.aspose.gridweb/gridcell).

**Remarks**

En formelsträng börjar alltid med ett lika-tecken (=). Och vänligen använd alltid kommatecken (,) som parameteravgränsare, till exempel "=SUM(A1, E1, H2)".

Användaren kan ange vilken formel som helst i Workbook-designerfilen. Aspose.Cells behåller alla formler. Om användaren använder den här egenskapen för att sätta en formel i en cell, stöds en stor del av Workbook:s inbyggda funktioner. Och mer kommer. Om du har några speciella behov för Workbook:s inbyggda funktioner, vänligen meddela oss.

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


Hämtar HTML-strängen som innehåller data och viss formatering i den här cellen.

**Returns:**
java.lang.String
### getIntValue() {#getIntValue--}
```
public int getIntValue()
```


Hämtar heltalsvärdet som finns i cellen.

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


Hämtar namnet på cellen. Till exempel: A1, F102.

**Returns:**
java.lang.String
### getRow() {#getRow--}
```
public int getRow()
```


Hämtar radnumret (nollbaserat) för cellen.

**Returns:**
int
### getStringValue() {#getStringValue--}
```
public String getStringValue()
```


Hämtar strängvärdet som finns i cellen.

**Returns:**
java.lang.String
### getStyle() {#getStyle--}
```
public GridTableItemStyle getStyle()
```


Hämtar en kopia av cellstilen. Ange stilen för cellen.

**Returns:**
[GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) - Style object.
### getType() {#getType--}
```
public int getType()
```


returnerar cellvärdestypen, betydelsen kan ses i GridCellValueType.java

**Returns:**
int
### getValue() {#getValue--}
```
public Object getValue()
```


Hämtar värdet som finns i den här cellen.

**Remarks**

Möjlig typ:

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


Hämtar bredden på värdet i enheten pixlar.

**Returns:**
int -
### hashCode() {#hashCode--}
```
public int hashCode()
```


Fungerar som en hash-funktion för en specifik typ.

**Returns:**
int - En hashkod för aktuellt GridCell-objekt.
### isErrorValue() {#isErrorValue--}
```
public boolean isErrorValue()
```


Kontrollerar om en formel kan utvärdera ett resultat korrekt.

**Remarks**

Gäller endast för formelcell.

**Returns:**
boolean
### isFormula() {#isFormula--}
```
public boolean isFormula()
```


Representerar om den angivna cellen innehåller en formel.

**Returns:**
boolean
### isStyleSet() {#isStyleSet--}
```
public boolean isStyleSet()
```


Indikerar om cellens stil är inställd. Om den returnerar false betyder det att cellen har ett standardcellformat.

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


Sätter ett booleskt värde i cellen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| param_boolean | boolean | Indatavärde |

### putValue(DateTime param_date) {#putValue-com.aspose.gridweb.DateTime-}
```
public void putValue(DateTime param_date)
```


Sätter ett DateTime‑värde i cellen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| param_date | [DateTime](../../com.aspose.gridweb/datetime) | Indatavärde |

### putValue(double param_double) {#putValue-double-}
```
public void putValue(double param_double)
```


Lägger in ett dubbelvärde i cellen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| param_double | double | Indatavärde |

### putValue(int param_int) {#putValue-int-}
```
public void putValue(int param_int)
```


Sätter ett heltalsvärde i cellen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| param_int | int | Indatavärde |

### putValue(Object objectValue) {#putValue-java.lang.Object-}
```
public void putValue(Object objectValue)
```


Sätter ett objektvärde i cellen. samma som setValue(Object param\_object)

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| objectValue | java.lang.Object | indatavärde |

### putValue(String param_string) {#putValue-java.lang.String-}
```
public void putValue(String param_string)
```


Sätter ett strängvärde i cellen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| param_string | java.lang.String | Indatavärde |

### putValue(String stringValue, boolean isConverted) {#putValue-java.lang.String-boolean-}
```
public void putValue(String stringValue, boolean isConverted)
```


Lägger in ett strängvärde i cellen och konverterar värdet till en annan datatyp om det är lämpligt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stringValue | java.lang.String | Indatavärde |
| isConverted | boolean | True: konverterad till annan datatyp om lämpligt. |

### putValue(String stringValue, boolean isConverted, boolean setStyle) {#putValue-java.lang.String-boolean-boolean-}
```
public void putValue(String stringValue, boolean isConverted, boolean setStyle)
```


Lägger in ett värde i cellen, om det är lämpligt konverteras värdet till en annan datatyp och cellens talformat återställs.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stringValue | java.lang.String | Indatavärde |
| isConverted | boolean | True: konverterad till annan datatyp om lämpligt. |
| setStyle | boolean | True: sätt talformatet till cellens stil när du konverterar till annan datatyp |

### putValueAndSetFormatByValue(String stringValue) {#putValueAndSetFormatByValue-java.lang.String-}
```
public void putValueAndSetFormatByValue(String stringValue)
```


Sätter cellens värde med ett strängvärde och anger cellformatet efter detta värde.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| stringValue | java.lang.String | Inmatningsvärde. |

### removeComment() {#removeComment--}
```
public void removeComment()
```


Tar bort kommentarsobjektet från cellen.

### removeValidation() {#removeValidation--}
```
public void removeValidation()
```


Tar bort valideringsobjektet från cellen.

### setBorder(WebBorderStyle borderStyle) {#setBorder-com.aspose.gridweb.WebBorderStyle-}
```
public void setBorder(WebBorderStyle borderStyle)
```


Sätter kanter (top,bottom,left and right) för en cell, alla kanter har samma kantstil.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| borderStyle | [WebBorderStyle](../../com.aspose.gridweb/webborderstyle) | Kantstilen. |

### setCustom(String custom) {#setCustom-java.lang.String-}
```
public void setCustom(String custom)
```


sätter det anpassade formatet, null eller tom sträng betyder inget anpassat format.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| anpassad | java.lang.String | den anpassade strängpresentationen |

### setFormula(String value) {#setFormula-java.lang.String-}
```
public void setFormula(String value)
```


Sätter en formel för [GridCell](../../com.aspose.gridweb/gridcell).

**Remarks**

En formelsträng börjar alltid med ett lika-tecken (=). Och vänligen använd alltid kommatecken (,) som parameteravgränsare, till exempel "=SUM(A1, E1, H2)".

Användaren kan ange vilken formel som helst i Workbook-designerfilen. Aspose.Cells behåller alla formler. Om användaren använder den här egenskapen för att sätta en formel i en cell, stöds en stor del av Workbook:s inbyggda funktioner. Och mer kommer. Om du har några speciella behov för Workbook:s inbyggda funktioner, vänligen meddela oss.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setFormula(String formula, Object value) {#setFormula-java.lang.String-java.lang.Object-}
```
public void setFormula(String formula, Object value)
```


Ställ in formeln och formelns värde.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| formula | java.lang.String | Formeln. |
| värde | java.lang.Object | Formelns värde. |

### setHtmlString(String value) {#setHtmlString-java.lang.String-}
```
public void setHtmlString(String value)
```


Sätter HTML-strängen som innehåller data och viss formatering i den här cellen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setNumberType(int numbertype) {#setNumberType-int-}
```
public void setNumberType(int numbertype)
```


ange visningsformatet för tal och datum

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| numbertype | int | värdet av den numbertype, se GridTableItemStyle.NumberType |

### setStyle(GridTableItemStyle value) {#setStyle-com.aspose.gridweb.GridTableItemStyle-}
```
public void setStyle(GridTableItemStyle value)
```


Hämtar en kopia av cellstilen. Ange stilen för cellen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) |  |

### setValue(Object value) {#setValue-java.lang.Object-}
```
public void setValue(Object value)
```


Hämtar värdet som finns i den här cellen.

**Remarks**

Möjlig typ:

null,

Boolean,

DateTime,

Double,

Integer

String.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.Object |  |

### toString() {#toString--}
```
public String toString()
```


Returnerar en sträng som representerar det aktuella Cell‑objektet.

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

