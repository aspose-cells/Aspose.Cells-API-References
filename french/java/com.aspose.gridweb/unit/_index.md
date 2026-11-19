---
title: "Unit"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente une mesure de longueur"
type: docs
url: /fr/java/com.aspose.gridweb/unit/
---

**Inheritance:**
java.lang.Object
```
public class Unit
```

Représente une mesure de longueur
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [Unit()](#Unit--) | le constructeur par défaut |
| [Unit(double value, int type)](#Unit-double-int-) | Initialise une nouvelle instance de la structure Unit avec le nombre à virgule flottante double précision spécifié et le UnitType. |
| [Unit(double value)](#Unit-double-) | Initialise une nouvelle instance de la structure Unit avec le nombre à virgule flottante double précision spécifié. |
| [Unit(int value)](#Unit-int-) | Initialise une nouvelle instance de la structure Unit avec l'entier signé 32 bits spécifié. |
| [Unit(String value)](#Unit-java.lang.String-) | Initialise une nouvelle instance de la structure Unit avec la longueur spécifiée. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [GetExtension(int type)](#GetExtension-int-) | obtenir la chaîne selon le type, peut obtenir "px" "pt" "%" et ainsi de suite ; |
| [Parse(String s)](#Parse-java.lang.String-) | Convertit la chaîne spécifiée en Unit. |
| [Percentage(double n)](#Percentage-double-) | Crée un Unit de type Percentage à partir du nombre à virgule flottante double précision spécifié. |
| [Pixel(int n)](#Pixel-int-) | Crée un Unit de type Pixel à partir de l'entier signé 32 bits spécifié. |
| [Point(int n)](#Point-int-) | Crée un Unit de type Point à partir de l'entier signé 32 bits spécifié. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getType()](#getType--) | Obtient le type d'unité du Unit. |
| [getValue()](#getValue--) | Obtient la longueur du Unit. |
| [hashCode()](#hashCode--) |  |
| [isEmpty()](#isEmpty--) | Obtient une valeur indiquant si le Unit est vide. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) | obtenir la représentation sous forme de chaîne du Unit. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### Unit() {#Unit--}
```
public Unit()
```


le constructeur par défaut

### Unit(double value, int type) {#Unit-double-int-}
```
public Unit(double value, int type)
```


Initialise une nouvelle instance de la structure Unit avec le nombre à virgule flottante double précision spécifié et le UnitType.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |
| type | int |  |

### Unit(double value) {#Unit-double-}
```
public Unit(double value)
```


Initialise une nouvelle instance de la structure Unit avec le nombre à virgule flottante double précision spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | double |  |

### Unit(int value) {#Unit-int-}
```
public Unit(int value)
```


Initialise une nouvelle instance de la structure Unit avec l'entier signé 32 bits spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### Unit(String value) {#Unit-java.lang.String-}
```
public Unit(String value)
```


Initialise une nouvelle instance de la structure Unit avec la longueur spécifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### GetExtension(int type) {#GetExtension-int-}
```
public static String GetExtension(int type)
```


obtenir la chaîne selon le type, peut obtenir "px" "pt" "%" et ainsi de suite ;

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| type | int |  |

**Returns:**
java.lang.String
### Parse(String s) {#Parse-java.lang.String-}
```
public static Unit Parse(String s)
```


Convertit la chaîne spécifiée en Unit.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| s | java.lang.String |  |

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### Percentage(double n) {#Percentage-double-}
```
public static Unit Percentage(double n)
```


Crée un Unit de type Percentage à partir du nombre à virgule flottante double précision spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| n | double |  |

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### Pixel(int n) {#Pixel-int-}
```
public static Unit Pixel(int n)
```


Crée un Unit de type Pixel à partir de l'entier signé 32 bits spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| n | int |  |

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
### Point(int n) {#Point-int-}
```
public static Unit Point(int n)
```


Crée un Unit de type Point à partir de l'entier signé 32 bits spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| n | int |  |

**Returns:**
[Unit](../../com.aspose.gridweb/unit)
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


Obtient le type d'unité du Unit.

**Returns:**
int
### getValue() {#getValue--}
```
public double getValue()
```


Obtient la longueur du Unit.

**Returns:**
double
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isEmpty() {#isEmpty--}
```
public boolean isEmpty()
```


Obtient une valeur indiquant si le Unit est vide.

**Returns:**
boolean -
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


obtenir la représentation sous forme de chaîne du Unit.

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

