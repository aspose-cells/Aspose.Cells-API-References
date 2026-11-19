---
title: "DocumentProperty"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente une propriété de document personnalisée ou intégrée."
type: docs
url: /fr/java/com.aspose.cells/documentproperty/
---

**Inheritance:**
java.lang.Object
```
public class DocumentProperty
```

Représente une propriété de document personnalisée ou intégrée.

**Example**

```
         //Instantiate a Workbook object
         Workbook workbook = new Workbook("book1.xls");
 
         //Retrieve a list of all custom document properties of the Excel file
         DocumentPropertyCollection customProperties = workbook.getWorksheets().getCustomDocumentProperties();
 
         //Accessng a custom document property by using the property index
         DocumentProperty customProperty1 = customProperties.get(3);
 
         //Accessng a custom document property by using the property name
         DocumentProperty customProperty2 = customProperties.get("Owner");
```
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getName()](#getName--) | Renvoie le nom de la propriété. |
| [getSource()](#getSource--) | La source du contenu lié. |
| [getType()](#getType--) | Obtient le type de données de la propriété. |
| [getValue()](#getValue--) | Obtient la valeur de la propriété. |
| [hashCode()](#hashCode--) |  |
| [isGeneratedName()](#isGeneratedName--) | Renvoie true si cette propriété n'a pas de nom dans le stockage OLE2 et qu'un nom unique a été généré uniquement pour l'API publique. |
| [isLinkedToContent()](#isLinkedToContent--) | Indique si cette propriété est liée au contenu |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setValue(Object value)](#setValue-java.lang.Object-) | Définit la valeur de la propriété. |
| [toBool()](#toBool--) | Renvoie la valeur de la propriété en tant que bool. |
| [toDateTime()](#toDateTime--) | Renvoie la valeur de la propriété en tant que DateTime dans le fuseau horaire local. |
| [toDouble()](#toDouble--) | Renvoie la valeur de la propriété en tant que double. |
| [toInt()](#toInt--) | Renvoie la valeur de la propriété en tant qu'entier. |
| [toString()](#toString--) | Renvoie la valeur de la propriété sous forme de chaîne. |
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
### getName() {#getName--}
```
public String getName()
```


Renvoie le nom de la propriété.

**Returns:**
java.lang.String
### getSource() {#getSource--}
```
public String getSource()
```


La source du contenu lié.

**Returns:**
java.lang.String
### getType() {#getType--}
```
public int getType()
```


Obtient le type de données de la propriété.

Voir [PropertyType](../../com.aspose.cells/propertytype).

**Returns:**
int
### getValue() {#getValue--}
```
public Object getValue()
```


Obtient la valeur de la propriété.

**Returns:**
java.lang.Object
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isGeneratedName() {#isGeneratedName--}
```
public boolean isGeneratedName()
```


Renvoie true si cette propriété n'a pas de nom dans le stockage OLE2 et qu'un nom unique a été généré uniquement pour l'API publique.

**Returns:**
boolean
### isLinkedToContent() {#isLinkedToContent--}
```
public boolean isLinkedToContent()
```


Indique si cette propriété est liée au contenu

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




### setValue(Object value) {#setValue-java.lang.Object-}
```
public void setValue(Object value)
```


Définit la valeur de la propriété.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.Object |  |

### toBool() {#toBool--}
```
public boolean toBool()
```


Renvoie la valeur de la propriété en tant que bool.

**Remarks**

Lance une exception si le type de propriété n'est pas PropertyType.Boolean.

**Returns:**
boolean
### toDateTime() {#toDateTime--}
```
public DateTime toDateTime()
```


Renvoie la valeur de la propriété en tant que DateTime dans le fuseau horaire local.

**Remarks**

Lance une exception si le type de propriété n'est pas PropertyType.Date.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### toDouble() {#toDouble--}
```
public double toDouble()
```


Renvoie la valeur de la propriété en tant que double.

**Remarks**

Lance une exception si le type de propriété n'est pas PropertyType.Float.

**Returns:**
double
### toInt() {#toInt--}
```
public int toInt()
```


Renvoie la valeur de la propriété en tant qu'entier.

**Remarks**

Lance une exception si le type de propriété n'est pas PropertyType.Number.

**Returns:**
int
### toString() {#toString--}
```
public String toString()
```


Renvoie la valeur de la propriété sous forme de chaîne.

**Remarks**

Convertit une propriété numérique en utilisant Object.ToString(). Convertit une propriété booléenne en "Y" ou "N". Convertit une propriété de date en une chaîne de date courte.

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

