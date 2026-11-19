---
title: "LowCodeHtmlSaveOptions"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Options pour enregistrer le HTML de manière low‑code."
type: docs
url: /fr/java/com.aspose.cells/lowcodehtmlsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions)
```
public class LowCodeHtmlSaveOptions extends LowCodeSaveOptions
```

Options pour enregistrer le HTML de manière low‑code.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [LowCodeHtmlSaveOptions()](#LowCodeHtmlSaveOptions--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getHtmlOptions()](#getHtmlOptions--) | Les options générales pour enregistrer le HTML. |
| [getOutputFile()](#getOutputFile--) | Obtient le fichier (avec le chemin si nécessaire) pour enregistrer les données générées. |
| [getOutputStream()](#getOutputStream--) | Obtient le Stream pour écrire les données générées. |
| [getSaveFormat()](#getSaveFormat--) | Obtient le format de la feuille de calcul. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setHtmlOptions(HtmlSaveOptions value)](#setHtmlOptions-com.aspose.cells.HtmlSaveOptions-) | Les options générales pour enregistrer le HTML. |
| [setOutputFile(String value)](#setOutputFile-java.lang.String-) | Définit le fichier (avec le chemin si nécessaire) pour enregistrer les données générées. |
| [setOutputStream(InputStream value)](#setOutputStream-java.io.InputStream-) | Définit le Stream pour écrire les données générées. |
| [setSaveFormat(int value)](#setSaveFormat-int-) | Définit le format de la feuille de calcul. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### LowCodeHtmlSaveOptions() {#LowCodeHtmlSaveOptions--}
```
public LowCodeHtmlSaveOptions()
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getHtmlOptions() {#getHtmlOptions--}
```
public HtmlSaveOptions getHtmlOptions()
```


Les options générales pour enregistrer le HTML.

**Remarks**

Lorsque une instance de [HtmlSaveOptions](../../com.aspose.cells/htmlsaveoptions) est spécifiée, la méthode [getSaveFormat()](../../com.aspose.cells/lowcodehtmlsaveoptions\#getSaveFormat--) sera écrasée (si elle avait été spécifiée auparavant).

**Returns:**
[HtmlSaveOptions](../../com.aspose.cells/htmlsaveoptions)
### getOutputFile() {#getOutputFile--}
```
public String getOutputFile()
```


Obtient le fichier (avec le chemin si nécessaire) pour enregistrer les données générées. Lors de la définition de cette propriété avec une valeur différente de null ou d'une chaîne vide, [getOutputStream()](../../com.aspose.cells/lowcodesaveoptions\#getOutputStream--) sera ignoré.

**Returns:**
java.lang.String
### getOutputStream() {#getOutputStream--}
```
public InputStream getOutputStream()
```


Obtient le Stream pour écrire les données générées. Lors de la définition de cette propriété avec une valeur différente de null, [getOutputFile()](../../com.aspose.cells/lowcodesaveoptions\#getOutputFile--) sera ignoré.

**Returns:**
java.io.InputStream
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Obtient le format de la feuille de calcul.

Voir [SaveFormat](../../com.aspose.cells/saveformat).

**Remarks**

Lors de la modification de cette propriété, le format d'enregistrement spécifié par [getHtmlOptions()](../../com.aspose.cells/lowcodehtmlsaveoptions\#getHtmlOptions--) sera ignoré (s'il avait été spécifié auparavant).

**Returns:**
int
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




### setHtmlOptions(HtmlSaveOptions value) {#setHtmlOptions-com.aspose.cells.HtmlSaveOptions-}
```
public void setHtmlOptions(HtmlSaveOptions value)
```


Les options générales pour enregistrer le HTML.

**Remarks**

Lorsque une instance de [HtmlSaveOptions](../../com.aspose.cells/htmlsaveoptions) est spécifiée, la méthode [getSaveFormat()](../../com.aspose.cells/lowcodehtmlsaveoptions\#getSaveFormat--) sera écrasée (si elle avait été spécifiée auparavant).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [HtmlSaveOptions](../../com.aspose.cells/htmlsaveoptions) |  |

### setOutputFile(String value) {#setOutputFile-java.lang.String-}
```
public void setOutputFile(String value)
```


Définit le fichier (avec le chemin si nécessaire) pour enregistrer les données générées. Lors de la définition de cette propriété avec une valeur différente de null ou d'une chaîne vide, [getOutputStream()](../../com.aspose.cells/lowcodesaveoptions\#getOutputStream--) sera ignoré.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String |  |

### setOutputStream(InputStream value) {#setOutputStream-java.io.InputStream-}
```
public void setOutputStream(InputStream value)
```


Définit le Stream pour écrire les données générées. Lors de la définition de cette propriété avec une valeur différente de null, [getOutputFile()](../../com.aspose.cells/lowcodesaveoptions\#getOutputFile--) sera ignoré.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.io.InputStream |  |

### setSaveFormat(int value) {#setSaveFormat-int-}
```
public void setSaveFormat(int value)
```


Définit le format de la feuille de calcul.

Voir [SaveFormat](../../com.aspose.cells/saveformat).

**Remarks**

Lors de la modification de cette propriété, le format d'enregistrement spécifié par [getHtmlOptions()](../../com.aspose.cells/lowcodehtmlsaveoptions\#getHtmlOptions--) sera ignoré (s'il avait été spécifié auparavant).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

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

