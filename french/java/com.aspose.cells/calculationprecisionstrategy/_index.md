---
title: "CalculationPrecisionStrategy"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Énumère les stratégies de gestion de la précision du calcul."
type: docs
url: /fr/java/com.aspose.cells/calculationprecisionstrategy/
---

**Inheritance:**
java.lang.Object
```
public final class CalculationPrecisionStrategy
```

Énumère les stratégies de gestion de la précision des calculs. En raison du problème de précision de l'arithmétique à virgule flottante IEEE 754, certaines formules "apparemment simples" peuvent ne pas être calculées avec le résultat attendu. Par exemple la formule "=-0.45+0.43+0.02", lorsqu'on calcule les opérandes avec l'opérateur '+' directement, le résultat n'est pas zéro. Pour ce type de problème de précision, certaines stratégies spéciales peuvent fournir le résultat attendu.
## Champs

| Champ | Description |
| --- | --- |
| [DECIMAL](#DECIMAL) | Utilise le décimal comme opérandes lorsque cela est possible. |
| [NONE](#NONE) | Aucune stratégie appliquée au calcul. |
| [ROUND](#ROUND) | Arrondit le résultat du calcul en fonction des chiffres significatifs. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### DECIMAL {#DECIMAL}
```
public static final int DECIMAL
```


Utilise le type décimal comme opérandes lorsque c'est possible. Le moins efficace en termes de performances.

### NONE {#NONE}
```
public static final int NONE
```


Aucune stratégie appliquée au calcul. Lors du calcul, utilisez simplement la valeur double originale comme opérande et renvoyez le résultat directement. Le plus efficace en termes de performances et applicable dans la plupart des cas.

### ROUND {#ROUND}
```
public static final int ROUND
```


Arrondit le résultat du calcul en fonction des chiffres significatifs.

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

