---
title: "ConditionalFormattingValue"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Décrit les valeurs des points d'interpolation dans une barre de données à échelle graduée ou un jeu d'icônes."
type: docs
url: /fr/java/com.aspose.cells/conditionalformattingvalue/
---

**Inheritance:**
java.lang.Object
```
public class ConditionalFormattingValue
```

Décrit les valeurs des points d'interpolation dans une échelle de dégradé, dataBar ou iconSet.
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getType()](#getType--) | Obtient le type de cet objet de valeur de mise en forme conditionnelle. |
| [getValue()](#getValue--) | Obtient la valeur de cet objet de valeur de mise en forme conditionnelle. |
| [hashCode()](#hashCode--) |  |
| [isGTE()](#isGTE--) | Obtient le drapeau Greater Than Or Equal. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setGTE(boolean value)](#setGTE-boolean-) | Définit le drapeau Greater Than Or Equal. |
| [setType(int value)](#setType-int-) | Définit le type de cet objet de valeur de mise en forme conditionnelle. |
| [setValue(Object value)](#setValue-java.lang.Object-) | Définit la valeur de cet objet de valeur de mise en forme conditionnelle. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getType() {#getType--}
```
public int getType()
```


Obtient le type de cet objet de valeur de mise en forme conditionnelle. Définir le type sur FormatConditionValueType.Min ou FormatConditionValueType.Max définira automatiquement \"Value\" à null.

Voir [FormatConditionValueType](../../com.aspose.cells/formatconditionvaluetype).

**Returns:**
int
### getValue() {#getValue--}
```
public Object getValue()
```


Obtient la valeur de cet objet de valeur de mise en forme conditionnelle. Il doit être utilisé en conjonction avec Type.

**Remarks**

Si la valeur est une chaîne et commence par \"=\", elle sera traitée comme une formule, sinon nous la traiterons comme une valeur simple.

**Returns:**
java.lang.Object
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isGTE() {#isGTE--}
```
public boolean isGTE()
```


Obtient le drapeau Greater Than Or Equal. À n'utiliser que pour les jeux d'icônes, détermine si cette valeur seuil utilise l'opérateur supérieur ou égal. 'false' indique que 'supérieur à' est utilisé au lieu de 'supérieur ou égal'. La valeur par défaut est true.

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




### setGTE(boolean value) {#setGTE-boolean-}
```
public void setGTE(boolean value)
```


Définit le drapeau Greater Than Or Equal. À n'utiliser que pour les jeux d'icônes, détermine si cette valeur seuil utilise l'opérateur supérieur ou égal. 'false' indique que 'supérieur à' est utilisé au lieu de 'supérieur ou égal'. La valeur par défaut est true.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Définit le type de cet objet de valeur de mise en forme conditionnelle. Définir le type sur FormatConditionValueType.Min ou FormatConditionValueType.Max définira automatiquement \"Value\" à null.

Voir [FormatConditionValueType](../../com.aspose.cells/formatconditionvaluetype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setValue(Object value) {#setValue-java.lang.Object-}
```
public void setValue(Object value)
```


Définit la valeur de cet objet de valeur de mise en forme conditionnelle. Il doit être utilisé en conjonction avec Type.

**Remarks**

Si la valeur est une chaîne et commence par \"=\", elle sera traitée comme une formule, sinon nous la traiterons comme une valeur simple.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.Object |  |

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

