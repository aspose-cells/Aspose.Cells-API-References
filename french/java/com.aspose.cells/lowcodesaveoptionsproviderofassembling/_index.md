---
title: "LowCodeSaveOptionsProviderOfAssembling"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Implémentation permettant de fournir des options d'enregistrement qui enregistrent les parties découpées dans des fichiers et dont le chemin du fichier résultant est nommé ainsi il peut contenir des répertoires SheetIndex ou SheetName SplitPartIndex."
type: docs
url: /fr/java/com.aspose.cells/lowcodesaveoptionsproviderofassembling/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.AbstractLowCodeSaveOptionsProvider](../../com.aspose.cells/abstractlowcodesaveoptionsprovider)
```
public class LowCodeSaveOptionsProviderOfAssembling extends AbstractLowCodeSaveOptionsProvider
```

Implémentation permettant de fournir des options d'enregistrement qui enregistrent les parties découpées dans des fichiers et dont le chemin du fichier résultant est nommé comme (il peut contenir des répertoires) : [getPathHeader()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getPathHeader--)+[getSheetPrefix()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getSheetPrefix--)+SheetIndex(ou SheetName)+[getSplitPartPrefix()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getSplitPartPrefix--)+SplitPartIndex+[getPathTail()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getPathTail--).
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [LowCodeSaveOptionsProviderOfAssembling()](#LowCodeSaveOptionsProviderOfAssembling--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [finish(LowCodeSaveOptions part)](#finish-com.aspose.cells.LowCodeSaveOptions-) | Libère les ressources après le traitement de la partie découpée actuelle. |
| [getBuildPathWithSheetAlways()](#getBuildPathWithSheetAlways--) | Indique si l'index ou le nom de la feuille est toujours ajouté au chemin du fichier. |
| [getBuildPathWithSplitPartAlways()](#getBuildPathWithSplitPartAlways--) | Indique si l'index de la partie découpée est toujours ajouté au chemin du fichier. |
| [getClass()](#getClass--) |  |
| [getPathHeader()](#getPathHeader--) | Partie d'en-tête (avant le contenu ajouté de la feuille et de la partie découpée) du chemin du fichier. |
| [getPathTail()](#getPathTail--) | Partie finale (après les numéros de séquence) du chemin du fichier. |
| [getSaveOptions(SplitPartInfo part)](#getSaveOptions-com.aspose.cells.SplitPartInfo-) | Obtient les options d'enregistrement à partir desquelles récupérer les paramètres de sortie pour la partie découpée actuelle. |
| [getSaveOptionsTemplate()](#getSaveOptionsTemplate--) | Le modèle pour créer une instance d'options d'enregistrement dans [getSaveOptions(SplitPartInfo)](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getSaveOptions-SplitPartInfo-). |
| [getSheetIndexOffset()](#getSheetIndexOffset--) | Décalage de l'index de la feuille entre celui utilisé dans le chemin du fichier et sa valeur réelle ([SplitPartInfo.getSheetIndex()](../../com.aspose.cells/splitpartinfo\#getSheetIndex--)). |
| [getSheetPrefix()](#getSheetPrefix--) | Préfixe pour l'index de la feuille de calcul. |
| [getSplitPartIndexOffset()](#getSplitPartIndexOffset--) | Décalage de l'index de la partie découpée entre ce qui est utilisé dans le chemin du fichier et sa valeur réelle([SplitPartInfo.getPartIndex()](../../com.aspose.cells/splitpartinfo\#getPartIndex--)). |
| [getSplitPartPrefix()](#getSplitPartPrefix--) | Préfixe pour l'index de la partie découpée. |
| [getUseSheetName()](#getUseSheetName--) | Indique si le chemin du fichier est construit avec le nom de la feuille au lieu de l'index de la feuille. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBuildPathWithSheetAlways(boolean value)](#setBuildPathWithSheetAlways-boolean-) | Indique si l'index ou le nom de la feuille est toujours ajouté au chemin du fichier. |
| [setBuildPathWithSplitPartAlways(boolean value)](#setBuildPathWithSplitPartAlways-boolean-) | Indique si l'index de la partie découpée est toujours ajouté au chemin du fichier. |
| [setPathHeader(String value)](#setPathHeader-java.lang.String-) | Partie d'en-tête (avant le contenu ajouté de la feuille et de la partie découpée) du chemin du fichier. |
| [setPathTail(String value)](#setPathTail-java.lang.String-) | Partie finale (après les numéros de séquence) du chemin du fichier. |
| [setSaveOptionsTemplate(LowCodeSaveOptions value)](#setSaveOptionsTemplate-com.aspose.cells.LowCodeSaveOptions-) | Le modèle pour créer une instance d'options d'enregistrement dans [getSaveOptions(SplitPartInfo)](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getSaveOptions-SplitPartInfo-). |
| [setSheetIndexOffset(int value)](#setSheetIndexOffset-int-) | Décalage de l'index de la feuille entre celui utilisé dans le chemin du fichier et sa valeur réelle ([SplitPartInfo.getSheetIndex()](../../com.aspose.cells/splitpartinfo\#getSheetIndex--)). |
| [setSheetPrefix(String value)](#setSheetPrefix-java.lang.String-) | Préfixe pour l'index de la feuille de calcul. |
| [setSplitPartIndexOffset(int value)](#setSplitPartIndexOffset-int-) | Décalage de l'index de la partie découpée entre ce qui est utilisé dans le chemin du fichier et sa valeur réelle([SplitPartInfo.getPartIndex()](../../com.aspose.cells/splitpartinfo\#getPartIndex--)). |
| [setSplitPartPrefix(String value)](#setSplitPartPrefix-java.lang.String-) | Préfixe pour l'index de la partie découpée. |
| [setUseSheetName(boolean value)](#setUseSheetName-boolean-) | Indique si le chemin du fichier est construit avec le nom de la feuille au lieu de l'index de la feuille. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### LowCodeSaveOptionsProviderOfAssembling() {#LowCodeSaveOptionsProviderOfAssembling--}
```
public LowCodeSaveOptionsProviderOfAssembling()
```


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


Indique si l'index ou le nom de la feuille est toujours ajouté au chemin du fichier. La valeur par défaut est false, c'est‑à‑dire que lorsqu'il n'y a qu'une seule feuille, l'index (ou le nom) de la feuille et le préfixe correspondant ne seront pas ajoutés au chemin du fichier.

**Returns:**
boolean
### getBuildPathWithSplitPartAlways() {#getBuildPathWithSplitPartAlways--}
```
public boolean getBuildPathWithSplitPartAlways()
```


Indique si l'index de la partie découpée est toujours ajouté au chemin du fichier. La valeur par défaut est false, c'est‑à‑dire que lorsqu'il n'y a qu'une seule partie découpée, l'index de la partie découpée et le préfixe correspondant ne seront pas ajoutés au chemin du fichier.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getPathHeader() {#getPathHeader--}
```
public String getPathHeader()
```


Partie d'en-tête (avant le contenu ajouté de la feuille et de la partie découpée) du chemin du fichier.

**Returns:**
java.lang.String
### getPathTail() {#getPathTail--}
```
public String getPathTail()
```


Partie finale (après les numéros de séquence) du chemin du fichier. Elle doit inclure l'extension du nom de fichier.

**Returns:**
java.lang.String
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


Le modèle pour créer une instance d'options d'enregistrement dans [getSaveOptions(SplitPartInfo)](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getSaveOptions-SplitPartInfo-).

**Remarks**

Si le modèle a été spécifié, l'instance créée copiera tous les paramètres à partir de celui‑ci et mettra à jour le fichier de sortie en conséquence.

**Returns:**
[LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions)
### getSheetIndexOffset() {#getSheetIndexOffset--}
```
public int getSheetIndexOffset()
```


Décalage de l'index de la feuille entre celui utilisé dans le chemin du fichier et sa valeur réelle ([SplitPartInfo.getSheetIndex()](../../com.aspose.cells/splitpartinfo\#getSheetIndex--)).

**Remarks**

Ne prend effet que lorsque [getUseSheetName()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getUseSheetName--) est false.

**Returns:**
int
### getSheetPrefix() {#getSheetPrefix--}
```
public String getSheetPrefix()
```


Préfixe pour l'index de la feuille de calcul.

**Remarks**

S'il n'y a qu'une seule feuille de calcul et que [getBuildPathWithSheetAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getBuildPathWithSheetAlways--) est false, alors ce préfixe et l'index (ou le nom) de la feuille ne seront pas ajoutés au chemin de fichier résultant.

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

S'il n'y a qu'une seule partie découpée et que [getBuildPathWithSplitPartAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getBuildPathWithSplitPartAlways--) est false, alors ce préfixe et l'index de la partie découpée (0) ne seront pas ajoutés au chemin de fichier résultant.

**Returns:**
java.lang.String
### getUseSheetName() {#getUseSheetName--}
```
public boolean getUseSheetName()
```


Indique si le chemin du fichier est construit avec le nom de la feuille au lieu de l'index de la feuille. La valeur par défaut est false.

**Remarks**

Le nom de la feuille ne sera jamais reconstruit automatiquement. Ainsi, lorsqu'il est réglé sur true, veuillez vous assurer qu'aucun nom de feuille spécial ne peut entraîner un chemin ou un nom de fichier invalide.

**Returns:**
boolean
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


Indique si l'index ou le nom de la feuille est toujours ajouté au chemin du fichier. La valeur par défaut est false, c'est‑à‑dire que lorsqu'il n'y a qu'une seule feuille, l'index (ou le nom) de la feuille et le préfixe correspondant ne seront pas ajoutés au chemin du fichier.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setBuildPathWithSplitPartAlways(boolean value) {#setBuildPathWithSplitPartAlways-boolean-}
```
public void setBuildPathWithSplitPartAlways(boolean value)
```


Indique si l'index de la partie découpée est toujours ajouté au chemin du fichier. La valeur par défaut est false, c'est‑à‑dire que lorsqu'il n'y a qu'une seule partie découpée, l'index de la partie découpée et le préfixe correspondant ne seront pas ajoutés au chemin du fichier.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setPathHeader(String value) {#setPathHeader-java.lang.String-}
```
public void setPathHeader(String value)
```


Partie d'en-tête (avant le contenu ajouté de la feuille et de la partie découpée) du chemin du fichier.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setPathTail(String value) {#setPathTail-java.lang.String-}
```
public void setPathTail(String value)
```


Partie finale (après les numéros de séquence) du chemin du fichier. Elle doit inclure l'extension du nom de fichier.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setSaveOptionsTemplate(LowCodeSaveOptions value) {#setSaveOptionsTemplate-com.aspose.cells.LowCodeSaveOptions-}
```
public void setSaveOptionsTemplate(LowCodeSaveOptions value)
```


Le modèle pour créer une instance d'options d'enregistrement dans [getSaveOptions(SplitPartInfo)](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getSaveOptions-SplitPartInfo-).

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

**Remarks**

Ne prend effet que lorsque [getUseSheetName()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getUseSheetName--) est false.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setSheetPrefix(String value) {#setSheetPrefix-java.lang.String-}
```
public void setSheetPrefix(String value)
```


Préfixe pour l'index de la feuille de calcul.

**Remarks**

S'il n'y a qu'une seule feuille de calcul et que [getBuildPathWithSheetAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getBuildPathWithSheetAlways--) est false, alors ce préfixe et l'index (ou le nom) de la feuille ne seront pas ajoutés au chemin de fichier résultant.

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

S'il n'y a qu'une seule partie découpée et que [getBuildPathWithSplitPartAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getBuildPathWithSplitPartAlways--) est false, alors ce préfixe et l'index de la partie découpée (0) ne seront pas ajoutés au chemin de fichier résultant.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setUseSheetName(boolean value) {#setUseSheetName-boolean-}
```
public void setUseSheetName(boolean value)
```


Indique si le chemin du fichier est construit avec le nom de la feuille au lieu de l'index de la feuille. La valeur par défaut est false.

**Remarks**

Le nom de la feuille ne sera jamais reconstruit automatiquement. Ainsi, lorsqu'il est réglé sur true, veuillez vous assurer qu'aucun nom de feuille spécial ne peut entraîner un chemin ou un nom de fichier invalide.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

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

