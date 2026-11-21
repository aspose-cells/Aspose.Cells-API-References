---
title: "SignatureLine"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar signaturlinjen."
type: docs
url: /sv/java/com.aspose.cells/signatureline/
---

**Inheritance:**
java.lang.Object
```
public class SignatureLine
```

Representerar signaturlinjen.

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
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [SignatureLine()](#SignatureLine--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllowComments()](#getAllowComments--) | Indikerar om kommentarer kan bifogas. |
| [getClass()](#getClass--) |  |
| [getEmail()](#getEmail--) | Hämtar e‑postadressen för sångaren. |
| [getId()](#getId--) | Hämtar identifieraren för denna signaturlinje. |
| [getInstructions()](#getInstructions--) | Hämtar texten som visas för användaren vid signering. |
| [getProviderId()](#getProviderId--) | Hämtar ID:t för signaturleverantören. |
| [getShowSignedDate()](#getShowSignedDate--) | Indikerar om signeringsdatum ska visas. |
| [getSignatureLineType()](#getSignatureLineType--) | Hämtar signaturtypen. |
| [getSigner()](#getSigner--) | Hämtar undertecknaren. |
| [getTitle()](#getTitle--) | Hämtar titeln för sångaren. |
| [hashCode()](#hashCode--) |  |
| [isLine()](#isLine--) | Indikerar om det är en signaturlinje. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllowComments(boolean value)](#setAllowComments-boolean-) | Indikerar om kommentarer kan bifogas. |
| [setEmail(String value)](#setEmail-java.lang.String-) | Ställer in e‑postadressen för sångaren. |
| [setId(UUID value)](#setId-java.util.UUID-) | Ställer in identifieraren för denna signaturlinje. |
| [setInstructions(String value)](#setInstructions-java.lang.String-) | Ställer in texten som visas för användaren vid signering. |
| [setLine(boolean value)](#setLine-boolean-) | Indikerar om det är en signaturlinje. |
| [setProviderId(UUID value)](#setProviderId-java.util.UUID-) | Ställer in ID:t för signaturleverantören. |
| [setShowSignedDate(boolean value)](#setShowSignedDate-boolean-) | Indikerar om signeringsdatum ska visas. |
| [setSignatureLineType(int value)](#setSignatureLineType-int-) | Ställer in signaturtypen. |
| [setSigner(String value)](#setSigner-java.lang.String-) | Ställer in undertecknaren. |
| [setTitle(String value)](#setTitle-java.lang.String-) | Ställer in titeln för sångaren. |
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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getAllowComments() {#getAllowComments--}
```
public boolean getAllowComments()
```


Indikerar om kommentarer kan bifogas.

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


Hämtar e‑postadressen för sångaren.

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


Hämtar identifieraren för denna signaturlinje.

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


Hämtar texten som visas för användaren vid signering.

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


Hämtar ID:t för signaturleverantören.

**Remarks**

Det är vanligtvis CLSID för leverantörens COM‑tillägg.

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


Indikerar om signeringsdatum ska visas.

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


Hämtar signaturtypen. Default - När standardvärdet är angivet är det motsvarande ProviderId‑värdet fixerat till \{0000000000-0000-0000-0000-0000000000\}. Stamp - När värdet är Stamp är det motsvarande ProviderId‑värdet vanligtvis \{000CD6A4-0000-0000-C000-000000000046\}. Custom - När värdet är Custom måste det motsvarande ProviderId‑värdet vanligtvis anges av användaren. Det bör hämtas från dokumentationen som medföljer leverantören.

Se [SignatureType](../../com.aspose.cells/signaturetype).

**Returns:**
int
### getSigner() {#getSigner--}
```
public String getSigner()
```


Hämtar undertecknaren.

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


Hämtar titeln för sångaren.

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


Indikerar om det är en signaturlinje.

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


Indikerar om kommentarer kan bifogas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setEmail(String value) {#setEmail-java.lang.String-}
```
public void setEmail(String value)
```


Ställer in e‑postadressen för sångaren.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setId(UUID value) {#setId-java.util.UUID-}
```
public void setId(UUID value)
```


Ställer in identifieraren för denna signaturlinje.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.util.UUID |  |

### setInstructions(String value) {#setInstructions-java.lang.String-}
```
public void setInstructions(String value)
```


Ställer in texten som visas för användaren vid signering.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setLine(boolean value) {#setLine-boolean-}
```
public void setLine(boolean value)
```


Indikerar om det är en signaturlinje.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setProviderId(UUID value) {#setProviderId-java.util.UUID-}
```
public void setProviderId(UUID value)
```


Ställer in ID:t för signaturleverantören.

**Remarks**

Det är vanligtvis CLSID för leverantörens COM‑tillägg.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.util.UUID |  |

### setShowSignedDate(boolean value) {#setShowSignedDate-boolean-}
```
public void setShowSignedDate(boolean value)
```


Indikerar om signeringsdatum ska visas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setSignatureLineType(int value) {#setSignatureLineType-int-}
```
public void setSignatureLineType(int value)
```


Ställer in signaturtypen. Default - När standardvärdet är angivet är det motsvarande ProviderId‑värdet fixerat till \{0000000000-0000-0000-0000-0000000000\}. Stamp - När värdet är Stamp är det motsvarande ProviderId‑värdet vanligtvis \{000CD6A4-0000-0000-C000-000000000046\}. Custom - När värdet är Custom måste det motsvarande ProviderId‑värdet vanligtvis anges av användaren. Det bör hämtas från dokumentationen som medföljer leverantören.

Se [SignatureType](../../com.aspose.cells/signaturetype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setSigner(String value) {#setSigner-java.lang.String-}
```
public void setSigner(String value)
```


Ställer in undertecknaren.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setTitle(String value) {#setTitle-java.lang.String-}
```
public void setTitle(String value)
```


Ställer in titeln för sångaren.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

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

