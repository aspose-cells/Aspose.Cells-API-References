---
title: "SignatureLine"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente la ligne de signature."
type: docs
url: /fr/java/com.aspose.cells/signatureline/
---

**Inheritance:**
java.lang.Object
```
public class SignatureLine
```

Représente la ligne de signature.

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
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [SignatureLine()](#SignatureLine--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllowComments()](#getAllowComments--) | Indique si des commentaires peuvent être joints. |
| [getClass()](#getClass--) |  |
| [getEmail()](#getEmail--) | Obtient l'e‑mail du chanteur. |
| [getId()](#getId--) | Obtient l'identifiant de cette ligne de signature. |
| [getInstructions()](#getInstructions--) | Obtient le texte affiché à l'utilisateur lors de la signature. |
| [getProviderId()](#getProviderId--) | Obtient l'ID du fournisseur de signature. |
| [getShowSignedDate()](#getShowSignedDate--) | Indique si la date de signature doit être affichée. |
| [getSignatureLineType()](#getSignatureLineType--) | Obtient le type de signature. |
| [getSigner()](#getSigner--) | Obtient le signataire. |
| [getTitle()](#getTitle--) | Obtient le titre du chanteur. |
| [hashCode()](#hashCode--) |  |
| [isLine()](#isLine--) | Indique s'il s'agit d'une ligne de signature. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllowComments(boolean value)](#setAllowComments-boolean-) | Indique si des commentaires peuvent être joints. |
| [setEmail(String value)](#setEmail-java.lang.String-) | Définit l'e‑mail du chanteur. |
| [setId(UUID value)](#setId-java.util.UUID-) | Définit l'identifiant de cette ligne de signature. |
| [setInstructions(String value)](#setInstructions-java.lang.String-) | Définit le texte affiché à l'utilisateur lors de la signature. |
| [setLine(boolean value)](#setLine-boolean-) | Indique s'il s'agit d'une ligne de signature. |
| [setProviderId(UUID value)](#setProviderId-java.util.UUID-) | Définit l'ID du fournisseur de signature. |
| [setShowSignedDate(boolean value)](#setShowSignedDate-boolean-) | Indique si la date de signature doit être affichée. |
| [setSignatureLineType(int value)](#setSignatureLineType-int-) | Définit le type de signature. |
| [setSigner(String value)](#setSigner-java.lang.String-) | Définit le signataire. |
| [setTitle(String value)](#setTitle-java.lang.String-) | Définit le titre du chanteur. |
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
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getAllowComments() {#getAllowComments--}
```
public boolean getAllowComments()
```


Indique si des commentaires peuvent être joints.

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


Obtient l'e‑mail du chanteur.

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


Obtient l'identifiant de cette ligne de signature.

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


Obtient le texte affiché à l'utilisateur lors de la signature.

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


Obtient l'ID du fournisseur de signature.

**Remarks**

Il s'agit généralement du CLSID du module complémentaire COM du fournisseur.

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


Indique si la date de signature doit être affichée.

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


Obtient le type de signature. Default - Lorsque la valeur par défaut est définie, la valeur ProviderId correspondante est fixée à \{0000000000-0000-0000-0000-0000000000\}. Stamp - Lorsque la valeur est Stamp, la valeur ProviderId correspondante est généralement \{000CD6A4-0000-0000-C000-000000000046\}. Custom - Lorsque la valeur est Custom, la valeur ProviderId correspondante doit généralement être définie par l'utilisateur. Elle doit être obtenue dans la documentation fournie avec le fournisseur.

Voir [SignatureType](../../com.aspose.cells/signaturetype).

**Returns:**
int
### getSigner() {#getSigner--}
```
public String getSigner()
```


Obtient le signataire.

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


Obtient le titre du chanteur.

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


Indique s'il s'agit d'une ligne de signature.

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


Indique si des commentaires peuvent être joints.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setEmail(String value) {#setEmail-java.lang.String-}
```
public void setEmail(String value)
```


Définit l'e‑mail du chanteur.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setId(UUID value) {#setId-java.util.UUID-}
```
public void setId(UUID value)
```


Définit l'identifiant de cette ligne de signature.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.util.UUID |  |

### setInstructions(String value) {#setInstructions-java.lang.String-}
```
public void setInstructions(String value)
```


Définit le texte affiché à l'utilisateur lors de la signature.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setLine(boolean value) {#setLine-boolean-}
```
public void setLine(boolean value)
```


Indique s'il s'agit d'une ligne de signature.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setProviderId(UUID value) {#setProviderId-java.util.UUID-}
```
public void setProviderId(UUID value)
```


Définit l'ID du fournisseur de signature.

**Remarks**

Il s'agit généralement du CLSID du module complémentaire COM du fournisseur.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.util.UUID |  |

### setShowSignedDate(boolean value) {#setShowSignedDate-boolean-}
```
public void setShowSignedDate(boolean value)
```


Indique si la date de signature doit être affichée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setSignatureLineType(int value) {#setSignatureLineType-int-}
```
public void setSignatureLineType(int value)
```


Définit le type de signature. Default - Lorsque la valeur par défaut est définie, la valeur ProviderId correspondante est fixée à \{0000000000-0000-0000-0000-0000000000\}. Stamp - Lorsque la valeur est Stamp, la valeur ProviderId correspondante est généralement \{000CD6A4-0000-0000-C000-000000000046\}. Custom - Lorsque la valeur est Custom, la valeur ProviderId correspondante doit généralement être définie par l'utilisateur. Elle doit être obtenue dans la documentation fournie avec le fournisseur.

Voir [SignatureType](../../com.aspose.cells/signaturetype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setSigner(String value) {#setSigner-java.lang.String-}
```
public void setSigner(String value)
```


Définit le signataire.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setTitle(String value) {#setTitle-java.lang.String-}
```
public void setTitle(String value)
```


Définit le titre du chanteur.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

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
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

