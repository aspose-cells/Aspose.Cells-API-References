---
title: "CustomFunctionDefinition"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Définition d'une fonction personnalisée pour le calcul avec le moteur personnalisé de l'utilisateur."
type: docs
url: /fr/java/com.aspose.cells/customfunctiondefinition/
---

**Inheritance:**
java.lang.Object
```
public class CustomFunctionDefinition
```

Définition d'une fonction personnalisée pour le calcul avec le moteur personnalisé de l'utilisateur.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [CustomFunctionDefinition()](#CustomFunctionDefinition--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArrayModeParameters(String functionName)](#getArrayModeParameters-java.lang.String-) | Obtient les indices des paramètres de la fonction personnalisée donnée qui doivent être calculés en mode tableau. |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### CustomFunctionDefinition() {#CustomFunctionDefinition--}
```
public CustomFunctionDefinition()
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
### getArrayModeParameters(String functionName) {#getArrayModeParameters-java.lang.String-}
```
public int[] getArrayModeParameters(String functionName)
```


Obtient les indices des paramètres de la fonction personnalisée donnée qui doivent être calculés en mode tableau.

**Remarks**

Pour une expression qui doit être calculée, en prenant A:A+B:B comme exemple : généralement en mode valeur, elle sera calculée en une seule valeur selon la base de la cellule actuelle. Mais en mode tableau, toutes les valeurs de A1+B1, A2+B2, A3+B3, ... seront calculées et utilisées pour le calcul.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| functionName | java.lang.String | Nom de la fonction personnalisée. |

**Returns:**
int[] - Indices des paramètres qui doivent être calculés en mode tableau pour la fonction personnalisée donnée. La valeur par défaut est null, aucun paramètre ne doit être calculé en mode tableau pour la fonction personnalisée.
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

