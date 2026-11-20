---
title: "SignatureLine"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt die Signaturzeile dar."
type: docs
url: /de/java/com.aspose.cells/signatureline/
---

**Inheritance:**
java.lang.Object
```
public class SignatureLine
```

Stellt die Signaturzeile dar.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         Worksheet worksheet = workbook.getWorksheets().get(0);
 
         // Create signature line object
         SignatureLine s = new SignatureLine();
         s.setSigner("Simon");
         s.setTitle("Development");
         s.setEmail("simon@aspose.com");
         s.setInstructions("Sign to confirm the excel content.");
 
         // Adds a Signature Line to the worksheet.
         Picture signatureLine = worksheet.getShapes().addSignatureLine(0, 0, s);
 
         //do your business
 
         //Save the excel file.
         workbook.save("result.xlsx");
```
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [SignatureLine()](#SignatureLine--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllowComments()](#getAllowComments--) | Gibt an, ob Kommentare angehängt werden können. |
| [getClass()](#getClass--) |  |
| [getEmail()](#getEmail--) | Liest die E‑Mail des Unterzeichners. |
| [getId()](#getId--) | Liest den Bezeichner für diese Signaturzeile. |
| [getInstructions()](#getInstructions--) | Liest den Text, der dem Benutzer zur Signaturzeit angezeigt wird. |
| [getProviderId()](#getProviderId--) | Liest die ID des Signaturanbieters. |
| [getShowSignedDate()](#getShowSignedDate--) | Gibt an, ob das signierte Datum angezeigt wird. |
| [getSignatureLineType()](#getSignatureLineType--) | Liest den Signaturtyp. |
| [getSigner()](#getSigner--) | Liest den Unterzeichner. |
| [getTitle()](#getTitle--) | Liest den Titel des Unterzeichners. |
| [hashCode()](#hashCode--) |  |
| [isLine()](#isLine--) | Gibt an, ob es sich um eine Signaturzeile handelt. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllowComments(boolean value)](#setAllowComments-boolean-) | Gibt an, ob Kommentare angehängt werden können. |
| [setEmail(String value)](#setEmail-java.lang.String-) | Legt die E‑Mail des Unterzeichners fest. |
| [setId(UUID value)](#setId-java.util.UUID-) | Legt den Bezeichner für diese Signaturzeile fest. |
| [setInstructions(String value)](#setInstructions-java.lang.String-) | Legt den dem Benutzer beim Signieren angezeigten Text fest. |
| [setLine(boolean value)](#setLine-boolean-) | Gibt an, ob es sich um eine Signaturzeile handelt. |
| [setProviderId(UUID value)](#setProviderId-java.util.UUID-) | Legt die ID des Signaturanbieters fest. |
| [setShowSignedDate(boolean value)](#setShowSignedDate-boolean-) | Gibt an, ob das signierte Datum angezeigt wird. |
| [setSignatureLineType(int value)](#setSignatureLineType-int-) | Legt den Signaturtyp fest. |
| [setSigner(String value)](#setSigner-java.lang.String-) | Legt den Unterzeichner fest. |
| [setTitle(String value)](#setTitle-java.lang.String-) | Legt den Titel des Unterzeichners fest. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### SignatureLine() {#SignatureLine--}
```
public SignatureLine()
```


### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getAllowComments() {#getAllowComments--}
```
public boolean getAllowComments()
```


Gibt an, ob Kommentare angehängt werden können.

**Example**

```
         if(s.getAllowComments())
         {
             // Comments could be attached.
         }
```

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getEmail() {#getEmail--}
```
public String getEmail()
```


Liest die E‑Mail des Unterzeichners.

**Example**

```
         // Create signature line object
         SignatureLine s5 = new SignatureLine();
         s5.setEmail("Simon.Zhao@aspose.com");
```

**Returns:**
java.lang.String
### getId() {#getId--}
```
public UUID getId()
```


Liest den Bezeichner für diese Signaturzeile.

**Example**

```
         // Create signature line object
         SignatureLine s1 = new SignatureLine();
         s1.setId(java.util.UUID.randomUUID());
```

**Returns:**
java.util.UUID
### getInstructions() {#getInstructions--}
```
public String getInstructions()
```


Liest den Text, der dem Benutzer zur Signaturzeit angezeigt wird.

**Example**

```
         // Create signature line object
         SignatureLine s6 = new SignatureLine();
         s6.setInstructions("Just do it.");
