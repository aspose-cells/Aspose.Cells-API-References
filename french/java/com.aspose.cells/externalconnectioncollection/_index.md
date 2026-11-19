---
title: "ExternalConnectionCollection"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Spécifie la collection"
type: docs
url: /fr/java/com.aspose.cells/externalconnectioncollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class ExternalConnectionCollection extends CollectionBase
```

Spécifie la collection [ExternalConnection](../../com.aspose.cells/externalconnection)

**Example**

```
         Workbook wb = new Workbook("connection.xlsx");
         ExternalConnectionCollection dataConns = wb.getDataConnections();
         ExternalConnection dataConn = null;
         for (int i = 0; i <dataConns.getCount(); i++)
         {
             dataConn = dataConns.get(i);
             //get external connection id
             System.out.println(dataConn.getConnectionId());
         }
```
## Méthodes

| Méthode | Description |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | Ajoute un élément à l'instance CollectionBase. |
| [clear()](#clear--) | Supprime tous les objets de l'instance CollectionBase. |
| [contains(Object o)](#contains-java.lang.Object-) | Renvoie si l'instance contient cet objet |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Obtient l'élément [ExternalConnection](../../com.aspose.cells/externalconnection) à l'index spécifié. |
| [get(String connectionName)](#get-java.lang.String-) | Obtient l'élément [ExternalConnection](../../com.aspose.cells/externalconnection) avec le nom spécifié. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Obtient le nombre d'éléments contenus dans l'instance CollectionBase. |
| [getExternalConnectionById(int connId)](#getExternalConnectionById-int-) | Obtient l'élément [ExternalConnection](../../com.aspose.cells/externalconnection) avec l'identifiant spécifié. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Détermine l'index d'un élément spécifique dans l'instance CollectionBase. |
| [iterator()](#iterator--) | Renvoie un énumérateur qui parcourt l'instance CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Supprime l'élément à l'index spécifié. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### clear() {#clear--}
```
public void clear()
```


Supprime tous les objets de l'instance CollectionBase.

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
public ExternalConnection get(int index)
```


Obtient l'élément [ExternalConnection](../../com.aspose.cells/externalconnection) à l'index spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | L'index de base zéro de l'élément. |

**Returns:**
[ExternalConnection](../../com.aspose.cells/externalconnection) - The element at the specified index.
### get(String connectionName) {#get-java.lang.String-}
```
public ExternalConnection get(String connectionName)
```


Obtient l'élément [ExternalConnection](../../com.aspose.cells/externalconnection) avec le nom spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| connectionName | java.lang.String | le nom de la connexion de données |

**Returns:**
[ExternalConnection](../../com.aspose.cells/externalconnection) - The element with the specified name.
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


Obtient le nombre d'éléments contenus dans l'instance CollectionBase.

**Returns:**
int - Le nombre d'éléments contenus dans l'instance CollectionBase.
### getExternalConnectionById(int connId) {#getExternalConnectionById-int-}
```
public ExternalConnection getExternalConnectionById(int connId)
```


Obtient l'élément [ExternalConnection](../../com.aspose.cells/externalconnection) avec l'identifiant spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| connId | int | identifiant de connexion externe |

**Returns:**
[ExternalConnection](../../com.aspose.cells/externalconnection) - The element with the specified id.
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
### iterator() {#iterator--}
```
public Iterator iterator()
```


Renvoie un énumérateur qui parcourt l'instance CollectionBase.

**Returns:**
java.util.Iterator - Un itérateur pour l'instance CollectionBase.
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


Supprime l'élément à l'index spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | L'index basé sur zéro de l'élément à supprimer. |

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

