---
title: "AbstractGlobalizationSettings"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente les paramètres de mondialisation."
type: docs
url: /fr/java/com.aspose.cells/abstractglobalizationsettings/
---

**Inheritance:**
java.lang.Object
```
public abstract class AbstractGlobalizationSettings
```

Représente les paramètres de mondialisation.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [AbstractGlobalizationSettings()](#AbstractGlobalizationSettings--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
| [compare(String v1, String v2, boolean ignoreCase)](#compare-java.lang.String-java.lang.String-boolean-) | Compare deux valeurs de chaîne selon certaines règles de collation. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getCollationKey(String v, boolean ignoreCase)](#getCollationKey-java.lang.String-boolean-) | Transforme la chaîne en un objet comparable selon certaines règles de collation. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### AbstractGlobalizationSettings() {#AbstractGlobalizationSettings--}
```
public AbstractGlobalizationSettings()
```


### compare(String v1, String v2, boolean ignoreCase) {#compare-java.lang.String-java.lang.String-boolean-}
```
public int compare(String v1, String v2, boolean ignoreCase)
```


Compare deux valeurs de chaîne selon certaines règles de collation.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| v1 | java.lang.String | la première chaîne |
| v2 | java.lang.String | la deuxième chaîne |
| ignoreCase | boolean | indique s'il faut ignorer la casse lors de la comparaison des valeurs |

**Returns:**
int - Entier qui indique la relation lexicale entre les deux comparands
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
### getCollationKey(String v, boolean ignoreCase) {#getCollationKey-java.lang.String-boolean-}
```
public Comparable getCollationKey(String v, boolean ignoreCase)
```


Transforme la chaîne en un objet comparable selon certaines règles de collation.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| v | java.lang.String | La valeur String doit être comparée avec d'autres. |
| ignoreCase | boolean | indique s'il faut ignorer la casse lors de la comparaison des valeurs |

**Returns:**
java.lang.Comparable - L'objet peut être utilisé pour comparer ou trier des valeurs de chaîne
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

