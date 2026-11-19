---
title: "ConnectionParameter"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Spécifie les propriétés de tous les paramètres utilisés avec les connexions de données externes. Les paramètres sont valides pour ODBC et les requêtes Web."
type: docs
url: /fr/java/com.aspose.cells/connectionparameter/
---

**Inheritance:**
java.lang.Object
```
public class ConnectionParameter
```

Spécifie les propriétés de tous les paramètres utilisés avec les connexions de données externes. Les paramètres sont valides pour ODBC et les requêtes Web.
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCellReference()](#getCellReference--) | Référence de cellule indiquant la valeur de quelle cellule utiliser pour le paramètre de requête. |
| [getClass()](#getClass--) |  |
| [getName()](#getName--) | Le nom du paramètre. |
| [getPrompt()](#getPrompt--) | Chaîne d’invite pour le paramètre. |
| [getRefreshOnChange()](#getRefreshOnChange--) | Indicateur indiquant si la requête doit se rafraîchir automatiquement lorsque le contenu d’une cellule fournissant la valeur du paramètre change. |
| [getSqlType()](#getSqlType--) | Type de données SQL du paramètre. |
| [getType()](#getType--) | Type de paramètre utilisé. |
| [getValue()](#getValue--) | Valeur numérique non entière, valeur entière, valeur de chaîne ou valeur booléenne à utiliser comme paramètre de requête. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCellReference(String value)](#setCellReference-java.lang.String-) | Référence de cellule indiquant la valeur de quelle cellule utiliser pour le paramètre de requête. |
| [setName(String value)](#setName-java.lang.String-) | Le nom du paramètre. |
| [setPrompt(String value)](#setPrompt-java.lang.String-) | Chaîne d’invite pour le paramètre. |
| [setRefreshOnChange(boolean value)](#setRefreshOnChange-boolean-) | Indicateur indiquant si la requête doit se rafraîchir automatiquement lorsque le contenu d’une cellule fournissant la valeur du paramètre change. |
| [setSqlType(int value)](#setSqlType-int-) | Type de données SQL du paramètre. |
| [setType(int value)](#setType-int-) | Type de paramètre utilisé. |
| [setValue(Object value)](#setValue-java.lang.Object-) | Valeur numérique non entière, valeur entière, valeur de chaîne ou valeur booléenne à utiliser comme paramètre de requête. |
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
### getCellReference() {#getCellReference--}
```
public String getCellReference()
```


Référence de cellule indiquant la valeur de quelle cellule utiliser pour le paramètre de requête. Utilisée uniquement lorsque parameterType est cell.

**Returns:**
java.lang.String
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getName() {#getName--}
```
public String getName()
```


Le nom du paramètre.

**Returns:**
java.lang.String
### getPrompt() {#getPrompt--}
```
public String getPrompt()
```


Chaîne d’invite pour le paramètre. Présentée à l’utilisateur de la feuille de calcul avec une interface d’entrée pour recueillir la valeur du paramètre avant de rafraîchir les données externes. Utilisée uniquement lorsque parameterType = prompt.

**Returns:**
java.lang.String
### getRefreshOnChange() {#getRefreshOnChange--}
```
public boolean getRefreshOnChange()
```


Indicateur indiquant si la requête doit se rafraîchir automatiquement lorsque le contenu d’une cellule fournissant la valeur du paramètre change. Si vrai, les données externes sont rafraîchies en utilisant la nouvelle valeur du paramètre à chaque modification. Si faux, les données externes ne sont rafraîchies que lorsqu’elles sont demandées par l’utilisateur, ou lorsqu’un autre événement déclenche le rafraîchissement (par ex., le classeur ouvert).

**Returns:**
boolean
### getSqlType() {#getSqlType--}
```
public int getSqlType()
```


Type de données SQL du paramètre. Valide uniquement pour les sources ODBC.

Voir [SqlDataType](../../com.aspose.cells/sqldatatype).

**Returns:**
int
### getType() {#getType--}
```
public int getType()
```


Type de paramètre utilisé. Si parameterType=value, alors la valeur provenant de boolean, double, integer ou string sera utilisée. Dans ce cas, il est attendu qu’une seule des \{boolean, double, integer, or string\} soit spécifiée.

Voir [ConnectionParameterType](../../com.aspose.cells/connectionparametertype).

**Returns:**
int
### getValue() {#getValue--}
```
public Object getValue()
```


Valeur numérique non entière, valeur entière, valeur de chaîne ou valeur booléenne à utiliser comme paramètre de requête. Utilisée uniquement lorsque parameterType est value.

**Returns:**
java.lang.Object
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




### setCellReference(String value) {#setCellReference-java.lang.String-}
```
public void setCellReference(String value)
```


Référence de cellule indiquant la valeur de quelle cellule utiliser pour le paramètre de requête. Utilisée uniquement lorsque parameterType est cell.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Le nom du paramètre.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setPrompt(String value) {#setPrompt-java.lang.String-}
```
public void setPrompt(String value)
```


Chaîne d’invite pour le paramètre. Présentée à l’utilisateur de la feuille de calcul avec une interface d’entrée pour recueillir la valeur du paramètre avant de rafraîchir les données externes. Utilisée uniquement lorsque parameterType = prompt.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setRefreshOnChange(boolean value) {#setRefreshOnChange-boolean-}
```
public void setRefreshOnChange(boolean value)
```


Indicateur indiquant si la requête doit se rafraîchir automatiquement lorsque le contenu d’une cellule fournissant la valeur du paramètre change. Si vrai, les données externes sont rafraîchies en utilisant la nouvelle valeur du paramètre à chaque modification. Si faux, les données externes ne sont rafraîchies que lorsqu’elles sont demandées par l’utilisateur, ou lorsqu’un autre événement déclenche le rafraîchissement (par ex., le classeur ouvert).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setSqlType(int value) {#setSqlType-int-}
```
public void setSqlType(int value)
```


Type de données SQL du paramètre. Valide uniquement pour les sources ODBC.

Voir [SqlDataType](../../com.aspose.cells/sqldatatype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


Type de paramètre utilisé. Si parameterType=value, alors la valeur provenant de boolean, double, integer ou string sera utilisée. Dans ce cas, il est attendu qu’une seule des \{boolean, double, integer, or string\} soit spécifiée.

Voir [ConnectionParameterType](../../com.aspose.cells/connectionparametertype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setValue(Object value) {#setValue-java.lang.Object-}
```
public void setValue(Object value)
```


Valeur numérique non entière, valeur entière, valeur de chaîne ou valeur booléenne à utiliser comme paramètre de requête. Utilisée uniquement lorsque parameterType est value.

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

