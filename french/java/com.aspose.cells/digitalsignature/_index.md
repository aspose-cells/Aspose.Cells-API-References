---
title: "DigitalSignature"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Signature dans le fichier."
type: docs
url: /fr/java/com.aspose.cells/digitalsignature/
---

**Inheritance:**
java.lang.Object
```
public class DigitalSignature
```

Signature dans le fichier.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [DigitalSignature(KeyStore certificate, String privateKeyPassword, String comments, DateTime signTime)](#DigitalSignature-java.security.KeyStore-java.lang.String-java.lang.String-com.aspose.cells.DateTime-) | Constructeur de digitalSignature. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCertificate()](#getCertificate--) | Objet certificat qui a été utilisé pour signer le document. |
| [getClass()](#getClass--) |  |
| [getComments()](#getComments--) | Le but de la signature. |
| [getId()](#getId--) | Spécifie un GUID qui peut être référencé en croix avec le GUID de la ligne de signature stockée dans le contenu du document. |
| [getImage()](#getImage--) | Spécifie une image pour la signature numérique. |
| [getProviderId()](#getProviderId--) | Spécifie l'ID de classe du fournisseur de signature. |
| [getSignTime()](#getSignTime--) | L'heure à laquelle le document a été signé. |
| [getText()](#getText--) | Spécifie le texte de la signature réelle dans la signature numérique. |
| [getXAdESType()](#getXAdESType--) | Type XAdES. |
| [hashCode()](#hashCode--) |  |
| [isValid()](#isValid--) | Si cette signature numérique est valide et que le document n’a pas été altéré, cette valeur sera true. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCertificate(KeyStore value)](#setCertificate-java.security.KeyStore-) | Objet certificat qui a été utilisé pour signer le document. |
| [setComments(String value)](#setComments-java.lang.String-) | Le but de la signature. |
| [setId(UUID value)](#setId-java.util.UUID-) | Spécifie un GUID qui peut être référencé en croix avec le GUID de la ligne de signature stockée dans le contenu du document. |
| [setImage(byte[] value)](#setImage-byte---) | Spécifie une image pour la signature numérique. |
| [setProviderId(UUID value)](#setProviderId-java.util.UUID-) | Spécifie l'ID de classe du fournisseur de signature. |
| [setSignTime(DateTime value)](#setSignTime-com.aspose.cells.DateTime-) | L'heure à laquelle le document a été signé. |
| [setText(String value)](#setText-java.lang.String-) | Spécifie le texte de la signature réelle dans la signature numérique. |
| [setXAdESType(int value)](#setXAdESType-int-) | Type XAdES. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### DigitalSignature(KeyStore certificate, String privateKeyPassword, String comments, DateTime signTime) {#DigitalSignature-java.security.KeyStore-java.lang.String-java.lang.String-com.aspose.cells.DateTime-}
```
public DigitalSignature(KeyStore certificate, String privateKeyPassword, String comments, DateTime signTime)
```


Constructeur de digitalSignature.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| certificat | java.security.KeyStore | Objet certificat qui a été utilisé pour signer le document. |
| privateKeyPassword | java.lang.String | Le mot de passe pour la clé privée. |
| commentaires | java.lang.String | Le but de la signature. |
| signTime | [DateTime](../../com.aspose.cells/datetime) | L'heure UTC lorsque le document a été signé. |

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
### getCertificate() {#getCertificate--}
```
public KeyStore getCertificate()
```


Objet certificat qui a été utilisé pour signer le document.

**Returns:**
java.security.KeyStore
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getComments() {#getComments--}
```
public String getComments()
```


Le but de la signature.

**Returns:**
java.lang.String
### getId() {#getId--}
```
public UUID getId()
```


Spécifie un GUID qui peut être référencé avec le GUID de la ligne de signature stockée dans le contenu du document. La valeur par défaut est Empty (tous les zéros) Guid.

**Remarks**

Lorsqu'il est défini, il associe [SignatureLine](../../com.aspose.cells/signatureline) à la [DigitalSignature](../../com.aspose.cells/digitalsignature) correspondante.

**Returns:**
java.util.UUID
### getImage() {#getImage--}
```
public byte[] getImage()
```


Spécifie une image pour la signature numérique. La valeur par défaut est null.

**Returns:**
byte[]
### getProviderId() {#getProviderId--}
```
public UUID getProviderId()
```


Spécifie l'ID de classe du fournisseur de signature. La valeur par défaut est Empty (tous les zéros) Guid.

**Remarks**

Le fournisseur de services cryptographiques (CSP) est un module logiciel indépendant qui exécute réellement les algorithmes de cryptographie pour l'authentification, le codage et le chiffrement. Microsoft Office réserve la valeur \{00000000-0000-0000-0000-000000000000\} pour son fournisseur de signature par défaut, et \{000CD6A4-0000-0000-C000-000000000046\} pour son fournisseur de signature asiatique de l'Est. Le GUID du fournisseur installé en supplément doit être obtenu dans la documentation fournie avec le fournisseur.

**Returns:**
java.util.UUID
### getSignTime() {#getSignTime--}
```
public DateTime getSignTime()
```


L'heure à laquelle le document a été signé.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getText() {#getText--}
```
public String getText()
```


Spécifie le texte de la signature réelle dans la signature numérique. La valeur par défaut est Empty.

**Returns:**
java.lang.String
### getXAdESType() {#getXAdESType--}
```
public int getXAdESType()
```


Type XAdES. La valeur par défaut est None (XAdES est désactivé).

Voir [XAdESType](../../com.aspose.cells/xadestype).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isValid() {#isValid--}
```
public boolean isValid()
```


Si cette signature numérique est valide et que le document n’a pas été altéré, cette valeur sera true.

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




### setCertificate(KeyStore value) {#setCertificate-java.security.KeyStore-}
```
public void setCertificate(KeyStore value)
```


Objet certificat qui a été utilisé pour signer le document.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.security.KeyStore |  |

### setComments(String value) {#setComments-java.lang.String-}
```
public void setComments(String value)
```


Le but de la signature.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setId(UUID value) {#setId-java.util.UUID-}
```
public void setId(UUID value)
```


Spécifie un GUID qui peut être référencé avec le GUID de la ligne de signature stockée dans le contenu du document. La valeur par défaut est Empty (tous les zéros) Guid.

**Remarks**

Lorsqu'il est défini, il associe [SignatureLine](../../com.aspose.cells/signatureline) à la [DigitalSignature](../../com.aspose.cells/digitalsignature) correspondante.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.util.UUID |  |

### setImage(byte[] value) {#setImage-byte---}
```
public void setImage(byte[] value)
```


Spécifie une image pour la signature numérique. La valeur par défaut est null.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | byte[] |  |

### setProviderId(UUID value) {#setProviderId-java.util.UUID-}
```
public void setProviderId(UUID value)
```


Spécifie l'ID de classe du fournisseur de signature. La valeur par défaut est Empty (tous les zéros) Guid.

**Remarks**

Le fournisseur de services cryptographiques (CSP) est un module logiciel indépendant qui exécute réellement les algorithmes de cryptographie pour l'authentification, le codage et le chiffrement. Microsoft Office réserve la valeur \{00000000-0000-0000-0000-000000000000\} pour son fournisseur de signature par défaut, et \{000CD6A4-0000-0000-C000-000000000046\} pour son fournisseur de signature asiatique de l'Est. Le GUID du fournisseur installé en supplément doit être obtenu dans la documentation fournie avec le fournisseur.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.util.UUID |  |

### setSignTime(DateTime value) {#setSignTime-com.aspose.cells.DateTime-}
```
public void setSignTime(DateTime value)
```


L'heure à laquelle le document a été signé.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Spécifie le texte de la signature réelle dans la signature numérique. La valeur par défaut est Empty.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setXAdESType(int value) {#setXAdESType-int-}
```
public void setXAdESType(int value)
```


Type XAdES. La valeur par défaut est None (XAdES est désactivé).

Voir [XAdESType](../../com.aspose.cells/xadestype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

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

