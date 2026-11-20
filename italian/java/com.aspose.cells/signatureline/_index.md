---
title: "SignatureLine"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta la linea di firma."
type: docs
url: /it/java/com.aspose.cells/signatureline/
---

**Inheritance:**
java.lang.Object
```
public class SignatureLine
```

Rappresenta la linea di firma.

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
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [SignatureLine()](#SignatureLine--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllowComments()](#getAllowComments--) | Indica se i commenti possono essere allegati. |
| [getClass()](#getClass--) |  |
| [getEmail()](#getEmail--) | Ottiene l'email del cantante. |
| [getId()](#getId--) | Ottiene l'identificatore per questa linea di firma. |
| [getInstructions()](#getInstructions--) | Ottiene il testo mostrato all'utente al momento della firma. |
| [getProviderId()](#getProviderId--) | Ottiene l'ID del provider di firma. |
| [getShowSignedDate()](#getShowSignedDate--) | Indica se mostra la data di firma. |
| [getSignatureLineType()](#getSignatureLineType--) | Ottiene il tipo di firma. |
| [getSigner()](#getSigner--) | Ottiene il firmatario. |
| [getTitle()](#getTitle--) | Ottiene il titolo del cantante. |
| [hashCode()](#hashCode--) |  |
| [isLine()](#isLine--) | Indica se è una linea di firma. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllowComments(boolean value)](#setAllowComments-boolean-) | Indica se i commenti possono essere allegati. |
| [setEmail(String value)](#setEmail-java.lang.String-) | Imposta l'email del cantante. |
| [setId(UUID value)](#setId-java.util.UUID-) | Imposta l'identificatore per questa linea di firma. |
| [setInstructions(String value)](#setInstructions-java.lang.String-) | Imposta il testo mostrato all'utente al momento della firma. |
| [setLine(boolean value)](#setLine-boolean-) | Indica se è una linea di firma. |
| [setProviderId(UUID value)](#setProviderId-java.util.UUID-) | Imposta l'ID del provider di firma. |
| [setShowSignedDate(boolean value)](#setShowSignedDate-boolean-) | Indica se mostra la data di firma. |
| [setSignatureLineType(int value)](#setSignatureLineType-int-) | Imposta il tipo di firma. |
| [setSigner(String value)](#setSigner-java.lang.String-) | Imposta il firmatario. |
| [setTitle(String value)](#setTitle-java.lang.String-) | Imposta il titolo del cantante. |
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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getAllowComments() {#getAllowComments--}
```
public boolean getAllowComments()
```


Indica se i commenti possono essere allegati.

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


Ottiene l'email del cantante.

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


Ottiene l'identificatore per questa linea di firma.

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


Ottiene il testo mostrato all'utente al momento della firma.

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


Ottiene l'ID del provider di firma.

**Remarks**

È tipicamente il CLSID del componente aggiuntivo COM del provider.

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


Indica se mostra la data di firma.

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


Ottiene il tipo di firma. Default - Quando il valore predefinito è impostato, il valore corrispondente di ProviderId è fissato a \{0000000000-0000-0000-0000-0000000000\}. Stamp - Quando il valore è Stamp, il valore corrispondente di ProviderId è solitamente \{000CD6A4-0000-0000-C000-000000000046\}. Custom - Quando il valore è Custom, il valore corrispondente di ProviderId di solito deve essere impostato dall'utente. dovrebbe essere ottenuto dalla documentazione fornita con il provider.

Vedi [SignatureType](../../com.aspose.cells/signaturetype).

**Returns:**
int
### getSigner() {#getSigner--}
```
public String getSigner()
```


Ottiene il firmatario.

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


Ottiene il titolo del cantante.

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


Indica se è una linea di firma.

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


Indica se i commenti possono essere allegati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setEmail(String value) {#setEmail-java.lang.String-}
```
public void setEmail(String value)
```


Imposta l'email del cantante.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setId(UUID value) {#setId-java.util.UUID-}
```
public void setId(UUID value)
```


Imposta l'identificatore per questa linea di firma.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.util.UUID |  |

### setInstructions(String value) {#setInstructions-java.lang.String-}
```
public void setInstructions(String value)
```


Imposta il testo mostrato all'utente al momento della firma.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setLine(boolean value) {#setLine-boolean-}
```
public void setLine(boolean value)
```


Indica se è una linea di firma.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setProviderId(UUID value) {#setProviderId-java.util.UUID-}
```
public void setProviderId(UUID value)
```


Imposta l'ID del provider di firma.

**Remarks**

È tipicamente il CLSID del componente aggiuntivo COM del provider.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.util.UUID |  |

### setShowSignedDate(boolean value) {#setShowSignedDate-boolean-}
```
public void setShowSignedDate(boolean value)
```


Indica se mostra la data di firma.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setSignatureLineType(int value) {#setSignatureLineType-int-}
```
public void setSignatureLineType(int value)
```


Imposta il tipo di firma. Default - Quando il valore predefinito è impostato, il valore corrispondente di ProviderId è fissato a \{0000000000-0000-0000-0000-0000000000\}. Stamp - Quando il valore è Stamp, il valore corrispondente di ProviderId è solitamente \{000CD6A4-0000-0000-C000-000000000046\}. Custom - Quando il valore è Custom, il valore corrispondente di ProviderId di solito deve essere impostato dall'utente. dovrebbe essere ottenuto dalla documentazione fornita con il provider.

Vedi [SignatureType](../../com.aspose.cells/signaturetype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setSigner(String value) {#setSigner-java.lang.String-}
```
public void setSigner(String value)
```


Imposta il firmatario.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setTitle(String value) {#setTitle-java.lang.String-}
```
public void setTitle(String value)
```


Imposta il titolo del cantante.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

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