```

**Returns:**
java.lang.String
### getProviderId() {#getProviderId--}
```
public UUID getProviderId()
```


Liest die ID des Signaturanbieters.

**Remarks**

Es ist typischerweise die CLSID des Provider‑COM‑Add‑Ins.

**Example**

```
         // Create signature line object
         SignatureLine s2 = new SignatureLine();
         s2.setProviderId(java.util.UUID.fromString("xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx"));//The GUID should be obtained from the documentation shipped with the provider.
```

**Returns:**
java.util.UUID
### getShowSignedDate() {#getShowSignedDate--}
```
public boolean getShowSignedDate()
```


Gibt an, ob das signierte Datum angezeigt wird.

**Example**

```
         if(s.getShowSignedDate())
         {
             //Show signed date.
         }
```

**Returns:**
boolean
### getSignatureLineType() {#getSignatureLineType--}
```
public int getSignatureLineType()
```


Liest den Signaturtyp. Default - Wenn der Standardwert gesetzt ist, ist der entsprechende ProviderId‑Wert fest auf \{0000000000-0000-0000-0000-0000000000\}. Stamp - Wenn der Wert Stamp ist, ist der entsprechende ProviderId‑Wert normalerweise \{000CD6A4-0000-0000-C000-000000000046\}. Custom - Wenn der Wert Custom ist, muss der entsprechende ProviderId‑Wert in der Regel vom Benutzer festgelegt werden. Er sollte aus der Dokumentation des Anbieters entnommen werden.

Siehe [SignatureType](../../com.aspose.cells/signaturetype).

**Returns:**
int
### getSigner() {#getSigner--}
```
public String getSigner()
```


Liest den Unterzeichner.

**Example**

```
         // Create signature line object
         SignatureLine s3 = new SignatureLine();
         s3.setSigner("Mr xxx");
```

**Returns:**
java.lang.String
### getTitle() {#getTitle--}
```
public String getTitle()
```


Liest den Titel des Unterzeichners.

**Example**

```
         // Create signature line object
         SignatureLine s4 = new SignatureLine();
         s4.setTitle("Development Lead");
```

**Returns:**
java.lang.String
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isLine() {#isLine--}
```
public boolean isLine()
```


Gibt an, ob es sich um eine Signaturzeile handelt.

**Example**

```
         if(s.isLine())
         {
             //Is line.
         }
```

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




### setAllowComments(boolean value) {#setAllowComments-boolean-}
```
public void setAllowComments(boolean value)
```


Gibt an, ob Kommentare angehängt werden können.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setEmail(String value) {#setEmail-java.lang.String-}
```
public void setEmail(String value)
```


Legt die E‑Mail des Unterzeichners fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setId(UUID value) {#setId-java.util.UUID-}
```
public void setId(UUID value)
```


Legt den Bezeichner für diese Signaturzeile fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.util.UUID |  |

### setInstructions(String value) {#setInstructions-java.lang.String-}
```
public void setInstructions(String value)
```


Legt den dem Benutzer beim Signieren angezeigten Text fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setLine(boolean value) {#setLine-boolean-}
```
public void setLine(boolean value)
```


Gibt an, ob es sich um eine Signaturzeile handelt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setProviderId(UUID value) {#setProviderId-java.util.UUID-}
```
public void setProviderId(UUID value)
```


Legt die ID des Signaturanbieters fest.

**Remarks**

Es ist typischerweise die CLSID des Provider‑COM‑Add‑Ins.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.util.UUID |  |

### setShowSignedDate(boolean value) {#setShowSignedDate-boolean-}
```
public void setShowSignedDate(boolean value)
```


Gibt an, ob das signierte Datum angezeigt wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setSignatureLineType(int value) {#setSignatureLineType-int-}
```
public void setSignatureLineType(int value)
```


Legt den Signaturtyp fest. Default - Wenn der Standardwert gesetzt ist, ist der entsprechende ProviderId‑Wert fest auf \{0000000000-0000-0000-0000-0000000000\}. Stamp - Wenn der Wert Stamp ist, ist der entsprechende ProviderId‑Wert normalerweise \{000CD6A4-0000-0000-C000-000000000046\}. Custom - Wenn der Wert Custom ist, muss der entsprechende ProviderId‑Wert in der Regel vom Benutzer festgelegt werden. Er sollte aus der Dokumentation des Anbieters entnommen werden.

Siehe [SignatureType](../../com.aspose.cells/signaturetype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setSigner(String value) {#setSigner-java.lang.String-}
```
public void setSigner(String value)
```


Legt den Unterzeichner fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setTitle(String value) {#setTitle-java.lang.String-}
```
public void setTitle(String value)
```


Legt den Titel des Unterzeichners fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

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

