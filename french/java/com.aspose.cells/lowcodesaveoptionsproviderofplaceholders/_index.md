---
title: "LowCodeSaveOptionsProviderOfPlaceHolders"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Implémentation pour fournir des options d'enregistrement qui enregistrent les parties découpées dans des fichiers et dont le chemin du fichier résultant est défini avec des espaces réservés."
type: docs
url: /fr/java/com.aspose.cells/lowcodesaveoptionsproviderofplaceholders/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.AbstractLowCodeSaveOptionsProvider](../../com.aspose.cells/abstractlowcodesaveoptionsprovider)
```
public class LowCodeSaveOptionsProviderOfPlaceHolders extends AbstractLowCodeSaveOptionsProvider
```

Implémentation pour fournir des options d'enregistrement qui enregistrent les parties découpées dans des fichiers et dont le chemin du fichier résultant est défini avec des espaces réservés.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [LowCodeSaveOptionsProviderOfPlaceHolders(String pathTemplate)](#LowCodeSaveOptionsProviderOfPlaceHolders-java.lang.String-) | Instancie une instance pour fournir des options d'enregistrement selon les modèles spécifiés. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [finish(LowCodeSaveOptions part)](#finish-com.aspose.cells.LowCodeSaveOptions-) | Libère les ressources après le traitement de la partie découpée actuelle. |
| [getBuildPathWithSheetAlways()](#getBuildPathWithSheetAlways--) | Indique si l'index ou le nom de la feuille est toujours ajouté au chemin du fichier. |
| [getBuildPathWithSplitPartAlways()](#getBuildPathWithSplitPartAlways--) | Indique si l'index de la partie découpée est toujours ajouté au chemin du fichier. |
| [getClass()](#getClass--) |  |
| [getSaveOptions(SplitPartInfo part)](#getSaveOptions-com.aspose.cells.SplitPartInfo-) | Obtient les options d'enregistrement à partir desquelles récupérer les paramètres de sortie pour la partie découpée actuelle. |
| [getSaveOptionsTemplate()](#getSaveOptionsTemplate--) | Le modèle pour créer une instance d'options d'enregistrement dans [getSaveOptions(SplitPartInfo)](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getSaveOptions-SplitPartInfo-). |
| [getSheetIndexOffset()](#getSheetIndexOffset--) | Décalage de l'index de la feuille entre celui utilisé dans le chemin du fichier et sa valeur réelle ([SplitPartInfo.getSheetIndex()](../../com.aspose.cells/splitpartinfo\#getSheetIndex--)). |
| [getSheetIndexPrefix()](#getSheetIndexPrefix--) | Préfixe pour l'index de la feuille de calcul. |
| [getSheetNamePrefix()](#getSheetNamePrefix--) | Préfixe pour l'index de la feuille de calcul. |
| [getSplitPartIndexOffset()](#getSplitPartIndexOffset--) | Décalage de l'index de la partie découpée entre ce qui est utilisé dans le chemin du fichier et sa valeur réelle([SplitPartInfo.getPartIndex()](../../com.aspose.cells/splitpartinfo\#getPartIndex--)). |
| [getSplitPartPrefix()](#getSplitPartPrefix--) | Préfixe pour l'index de la partie découpée. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBuildPathWithSheetAlways(boolean value)](#setBuildPathWithSheetAlways-boolean-) | Indique si l'index ou le nom de la feuille est toujours ajouté au chemin du fichier. |
| [setBuildPathWithSplitPartAlways(boolean value)](#setBuildPathWithSplitPartAlways-boolean-) | Indique si l'index de la partie découpée est toujours ajouté au chemin du fichier. |
| [setSaveOptionsTemplate(LowCodeSaveOptions value)](#setSaveOptionsTemplate-com.aspose.cells.LowCodeSaveOptions-) | Le modèle pour créer une instance d'options d'enregistrement dans [getSaveOptions(SplitPartInfo)](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getSaveOptions-SplitPartInfo-). |
| [setSheetIndexOffset(int value)](#setSheetIndexOffset-int-) | Décalage de l'index de la feuille entre celui utilisé dans le chemin du fichier et sa valeur réelle ([SplitPartInfo.getSheetIndex()](../../com.aspose.cells/splitpartinfo\#getSheetIndex--)). |
| [setSheetIndexPrefix(String value)](#setSheetIndexPrefix-java.lang.String-) | Préfixe pour l'index de la feuille de calcul. |
| [setSheetNamePrefix(String value)](#setSheetNamePrefix-java.lang.String-) | Préfixe pour l'index de la feuille de calcul. |
| [setSplitPartIndexOffset(int value)](#setSplitPartIndexOffset-int-) | Décalage de l'index de la partie découpée entre ce qui est utilisé dans le chemin du fichier et sa valeur réelle([SplitPartInfo.getPartIndex()](../../com.aspose.cells/splitpartinfo\#getPartIndex--)). |
| [setSplitPartPrefix(String value)](#setSplitPartPrefix-java.lang.String-) | Préfixe pour l'index de la partie découpée. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### LowCodeSaveOptionsProviderOfPlaceHolders(String pathTemplate) {#LowCodeSaveOptionsProviderOfPlaceHolders-java.lang.String-}
```
public LowCodeSaveOptionsProviderOfPlaceHolders(String pathTemplate)
```


Instancie une instance pour fournir des options d'enregistrement selon les modèles spécifiés.

**Remarks**

Les espaces réservés pris en charge dans le modèle de chemin de fichier :

 *  $\{SheetIndex\}: will be replaced by the sheet index of the split part
 *  $\{SheetName\}: will be replaced by the sheet name of the split part
 *  $\{SplitPartIndex\}: will be replaced by the index of the split part
 *  $\{SheetIndexPrefix\}: will be replaced by
 *  $\{SheetNamePrefix\}: will be replaced by
 *  $\{SplitPartPrefix\}: will be replaced by

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| pathTemplate | java.lang.String | Le modèle du chemin de fichier résultant. |

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
### finish(LowCodeSaveOptions part) {#finish-com.aspose.cells.LowCodeSaveOptions-}
```
public void finish(LowCodeSaveOptions part)
```


Libère les ressources après le traitement de la partie découpée actuelle.

**Remarks**

Par défaut, cette méthode ferme simplement le flux spécifié par le [LowCodeSaveOptions.getOutputStream()](../../com.aspose.cells/lowcodesaveoptions\#getOutputStream--) directement (si les options d'enregistrement ont spécifié un flux comme destination). L'utilisateur peut remplacer cette méthode pour contrôler la façon de libérer les ressources selon ses besoins et l'implémentation de [getSaveOptions(SplitPartInfo)](../../com.aspose.cells/abstractlowcodesaveoptionsprovider\#getSaveOptions-SplitPartInfo-).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| part | [LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions) | les options d'enregistrement utilisées pour la partie découpée actuelle. |

### getBuildPathWithSheetAlways() {#getBuildPathWithSheetAlways--}
```
public boolean getBuildPathWithSheetAlways()
```


Indique s'il faut toujours ajouter l'index ou le nom de la feuille au chemin du fichier. La valeur par défaut est false, c'est‑à‑dire que lorsqu'il n'y a qu'une seule feuille, l'index et le nom de la feuille ainsi que le préfixe correspondant ([getSheetNamePrefix()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getSheetNamePrefix--)) ne seront pas ajoutés au chemin du fichier.

**Returns:**
boolean
### getBuildPathWithSplitPartAlways() {#getBuildPathWithSplitPartAlways--}
```
public boolean getBuildPathWithSplitPartAlways()
```


Indique s'il faut toujours ajouter l'index de la partie découpée au chemin du fichier. La valeur par défaut est false, c'est‑à‑dire que lorsqu'il n'y a qu'une seule partie découpée, l'index de la partie découpée et le préfixe correspondant ([getSplitPartPrefix()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getSplitPartPrefix--)) ne seront pas ajoutés au chemin du fichier.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getSaveOptions(SplitPartInfo part) {#getSaveOptions-com.aspose.cells.SplitPartInfo-}
```
public LowCodeSaveOptions getSaveOptions(SplitPartInfo part)
```


Obtient les options d'enregistrement à partir desquelles récupérer les paramètres de sortie pour la partie découpée actuelle.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| part | [SplitPartInfo](../../com.aspose.cells/splitpartinfo) |  |

**Returns:**
[LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions)
### getSaveOptionsTemplate() {#getSaveOptionsTemplate--}
```
public LowCodeSaveOptions getSaveOptionsTemplate()
```


Le modèle pour créer une instance d'options d'enregistrement dans [getSaveOptions(SplitPartInfo)](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getSaveOptions-SplitPartInfo-).

**Remarks**

Si le modèle a été spécifié, l'instance créée copiera tous les paramètres à partir de celui‑ci et mettra à jour le fichier de sortie en conséquence.

**Returns:**
[LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions)
### getSheetIndexOffset() {#getSheetIndexOffset--}
```
public int getSheetIndexOffset()
```


Décalage de l'index de la feuille entre celui utilisé dans le chemin du fichier et sa valeur réelle ([SplitPartInfo.getSheetIndex()](../../com.aspose.cells/splitpartinfo\#getSheetIndex--)).

**Returns:**
int
### getSheetIndexPrefix() {#getSheetIndexPrefix--}
```
public String getSheetIndexPrefix()
```


Préfixe pour l'index de la feuille de calcul.

**Remarks**

S'il n'y a qu'une seule feuille de calcul et que [getBuildPathWithSheetAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getBuildPathWithSheetAlways--) est false, alors ce préfixe et l'index (ou le nom) de la feuille ne seront pas ajoutés au chemin du fichier résultant.

**Returns:**
java.lang.String
### getSheetNamePrefix() {#getSheetNamePrefix--}
```
public String getSheetNamePrefix()
```


Préfixe pour l'index de la feuille de calcul.

**Remarks**

S'il n'y a qu'une seule feuille de calcul et que [getBuildPathWithSheetAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getBuildPathWithSheetAlways--) est false, alors ce préfixe et l'index (ou le nom) de la feuille ne seront pas ajoutés au chemin du fichier résultant.

**Returns:**
java.lang.String
### getSplitPartIndexOffset() {#getSplitPartIndexOffset--}
```
public int getSplitPartIndexOffset()
```


Décalage de l'index de la partie découpée entre ce qui est utilisé dans le chemin du fichier et sa valeur réelle([SplitPartInfo.getPartIndex()](../../com.aspose.cells/splitpartinfo\#getPartIndex--)).

**Returns:**
int
### getSplitPartPrefix() {#getSplitPartPrefix--}
```
public String getSplitPartPrefix()
```


Préfixe pour l'index de la partie découpée.

**Remarks**

S'il n'y a qu'une seule partie découpée et que [getBuildPathWithSplitPartAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getBuildPathWithSplitPartAlways--) est false, alors ce préfixe et l'index de la partie découpée (0) ne seront pas ajoutés au chemin du fichier résultant.

**Returns:**
java.lang.String
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




### setBuildPathWithSheetAlways(boolean value) {#setBuildPathWithSheetAlways-boolean-}
```
public void setBuildPathWithSheetAlways(boolean value)
```


Indique s'il faut toujours ajouter l'index ou le nom de la feuille au chemin du fichier. La valeur par défaut est false, c'est‑à‑dire que lorsqu'il n'y a qu'une seule feuille, l'index et le nom de la feuille ainsi que le préfixe correspondant ([getSheetNamePrefix()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getSheetNamePrefix--)) ne seront pas ajoutés au chemin du fichier.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setBuildPathWithSplitPartAlways(boolean value) {#setBuildPathWithSplitPartAlways-boolean-}
```
public void setBuildPathWithSplitPartAlways(boolean value)
```


Indique s'il faut toujours ajouter l'index de la partie découpée au chemin du fichier. La valeur par défaut est false, c'est‑à‑dire que lorsqu'il n'y a qu'une seule partie découpée, l'index de la partie découpée et le préfixe correspondant ([getSplitPartPrefix()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getSplitPartPrefix--)) ne seront pas ajoutés au chemin du fichier.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setSaveOptionsTemplate(LowCodeSaveOptions value) {#setSaveOptionsTemplate-com.aspose.cells.LowCodeSaveOptions-}
```
public void setSaveOptionsTemplate(LowCodeSaveOptions value)
```


Le modèle pour créer une instance d'options d'enregistrement dans [getSaveOptions(SplitPartInfo)](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getSaveOptions-SplitPartInfo-).

**Remarks**

Si le modèle a été spécifié, l'instance créée copiera tous les paramètres à partir de celui‑ci et mettra à jour le fichier de sortie en conséquence.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions) |  |

### setSheetIndexOffset(int value) {#setSheetIndexOffset-int-}
```
public void setSheetIndexOffset(int value)
```


Décalage de l'index de la feuille entre celui utilisé dans le chemin du fichier et sa valeur réelle ([SplitPartInfo.getSheetIndex()](../../com.aspose.cells/splitpartinfo\#getSheetIndex--)).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setSheetIndexPrefix(String value) {#setSheetIndexPrefix-java.lang.String-}
```
public void setSheetIndexPrefix(String value)
```


Préfixe pour l'index de la feuille de calcul.

**Remarks**

S'il n'y a qu'une seule feuille de calcul et que [getBuildPathWithSheetAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getBuildPathWithSheetAlways--) est false, alors ce préfixe et l'index (ou le nom) de la feuille ne seront pas ajoutés au chemin du fichier résultant.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setSheetNamePrefix(String value) {#setSheetNamePrefix-java.lang.String-}
```
public void setSheetNamePrefix(String value)
```


Préfixe pour l'index de la feuille de calcul.

**Remarks**

S'il n'y a qu'une seule feuille de calcul et que [getBuildPathWithSheetAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getBuildPathWithSheetAlways--) est false, alors ce préfixe et l'index (ou le nom) de la feuille ne seront pas ajoutés au chemin du fichier résultant.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setSplitPartIndexOffset(int value) {#setSplitPartIndexOffset-int-}
```
public void setSplitPartIndexOffset(int value)
```


Décalage de l'index de la partie découpée entre ce qui est utilisé dans le chemin du fichier et sa valeur réelle([SplitPartInfo.getPartIndex()](../../com.aspose.cells/splitpartinfo\#getPartIndex--)).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setSplitPartPrefix(String value) {#setSplitPartPrefix-java.lang.String-}
```
public void setSplitPartPrefix(String value)
```


Préfixe pour l'index de la partie découpée.

**Remarks**

S'il n'y a qu'une seule partie découpée et que [getBuildPathWithSplitPartAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getBuildPathWithSplitPartAlways--) est false, alors ce préfixe et l'index de la partie découpée (0) ne seront pas ajoutés au chemin du fichier résultant.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

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

