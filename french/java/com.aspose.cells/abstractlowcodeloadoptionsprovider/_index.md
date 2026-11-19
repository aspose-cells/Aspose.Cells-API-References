---
title: "AbstractLowCodeLoadOptionsProvider"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Implémentation permettant de fournir plusieurs options de chargement pour les processus qui utilisent plusieurs entrées, telles que des fichiers de modèle."
type: docs
url: /fr/java/com.aspose.cells/abstractlowcodeloadoptionsprovider/
---

**Inheritance:**
java.lang.Object
```
public abstract class AbstractLowCodeLoadOptionsProvider
```

Implémentation pour fournir plusieurs options de chargement pour les processus qui utilisent plusieurs entrées (comme des fichiers de modèle).

**Remarks**

Par exemple, la fonctionnalité [SpreadsheetMerger](../../com.aspose.cells/spreadsheetmerger) nécessite plusieurs fichiers de modèle à fusionner.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [AbstractLowCodeLoadOptionsProvider()](#AbstractLowCodeLoadOptionsProvider--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [finish(LowCodeLoadOptions part)](#finish-com.aspose.cells.LowCodeLoadOptions-) | Libère les ressources après le traitement de la partie actuelle de l'entrée. |
| [getClass()](#getClass--) |  |
| [getCurrent()](#getCurrent--) | Obtient les options de chargement à partir desquelles charger les données de la partie actuellement traitée. |
| [hashCode()](#hashCode--) |  |
| [moveNext()](#moveNext--) | Vérifie s'il y a plus d'entrée. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### AbstractLowCodeLoadOptionsProvider() {#AbstractLowCodeLoadOptionsProvider--}
```
public AbstractLowCodeLoadOptionsProvider()
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
### finish(LowCodeLoadOptions part) {#finish-com.aspose.cells.LowCodeLoadOptions-}
```
public void finish(LowCodeLoadOptions part)
```


Libère les ressources après le traitement de la partie actuelle de l'entrée.

**Remarks**

Par défaut, cette méthode ferme simplement le flux spécifié par le [LowCodeLoadOptions.getInputStream()](../../com.aspose.cells/lowcodeloadoptions\#getInputStream--) directement (si les options de chargement ont spécifié un Stream comme source). L'utilisateur peut remplacer cette méthode pour contrôler la libération des ressources selon ses besoins et l'implémentation de [getCurrent()](../../com.aspose.cells/abstractlowcodeloadoptionsprovider\#getCurrent--).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| part | [LowCodeLoadOptions](../../com.aspose.cells/lowcodeloadoptions) | les options de chargement utilisées pour la partie actuellement divisée. |

### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCurrent() {#getCurrent--}
```
public abstract LowCodeLoadOptions getCurrent()
```


Obtient les options de chargement à partir desquelles charger les données de la partie actuellement traitée.

**Returns:**
[LowCodeLoadOptions](../../com.aspose.cells/lowcodeloadoptions)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### moveNext() {#moveNext--}
```
public abstract boolean moveNext()
```


Vérifie s'il y a plus d'entrée.

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

