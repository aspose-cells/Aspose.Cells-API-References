---
title: "SignificantDigitsType"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente le type de chiffres significatifs pour la sortie des valeurs numériques."
type: docs
url: /fr/java/com.aspose.cells/significantdigitstype/
---

**Inheritance:**
java.lang.Object
```
public final class SignificantDigitsType
```

Représente le type de chiffres significatifs pour la sortie des valeurs numériques.
## Champs

| Champ | Description |
| --- | --- |
| [DIGITS_15](#DIGITS-15) | 15 chiffres |
| [G_17](#G-17) | 17 chiffres en formatant la valeur avec "G17". |
| [ROUNDING_17](#ROUNDING-17) | 17 chiffres en arrondissant la valeur. |
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
### DIGITS_15 {#DIGITS-15}
```
public static final int DIGITS_15
```


15 chiffres

### G_17 {#G-17}
```
public static final int G_17
```


17 chiffres en formatant la valeur avec "G17".

**Remarks**

Pour certaines valeurs double, "G17" peut donner une valeur différente de celle originale/littérale saisie par l'utilisateur. Par exemple, la valeur double 0.15 sera affichée comme 0.14999999999999999 ; la valeur double 1.0E-16 sera affichée comme 9.9999999999999998E-17. Excel gère ces valeurs de manière incohérente, il enregistre 0.15 comme 0.15 dans le fichier xlsx, mais pour 1.0E-16 la valeur enregistrée dans le fichier xlsx est 9.9999999999999998E-17.

### ROUNDING_17 {#ROUNDING-17}
```
public static final int ROUNDING_17
```


17 chiffres en arrondissant la valeur.

**Remarks**

Ce type renvoie généralement la valeur telle qu'elle a été saisie par l'utilisateur, originale/littérale. Pour 0.15 il produit "0.15" et pour 1.0E-16 il produit "1.0E-16". Mais il existe également des cas particuliers qui peuvent donner des valeurs différentes de la littérale. Par exemple, lors de l'arrondi de 208435494.96478021 à 17 chiffres ("0.\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#\#"), le résultat est 208435494.96478.

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

