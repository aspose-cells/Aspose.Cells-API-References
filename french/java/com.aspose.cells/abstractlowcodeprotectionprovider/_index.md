---
title: "AbstractLowCodeProtectionProvider"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Implémentation pour fournir des paramètres de protection."
type: docs
url: /fr/java/com.aspose.cells/abstractlowcodeprotectionprovider/
---

**Inheritance:**
java.lang.Object
```
public class AbstractLowCodeProtectionProvider
```

Implémentation pour fournir des paramètres de protection.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [AbstractLowCodeProtectionProvider()](#AbstractLowCodeProtectionProvider--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getOpenPassword()](#getOpenPassword--) | Obtient le mot de passe pour ouvrir le fichier de feuille de calcul. |
| [getWorkbookPassword()](#getWorkbookPassword--) | Obtient le mot de passe pour protéger le classeur avec le type de protection spécifié. |
| [getWorkbookProtectionType()](#getWorkbookProtectionType--) | Obtient le type de protection pour protéger le classeur. |
| [getWorksheetPassword(String sheetName)](#getWorksheetPassword-java.lang.String-) | Obtient le mot de passe pour protéger la feuille de calcul spécifiée. |
| [getWorksheetProtectionType(String sheetName)](#getWorksheetProtectionType-java.lang.String-) | Obtient le type de protection pour protéger la feuille de calcul spécifiée. |
| [getWritePassword()](#getWritePassword--) | Obtient le mot de passe pour modifier le fichier de feuille de calcul. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### AbstractLowCodeProtectionProvider() {#AbstractLowCodeProtectionProvider--}
```
public AbstractLowCodeProtectionProvider()
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getOpenPassword() {#getOpenPassword--}
```
public String getOpenPassword()
```


Obtient le mot de passe pour ouvrir le fichier de feuille de calcul.

**Returns:**
java.lang.String - Mot de passe pour ouvrir le fichier de feuille de calcul. Vide signifie aucune protection lors de l'ouverture du fichier.
### getWorkbookPassword() {#getWorkbookPassword--}
```
public String getWorkbookPassword()
```


Obtient le mot de passe pour protéger le classeur avec le type de protection spécifié.

**Returns:**
java.lang.String - Mot de passe pour protéger le classeur.
### getWorkbookProtectionType() {#getWorkbookProtectionType--}
```
public int getWorkbookProtectionType()
```


Obtient le type de protection pour protéger le classeur.

**Returns:**
int - [ProtectionType](../../com.aspose.cells/protectiontype). Type de protection pour protéger le classeur. [ProtectionType.NONE](../../com.aspose.cells/protectiontype\#NONE) signifie aucune protection pour le classeur.
### getWorksheetPassword(String sheetName) {#getWorksheetPassword-java.lang.String-}
```
public String getWorksheetPassword(String sheetName)
```


Obtient le mot de passe pour protéger la feuille de calcul spécifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sheetName | java.lang.String |  |

**Returns:**
java.lang.String - Mot de passe pour protéger la feuille de calcul spécifiée.
### getWorksheetProtectionType(String sheetName) {#getWorksheetProtectionType-java.lang.String-}
```
public int getWorksheetProtectionType(String sheetName)
```


Obtient le type de protection pour protéger la feuille de calcul spécifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sheetName | java.lang.String |  |

**Returns:**
int - [ProtectionType](../../com.aspose.cells/protectiontype). Type de protection pour protéger la feuille de calcul spécifiée. [ProtectionType.NONE](../../com.aspose.cells/protectiontype\#NONE) signifie aucune protection pour la feuille de calcul.
### getWritePassword() {#getWritePassword--}
```
public String getWritePassword()
```


Obtient le mot de passe pour modifier le fichier de feuille de calcul.

**Returns:**
java.lang.String - Mot de passe pour modifier le fichier de feuille de calcul. Vide signifie aucune protection pour la modification du fichier.
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




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

