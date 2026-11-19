---
title: "AbstractLowCodeSaveOptionsProvider"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Implémentation pour fournir plusieurs options d'enregistrement pour les processus qui nécessitent plusieurs sorties."
type: docs
url: /fr/java/com.aspose.cells/abstractlowcodesaveoptionsprovider/
---

**Inheritance:**
java.lang.Object
```
public abstract class AbstractLowCodeSaveOptionsProvider
```

Implémentation permettant de fournir plusieurs options d'enregistrement pour les processus nécessitant plusieurs sorties. Par exemple, la fonctionnalité [SpreadsheetSplitter](../../com.aspose.cells/spreadsheetsplitter) nécessite plusieurs destinations pour enregistrer les fichiers découpés.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [AbstractLowCodeSaveOptionsProvider()](#AbstractLowCodeSaveOptionsProvider--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [finish(LowCodeSaveOptions part)](#finish-com.aspose.cells.LowCodeSaveOptions-) | Libère les ressources après le traitement de la partie découpée actuelle. |
| [getClass()](#getClass--) |  |
| [getSaveOptions(SplitPartInfo part)](#getSaveOptions-com.aspose.cells.SplitPartInfo-) | Obtient les options d'enregistrement à partir desquelles récupérer les paramètres de sortie pour la partie découpée actuelle. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### AbstractLowCodeSaveOptionsProvider() {#AbstractLowCodeSaveOptionsProvider--}
```
public AbstractLowCodeSaveOptionsProvider()
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
### finish(LowCodeSaveOptions part) {#finish-com.aspose.cells.LowCodeSaveOptions-}
```
public void finish(LowCodeSaveOptions part)
```


Libère les ressources après le traitement de la partie découpée actuelle.

**Remarks**

Par défaut, cette méthode ferme simplement le flux spécifié par le [LowCodeSaveOptions.getOutputStream()](../../com.aspose.cells/lowcodesaveoptions\#getOutputStream--) directement (si les options d'enregistrement ont spécifié un flux comme destination). L'utilisateur peut remplacer cette méthode pour contrôler la façon de libérer les ressources selon ses besoins et l'implémentation de [getSaveOptions(SplitPartInfo)](../../com.aspose.cells/abstractlowcodesaveoptionsprovider\#getSaveOptions-SplitPartInfo-).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| part | [LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions) | les options d'enregistrement utilisées pour la partie découpée actuelle. |

### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getSaveOptions(SplitPartInfo part) {#getSaveOptions-com.aspose.cells.SplitPartInfo-}
```
public abstract LowCodeSaveOptions getSaveOptions(SplitPartInfo part)
```


Obtient les options d'enregistrement à partir desquelles récupérer les paramètres de sortie pour la partie découpée actuelle. Retourner null indique d'ignorer la partie donnée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| part | [SplitPartInfo](../../com.aspose.cells/splitpartinfo) |  |

**Returns:**
[LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions)
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

