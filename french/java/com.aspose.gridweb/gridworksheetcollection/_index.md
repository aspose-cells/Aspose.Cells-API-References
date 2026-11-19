---
title: "GridWorksheetCollection"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Encapsule une collection d'objets."
type: docs
url: /fr/java/com.aspose.gridweb/gridworksheetcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.CollectionBase](../../com.aspose.gridweb/collectionbase)
```
public class GridWorksheetCollection extends CollectionBase
```

Encapsule une collection d'objets [GridWorksheet](../../com.aspose.gridweb/gridworksheet).
## Méthodes

| Méthode | Description |
| --- | --- |
| [add()](#add--) | Ajoute une feuille de calcul à la collection. |
| [add(Object o)](#add-java.lang.Object-) | Ajoute un élément à l'instance CollectionBase. |
| [add(String sheetName)](#add-java.lang.String-) | Ajoute une feuille de calcul à la collection. |
| [addCopy(int sheetIndex)](#addCopy-int-) | Ajoute une feuille de calcul à la collection et copie les données d'une feuille de calcul existante. |
| [addCopy(String sheetName)](#addCopy-java.lang.String-) | Ajoute une feuille de calcul à la collection et copie les données d'une feuille de calcul existante. |
| [calculateFormula()](#calculateFormula--) | Calcule le résultat des formules. |
| [clear()](#clear--) | Efface toutes les feuilles de calcul. |
| [contains(Object o)](#contains-java.lang.Object-) | Renvoie si l'instance contient cet objet |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Obtient l'élément [GridWorksheet](../../com.aspose.gridweb/gridworksheet) à l'index spécifié. |
| [get(String sheetName)](#get-java.lang.String-) | Obtient l'élément [GridWorksheet](../../com.aspose.gridweb/gridworksheet) avec le nom spécifié. |
| [getActiveSheetIndex()](#getActiveSheetIndex--) | Représente l'index de la feuille de calcul active lorsque le classeur est ouvert. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Obtient la taille de l'énumérateur |
| [getDefaultFontName()](#getDefaultFontName--) | Obtient le nom de police par défaut du contrôle. |
| [getDefaultFontSize()](#getDefaultFontSize--) | ????????? |
| [getNames()](#getNames--) | Obtient la collection de tous les objets Name dans la feuille de calcul. |
| [getNumberDecimalSeparator()](#getNumberDecimalSeparator--) | Obtient le séparateur décimal pour le formatage/l'analyse des valeurs numériques. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Détermine l'index d'un élément spécifique dans l'instance CollectionBase. |
| [insert(int index, String sheetName)](#insert-int-java.lang.String-) | Insérer une feuille de calcul. |
| [iterator()](#iterator--) | Obtient l'énumérateur des lignes |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Supprime l'élément à un index spécifié. |
| [removeAt(String name)](#removeAt-java.lang.String-) | Supprime l'élément à un nom spécifié. |
| [setActiveSheetIndex(int value)](#setActiveSheetIndex-int-) | Représente l'index de la feuille de calcul active lorsque le classeur est ouvert. |
| [setDefaultFontName(String value)](#setDefaultFontName-java.lang.String-) | Définit le nom de police par défaut du contrôle. |
| [setDefaultFontSize(FontUnit value)](#setDefaultFontSize-com.aspose.gridweb.FontUnit-) | ????????? |
| [setNumberDecimalSeparator(char value)](#setNumberDecimalSeparator-char-) | Définit le séparateur décimal pour le formatage/l'analyse des valeurs numériques. |
| [setVisible(String sheetName, boolean isVisible)](#setVisible-java.lang.String-boolean-) | Définit la visibilité de la feuille. |
| [swapSheet(int sheetIndex1, int sheetIndex2)](#swapSheet-int-int-) | Échange les deux feuilles. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add() {#add--}
```
public int add()
```


Ajoute une feuille de calcul à la collection.

**Returns:**
int - index de l'objet [GridWorksheet](../../com.aspose.gridweb/gridworksheet).
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


Ajoute un élément à l'instance CollectionBase.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| o | java.lang.Object | L'objet à ajouter à l'instance CollectionBase. |

**Returns:**
int - La position dans laquelle le nouvel élément a été inséré.
### add(String sheetName) {#add-java.lang.String-}
```
public GridWorksheet add(String sheetName)
```


Ajoute une feuille de calcul à la collection.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sheetName | java.lang.String | Nom de la feuille de calcul |

**Returns:**
[GridWorksheet](../../com.aspose.gridweb/gridworksheet) - [GridWorksheet](../../com.aspose.gridweb/gridworksheet) object.
### addCopy(int sheetIndex) {#addCopy-int-}
```
public int addCopy(int sheetIndex)
```


Ajoute une feuille de calcul à la collection et copie les données d'une feuille de calcul existante.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sheetIndex | int | Index de la feuille de calcul source. |

**Returns:**
int - index de l'objet [GridWorksheet](../../com.aspose.gridweb/gridworksheet).
### addCopy(String sheetName) {#addCopy-java.lang.String-}
```
public int addCopy(String sheetName)
```


Ajoute une feuille de calcul à la collection et copie les données d'une feuille de calcul existante.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sheetName | java.lang.String | Nom de la feuille de calcul source. |

**Returns:**
int - index de l'objet [GridWorksheet](../../com.aspose.gridweb/gridworksheet).
### calculateFormula() {#calculateFormula--}
```
public void calculateFormula()
```


Calcule le résultat des formules.

### clear() {#clear--}
```
public void clear()
```


Efface toutes les feuilles de calcul.

**Remarks**

Un classeur doit contenir une feuille de calcul.

### contains(Object o) {#contains-java.lang.Object-}
```
public boolean contains(Object o)
```


Renvoie si l'instance contient cet objet

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| o | java.lang.Object | objet de test |

**Returns:**
boolean - Si l'instance contient cet objet
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
### get(int index) {#get-int-}
```
public GridWorksheet get(int index)
```


Obtient l'élément [GridWorksheet](../../com.aspose.gridweb/gridworksheet) à l'index spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | L'index de base zéro de l'élément. |

**Returns:**
[GridWorksheet](../../com.aspose.gridweb/gridworksheet) - The element at the specified index.
### get(String sheetName) {#get-java.lang.String-}
```
public GridWorksheet get(String sheetName)
```


Obtient l'élément [GridWorksheet](../../com.aspose.gridweb/gridworksheet) avec le nom spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sheetName | java.lang.String | Le nom de la feuille de calcul. |

**Returns:**
[GridWorksheet](../../com.aspose.gridweb/gridworksheet) - The GridWorksheet with the name.
### getActiveSheetIndex() {#getActiveSheetIndex--}
```
public int getActiveSheetIndex()
```


Représente l'index de la feuille de calcul active lorsque le classeur est ouvert.

**Remarks**

L'index de la feuille commence à zéro.

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCount() {#getCount--}
```
public int getCount()
```


Obtient la taille de l'énumérateur

**Returns:**
int
### getDefaultFontName() {#getDefaultFontName--}
```
public String getDefaultFontName()
```


Obtient le nom de police par défaut du contrôle.

**Example**

```
             GridWeb GridWeb1=new GridWeb();
         		GridWeb1.setDefaultFontName("Arial");
```

**Returns:**
java.lang.String
### getDefaultFontSize() {#getDefaultFontSize--}
```
public FontUnit getDefaultFontSize()
```


?????????

**Returns:**
[FontUnit](../../com.aspose.gridweb/fontunit)
### getNames() {#getNames--}
```
public GridNameCollection getNames()
```


Obtient la collection de tous les objets Name dans la feuille de calcul.

**Returns:**
[GridNameCollection](../../com.aspose.gridweb/gridnamecollection)
### getNumberDecimalSeparator() {#getNumberDecimalSeparator--}
```
public char getNumberDecimalSeparator()
```


Obtient le séparateur décimal pour le formatage/l’analyse des valeurs numériques. La valeur par défaut est le séparateur décimal de la région actuelle.

**Returns:**
char
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public int indexOf(Object o)
```


Détermine l'index d'un élément spécifique dans l'instance CollectionBase.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| o | java.lang.Object | Détermine l'index d'un élément spécifique dans l'instance CollectionBase. |

**Returns:**
int - L'index de la valeur si elle est trouvée dans la liste ; sinon, -1.
### insert(int index, String sheetName) {#insert-int-java.lang.String-}
```
public GridWorksheet insert(int index, String sheetName)
```


Insérer une feuille de calcul.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | L'index de la feuille |
| sheetName | java.lang.String |  |

**Returns:**
[GridWorksheet](../../com.aspose.gridweb/gridworksheet)
### iterator() {#iterator--}
```
public Iterator iterator()
```


Obtient l'énumérateur des lignes

**Returns:**
java.util.Iterator - L'énumérateur des lignes
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Supprime l'élément à un index spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | La valeur d'index de l'élément à supprimer. |

### removeAt(String name) {#removeAt-java.lang.String-}
```
public void removeAt(String name)
```


Supprime l'élément à un nom spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| name | java.lang.String | Le nom de l'élément à supprimer. |

### setActiveSheetIndex(int value) {#setActiveSheetIndex-int-}
```
public void setActiveSheetIndex(int value)
```


Représente l'index de la feuille de calcul active lorsque le classeur est ouvert.

**Remarks**

L'index de la feuille commence à zéro.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setDefaultFontName(String value) {#setDefaultFontName-java.lang.String-}
```
public void setDefaultFontName(String value)
```


Définit le nom de police par défaut du contrôle.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setDefaultFontSize(FontUnit value) {#setDefaultFontSize-com.aspose.gridweb.FontUnit-}
```
public void setDefaultFontSize(FontUnit value)
```


?????????

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [FontUnit](../../com.aspose.gridweb/fontunit) |  |

### setNumberDecimalSeparator(char value) {#setNumberDecimalSeparator-char-}
```
public void setNumberDecimalSeparator(char value)
```


Définit le séparateur décimal pour le formatage/l'analyse des valeurs numériques. La valeur par défaut est le séparateur décimal de la région actuelle.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | char |  |

### setVisible(String sheetName, boolean isVisible) {#setVisible-java.lang.String-boolean-}
```
public void setVisible(String sheetName, boolean isVisible)
```


Définit la visibilité de la feuille.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sheetName | java.lang.String | Nom de la feuille de calcul source. |
| isVisible | boolean | Si la feuille de calcul est visible |

### swapSheet(int sheetIndex1, int sheetIndex2) {#swapSheet-int-int-}
```
public void swapSheet(int sheetIndex1, int sheetIndex2)
```


Échange les deux feuilles.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sheetIndex1 | int | La première feuille de calcul. |
| sheetIndex2 | int | La deuxième feuille de calcul. |

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

