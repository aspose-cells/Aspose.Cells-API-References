---
title: "VbaProjectReferenceCollection"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente toutes les références du projet VBA."
type: docs
url: /fr/java/com.aspose.cells/vbaprojectreferencecollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class VbaProjectReferenceCollection extends CollectionBase
```

Représente toutes les références du projet VBA.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
          // Init VBA project.
         VbaProject vbaProject = workbook.getVbaProject();
         // Add vba project reference
         vbaProject.getReferences().addRegisteredReference("stdole", "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");
         //Saving the Excel file
         workbook.save("book1.xlsm");
```
## Méthodes

| Méthode | Description |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | Ajoute un élément à l'instance CollectionBase. |
| [addControlReferernce(String name, String libid, String twiddledlibid, String extendedLibid)](#addControlReferernce-java.lang.String-java.lang.String-java.lang.String-java.lang.String-) | Ajoutez une référence à une bibliothèque de types modifiée et à sa bibliothèque de types étendue. |
| [addControlRefrernce(String name, String libid, String twiddledlibid, String extendedLibid)](#addControlRefrernce-java.lang.String-java.lang.String-java.lang.String-java.lang.String-) | Ajoutez une référence à une bibliothèque de types modifiée et à sa bibliothèque de types étendue. |
| [addProjectReferernce(String name, String absoluteLibid, String relativeLibid)](#addProjectReferernce-java.lang.String-java.lang.String-java.lang.String-) | Ajoute une référence à un projet VBA externe. |
| [addProjectRefrernce(String name, String absoluteLibid, String relativeLibid)](#addProjectRefrernce-java.lang.String-java.lang.String-java.lang.String-) | Ajoute une référence à un projet VBA externe. |
| [addRegisteredReference(String name, String libid)](#addRegisteredReference-java.lang.String-java.lang.String-) | Ajoutez une référence à une bibliothèque de types Automation. |
| [clear()](#clear--) | Supprime tous les objets de l'instance CollectionBase. |
| [contains(Object o)](#contains-java.lang.Object-) | Renvoie si l'instance contient cet objet |
| [copy(VbaProjectReferenceCollection source)](#copy-com.aspose.cells.VbaProjectReferenceCollection-) | Copie les références d'un autre projet VBA. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int i)](#get-int-) | Obtenez la référence dans la liste par son index. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Obtient le nombre d'éléments contenus dans l'instance CollectionBase. |
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
### addControlReferernce(String name, String libid, String twiddledlibid, String extendedLibid) {#addControlReferernce-java.lang.String-java.lang.String-java.lang.String-java.lang.String-}
```
public int addControlReferernce(String name, String libid, String twiddledlibid, String extendedLibid)
```


Ajoutez une référence à une bibliothèque de types modifiée et à sa bibliothèque de types étendue.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| name | java.lang.String | Le nom de la référence. |
| libid | java.lang.String | L'identifiant d'une bibliothèque de types Automation. |
| twiddledlibid | java.lang.String | L'identifiant d'une bibliothèque de types modifiée. |
| extendedLibid | java.lang.String | L'identifiant d'une bibliothèque de types étendue. |

**Returns:**
int -
### addControlRefrernce(String name, String libid, String twiddledlibid, String extendedLibid) {#addControlRefrernce-java.lang.String-java.lang.String-java.lang.String-java.lang.String-}
```
public int addControlRefrernce(String name, String libid, String twiddledlibid, String extendedLibid)
```


Ajoutez une référence à une bibliothèque de types modifiée et à sa bibliothèque de types étendue.

**Remarks**

NOTE : Cette méthode est maintenant obsolète. À la place, veuillez utiliser la méthode VbaProjectReferenceCollection.AddControlReferernce(). Cette méthode sera supprimée 12 mois après, depuis juillet 2026. Aspose s'excuse pour tout inconvénient que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| name | java.lang.String | Le nom de la référence. |
| libid | java.lang.String | L'identifiant d'une bibliothèque de types Automation. |
| twiddledlibid | java.lang.String | L'identifiant d'une bibliothèque de types modifiée. |
| extendedLibid | java.lang.String | L'identifiant d'une bibliothèque de types étendue. |

**Returns:**
int -
### addProjectReferernce(String name, String absoluteLibid, String relativeLibid) {#addProjectReferernce-java.lang.String-java.lang.String-java.lang.String-}
```
public int addProjectReferernce(String name, String absoluteLibid, String relativeLibid)
```


Ajoute une référence à un projet VBA externe.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| name | java.lang.String | Le nom de la référence. |
| absoluteLibid | java.lang.String | L'identifiant du projet VBA référencé avec un chemin absolu. |
| relativeLibid | java.lang.String | L'identifiant du projet VBA référencé avec un chemin relatif. |

**Returns:**
int -
### addProjectRefrernce(String name, String absoluteLibid, String relativeLibid) {#addProjectRefrernce-java.lang.String-java.lang.String-java.lang.String-}
```
public int addProjectRefrernce(String name, String absoluteLibid, String relativeLibid)
```


Ajoute une référence à un projet VBA externe.

**Remarks**

NOTE : Cette méthode est maintenant obsolète. À la place, veuillez utiliser la méthode VbaProjectReferenceCollection.AddProjectReferernce(). Cette méthode sera supprimée 12 mois après, depuis juillet 2026. Aspose s'excuse pour tout inconvénient que vous auriez pu rencontrer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| name | java.lang.String | Le nom de la référence. |
| absoluteLibid | java.lang.String | L'identifiant du projet VBA référencé avec un chemin absolu. |
| relativeLibid | java.lang.String | L'identifiant du projet VBA référencé avec un chemin relatif. |

**Returns:**
int -
### addRegisteredReference(String name, String libid) {#addRegisteredReference-java.lang.String-java.lang.String-}
```
public int addRegisteredReference(String name, String libid)
```


Ajoutez une référence à une bibliothèque de types Automation.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| name | java.lang.String | Le nom de la référence. |
| libid | java.lang.String | L'identifiant d'une bibliothèque de types Automation. |

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
### copy(VbaProjectReferenceCollection source) {#copy-com.aspose.cells.VbaProjectReferenceCollection-}
```
public void copy(VbaProjectReferenceCollection source)
```


Copie les références d'un autre projet VBA.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| source | [VbaProjectReferenceCollection](../../com.aspose.cells/vbaprojectreferencecollection) | Les références sources. |

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
### get(int i) {#get-int-}
```
public VbaProjectReference get(int i)
```


Obtenez la référence dans la liste par son index.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| i | int | L'index. |

**Returns:**
[VbaProjectReference](../../com.aspose.cells/vbaprojectreference) - 
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

