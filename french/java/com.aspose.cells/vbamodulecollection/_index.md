---
title: "VbaModuleCollection"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente la liste de"
type: docs
url: /fr/java/com.aspose.cells/vbamodulecollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class VbaModuleCollection extends CollectionBase
```

Représente la liste de [VbaModule](../../com.aspose.cells/vbamodule)

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
          // Init VBA project.
         VbaProject vbaProject = workbook.getVbaProject(); 
         // Add a new module.
         vbaProject.getModules().add(VbaModuleType.CLASS, "test");
         //Saving the Excel file
         workbook.save("book1.xlsm");
```
## Méthodes

| Méthode | Description |
| --- | --- |
| [add(Worksheet sheet)](#add-com.aspose.cells.Worksheet-) | Ajoute un module pour une feuille de calcul. |
| [add(int type, String name)](#add-int-java.lang.String-) | Ajoute un module. |
| [add(Object o)](#add-java.lang.Object-) | Ajoute un élément à l'instance CollectionBase. |
| [addDesignerStorage(String name, byte[] data)](#addDesignerStorage-java.lang.String-byte---) |  |
| [addUserForm(String name, String codes, byte[] designerStorage)](#addUserForm-java.lang.String-java.lang.String-byte---) | Insère le formulaire utilisateur dans le projet VBA. |
| [clear()](#clear--) | Supprime tous les objets de l'instance CollectionBase. |
| [contains(Object o)](#contains-java.lang.Object-) | Renvoie si l'instance contient cet objet |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Obtient [VbaModule](../../com.aspose.cells/vbamodule) dans la liste par l'index. |
| [get(String name)](#get-java.lang.String-) | Obtient [VbaModule](../../com.aspose.cells/vbamodule) dans la liste par le nom. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Obtient le nombre d'éléments contenus dans l'instance CollectionBase. |
| [getDesignerStorage(String name)](#getDesignerStorage-java.lang.String-) | Représente les données du Concepteur. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Détermine l'index d'un élément spécifique dans l'instance CollectionBase. |
| [iterator()](#iterator--) | Renvoie un énumérateur qui parcourt l'instance CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(Worksheet sheet)](#remove-com.aspose.cells.Worksheet-) | Supprime le module d'une feuille de calcul. |
| [remove(String name)](#remove-java.lang.String-) | Supprime le module par le nom |
| [removeAt(int index)](#removeAt-int-) | Supprime l'élément à l'index spécifié. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(Worksheet sheet) {#add-com.aspose.cells.Worksheet-}
```
public int add(Worksheet sheet)
```


Ajoute un module pour une feuille de calcul.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sheet | [Worksheet](../../com.aspose.cells/worksheet) | La feuille de calcul |

**Returns:**
int -
### add(int type, String name) {#add-int-java.lang.String-}
```
public int add(int type, String name)
```


Ajoute un module.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| type | int | [VbaModuleType](../../com.aspose.cells/vbamoduletype). Le type de module. |
| name | java.lang.String | Le nom du module. |

**Returns:**
int -
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
### addDesignerStorage(String name, byte[] data) {#addDesignerStorage-java.lang.String-byte---}
```
public void addDesignerStorage(String name, byte[] data)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| name | java.lang.String |  |
| données | byte[] |  |

### addUserForm(String name, String codes, byte[] designerStorage) {#addUserForm-java.lang.String-java.lang.String-byte---}
```
public int addUserForm(String name, String codes, byte[] designerStorage)
```


Insère le formulaire utilisateur dans le projet VBA.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| name | java.lang.String | Le nom du formulaire utilisateur |
| codes | java.lang.String | Les codes du formulaire utilisateur |
| designerStorage | byte[] | les paramètres du concepteur concernant le formulaire utilisateur |

**Returns:**
int -
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
public VbaModule get(int index)
```


Obtient [VbaModule](../../com.aspose.cells/vbamodule) dans la liste par l'index.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| index | int | L'index. |

**Returns:**
[VbaModule](../../com.aspose.cells/vbamodule) - 
### get(String name) {#get-java.lang.String-}
```
public VbaModule get(String name)
```


Obtient [VbaModule](../../com.aspose.cells/vbamodule) dans la liste par le nom.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| name | java.lang.String | Le nom du module. |

**Returns:**
[VbaModule](../../com.aspose.cells/vbamodule) - 
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
### getDesignerStorage(String name) {#getDesignerStorage-java.lang.String-}
```
public byte[] getDesignerStorage(String name)
```


Représente les données du Concepteur.

**Remarks**

Nous ne supportons pas l'analyse de ceux-ci. Seulement pour la copie.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
byte[]
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




### remove(Worksheet sheet) {#remove-com.aspose.cells.Worksheet-}
```
public void remove(Worksheet sheet)
```


Supprime le module d'une feuille de calcul.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sheet | [Worksheet](../../com.aspose.cells/worksheet) | La feuille de calcul |

### remove(String name) {#remove-java.lang.String-}
```
public void remove(String name)
```


Supprime le module par le nom

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| name | java.lang.String |  |

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

