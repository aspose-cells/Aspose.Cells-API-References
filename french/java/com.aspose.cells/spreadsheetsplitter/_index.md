---
title: "SpreadsheetSplitter"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Divise le fichier de feuille de calcul en plusieurs parties."
type: docs
url: /fr/java/com.aspose.cells/spreadsheetsplitter/
---

**Inheritance:**
java.lang.Object
```
public class SpreadsheetSplitter
```

Divise le fichier de feuille de calcul en plusieurs parties.

**Example**

```
         SpreadsheetSplitter.process("template.xlsx", "split.xlsx");
```
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [process(LowCodeSplitOptions options)](#process-com.aspose.cells.LowCodeSplitOptions-) | Divise le fichier de feuille de calcul en plusieurs parties. |
| [process(String templateFile, String resultFile)](#process-java.lang.String-java.lang.String-) | Divise le fichier modèle donné en plusieurs parties. |
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




### process(LowCodeSplitOptions options) {#process-com.aspose.cells.LowCodeSplitOptions-}
```
public static void process(LowCodeSplitOptions options)
```


Divise le fichier de feuille de calcul en plusieurs parties.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| options | [LowCodeSplitOptions](../../com.aspose.cells/lowcodesplitoptions) | Options pour diviser la feuille de calcul |

### process(String templateFile, String resultFile) {#process-java.lang.String-java.lang.String-}
```
public static void process(String templateFile, String resultFile)
```


Divise le fichier modèle donné en plusieurs parties.

**Remarks**

Les fichiers de sortie seront construits à partir du fichier résultant spécifié en ajoutant le numéro de séquence de la feuille et de la partie découpée. Par exemple, si le fichier de sortie spécifié est Split.xlsx, les fichiers générés seront Split\_0\_0.xlsx, Split\_0\_1.xlsx, ..., Split\_1\_0.xlsx, ...

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| templateFile | java.lang.String | Le fichier modèle à diviser. |
| resultFile | java.lang.String | Le fichier résultant (modèle de nom) |

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

