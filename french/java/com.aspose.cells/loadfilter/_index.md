---
title: "LoadFilter"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Représente le filtre qui fournit des options pour charger les données lors du chargement du classeur à partir d'un modèle."
type: docs
url: /fr/java/com.aspose.cells/loadfilter/
---

**Inheritance:**
java.lang.Object
```
public class LoadFilter
```

Représente le filtre qui fournit des options pour charger les données lors du chargement du classeur à partir d'un modèle.

**Remarks**

L'utilisateur peut spécifier les options de filtre ou implémenter son propre LoadFilter pour définir comment charger les données.

**Example**

L'exemple suivant montre comment déterminer les options de filtre en fonction des propriétés de la feuille de calcul.

```
         class LoadFilterSheet extends LoadFilter
         {
             public /*override*/ void startSheet(Worksheet sheet) 
             {
                 if ("Sheet1".equals(sheet.getName()))
                 {
                     setLoadDataFilterOptions(LoadDataFilterOptions.ALL);
                 }
                 else
                 {
                     setLoadDataFilterOptions(LoadDataFilterOptions.STRUCTURE);
                 }
             }
         }
         LoadOptions opts = new LoadOptions();
         opts.setLoadFilter(new LoadFilterSheet());
         Workbook wb = new Workbook("template.xlsx", opts);
         //Custom LoadFilter implementation
```
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [LoadFilter()](#LoadFilter--) | Construit un LoadFilter avec les options de filtre par défaut LoadDataFilterOptions.All. |
| [LoadFilter(int opts)](#LoadFilter-int-) | Construit un LoadFilter avec les options de filtre fournies. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getLoadDataFilterOptions()](#getLoadDataFilterOptions--) | Les options de filtre pour indiquer quelles données doivent être chargées. |
| [getSheetsInLoadingOrder()](#getSheetsInLoadingOrder--) | Spécifie les feuilles (indices) et l'ordre à charger. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setLoadDataFilterOptions(int value)](#setLoadDataFilterOptions-int-) | Les options de filtre pour indiquer quelles données doivent être chargées. |
| [startSheet(Worksheet sheet)](#startSheet-com.aspose.cells.Worksheet-) | Prépare les options de filtre avant de charger la feuille de calcul donnée. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### LoadFilter() {#LoadFilter--}
```
public LoadFilter()
```


Construit un LoadFilter avec les options de filtre par défaut LoadDataFilterOptions.All.

### LoadFilter(int opts) {#LoadFilter-int-}
```
public LoadFilter(int opts)
```


Construit un LoadFilter avec les options de filtre fournies.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| opts | int | [LoadDataFilterOptions](../../com.aspose.cells/loaddatafilteroptions). les options de filtre par défaut |

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
### getLoadDataFilterOptions() {#getLoadDataFilterOptions--}
```
public int getLoadDataFilterOptions()
```


Les options de filtre pour indiquer quelles données doivent être chargées.

Voir [LoadDataFilterOptions](../../com.aspose.cells/loaddatafilteroptions).

**Returns:**
int
### getSheetsInLoadingOrder() {#getSheetsInLoadingOrder--}
```
public int[] getSheetsInLoadingOrder()
```


Spécifie les feuilles (indices) et l'ordre à charger. La valeur par défaut est null, ce qui indique de charger toutes les feuilles dans l'ordre par défaut du fichier modèle. Si ce n'est pas null et que l'index d'une feuille n'est pas présent dans le tableau retourné, alors la feuille ne sera pas chargée.

**Returns:**
int[]
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




### setLoadDataFilterOptions(int value) {#setLoadDataFilterOptions-int-}
```
public void setLoadDataFilterOptions(int value)
```


Les options de filtre pour indiquer quelles données doivent être chargées.

Voir [LoadDataFilterOptions](../../com.aspose.cells/loaddatafilteroptions).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### startSheet(Worksheet sheet) {#startSheet-com.aspose.cells.Worksheet-}
```
public void startSheet(Worksheet sheet)
```


Prépare les options de filtre avant de charger la feuille de calcul donnée. L'implémentation de LoadFilter par l'utilisateur peut modifier les LoadDataFilterOptions ici pour indiquer comment charger les données pour cette feuille de calcul.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| sheet | [Worksheet](../../com.aspose.cells/worksheet) | La feuille de calcul à charger. Seules quelques propriétés peuvent être utilisées pour l'objet feuille de calcul donné ici car la plupart des données et propriétés n'ont pas été chargées. Les propriétés disponibles sont : Name, Index, VisibilityType |

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

