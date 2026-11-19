---
title: "MemorySetting"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Modes d'utilisation de la mémoire pour le modèle de données des cellules."
type: docs
url: /fr/java/com.aspose.cells/memorysetting/
---

**Inheritance:**
java.lang.Object
```
public final class MemorySetting
```

Modes d'utilisation de la mémoire pour le modèle de données des cellules.
## Champs

| Champ | Description |
| --- | --- |
| [FILE_CACHE](#FILE-CACHE) | Des performances mémoire préférables et l'utilisation d'un fichier au lieu de la mémoire pour maintenir les données des cellules. |
| [MEMORY_PREFERENCE](#MEMORY-PREFERENCE) | Performances mémoire préférables. |
| [NORMAL](#NORMAL) | Mode par défaut pour le modèle de cellules. |
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
### FILE_CACHE {#FILE-CACHE}
```
public static final int FILE_CACHE
```


Des performances mémoire préférables et l'utilisation d'un fichier au lieu de la mémoire pour maintenir les données des cellules.

**Remarks**

Avec ce mode, les données des cellules seront maintenues dans un format compact et la majeure partie des données sera conservée dans un fichier temporaire au lieu de la mémoire. Ainsi, en comparant avec le mode [MEMORY\_PREFERENCE](../../com.aspose.cells/memorysetting\#MEMORY-PREFERENCE), ce mode peut réduire davantage le coût mémoire, mais les opérations d'E/S pour accéder aux données des cellules entraîneront également un coût temporel plus élevé.

Cette option est disponible depuis la version v25.7.0.

| Quelques limites notables et opérations recommandées lors de l'utilisation de ce mode : |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Lorsque ce mode est utilisé pour une feuille de calcul dans un classeur, [Workbook.dispose()](../../com.aspose.cells/workbook\#dispose--) doit être appelé à la fin du travail pour libérer toutes les ressources telles que les fichiers temporaires. |
| L'accès aléatoire aux cellules entraîne de mauvaises performances car les données doivent être lues de manière aléatoire et répétée (le pointeur dans le fichier sera donc modifié en conséquence et des opérations d'E/S seront requises à plusieurs reprises). Si possible, veuillez toujours accéder aux données de façon séquentielle (ligne par ligne). |
| Lorsque les données d'une ligne ou d'une cellule sont modifiées, les données des autres cellules ou lignes peuvent également être affectées (par exemple, les données peuvent être décalées ou déplacées vers d'autres emplacements afin d'allouer suffisamment d'espace pour les données modifiées). Ainsi, chaque modification de chaque donnée nécessite la synchronisation des autres objets existants (tels que l'objet Row ou Cell). Donc, pour obtenir de meilleures performances, veuillez ne pas maintenir plusieurs lignes ou cellules simultanément. Les traiter une par une réduira la synchronisation des données et améliorera les performances. |

### MEMORY_PREFERENCE {#MEMORY-PREFERENCE}
```
public static final int MEMORY_PREFERENCE
```


Performances mémoire préférables.

**Remarks**

Avec ce mode, les données des cellules seront maintenues dans un format compact afin de réduire le coût mémoire. En revanche, les données compactes peuvent également entraîner un coût temporel plus élevé, notamment lors de la mise à jour des données des cellules ou de leur accès aléatoire.

Cette option est disponible depuis la version v8.0.0.

### NORMAL {#NORMAL}
```
public static final int NORMAL
```


Mode par défaut pour le modèle de cellules.

**Remarks**

Ce mode s'applique à toutes les versions.

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

