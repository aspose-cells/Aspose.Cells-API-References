---
title: "LowCodePdfSaveOptions"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Options pour enregistrer le PDF de manière low‑code."
type: docs
url: /fr/java/com.aspose.cells/lowcodepdfsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions)
```
public class LowCodePdfSaveOptions extends LowCodeSaveOptions
```

Options pour enregistrer le PDF de manière low‑code.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [LowCodePdfSaveOptions()](#LowCodePdfSaveOptions--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getOutputFile()](#getOutputFile--) | Obtient le fichier (avec le chemin si nécessaire) pour enregistrer les données générées. |
| [getOutputStream()](#getOutputStream--) | Obtient le Stream pour écrire les données générées. |
| [getPdfOptions()](#getPdfOptions--) | Les options pour enregistrer le fichier PDF. |
| [getSaveFormat()](#getSaveFormat--) | Le format d'enregistrement pour la sortie. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setOutputFile(String value)](#setOutputFile-java.lang.String-) | Définit le fichier (avec le chemin si nécessaire) pour enregistrer les données générées. |
| [setOutputStream(InputStream value)](#setOutputStream-java.io.InputStream-) | Définit le Stream pour écrire les données générées. |
| [setPdfOptions(PdfSaveOptions value)](#setPdfOptions-com.aspose.cells.PdfSaveOptions-) | Les options pour enregistrer le fichier PDF. |
| [setSaveFormat(int value)](#setSaveFormat-int-) | Le format d'enregistrement pour la sortie. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### LowCodePdfSaveOptions() {#LowCodePdfSaveOptions--}
```
public LowCodePdfSaveOptions()
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
### getPdfOptions() {#getPdfOptions--}
```
public PdfSaveOptions getPdfOptions()
```


Les options pour enregistrer le fichier PDF.

**Returns:**
[PdfSaveOptions](../../com.aspose.cells/pdfsaveoptions)
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Le format d'enregistrement pour la sortie. Pour convertir en PDF, il ne peut être que [SaveFormat.PDF](../../com.aspose.cells/saveformat\#PDF).

Voir [SaveFormat](../../com.aspose.cells/saveformat).

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

### setPdfOptions(PdfSaveOptions value) {#setPdfOptions-com.aspose.cells.PdfSaveOptions-}
```
public void setPdfOptions(PdfSaveOptions value)
```


Les options pour enregistrer le fichier PDF.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [PdfSaveOptions](../../com.aspose.cells/pdfsaveoptions) |  |

### setSaveFormat(int value) {#setSaveFormat-int-}
```
public void setSaveFormat(int value)
```


Le format d'enregistrement pour la sortie. Pour convertir en PDF, il ne peut être que [SaveFormat.PDF](../../com.aspose.cells/saveformat\#PDF).

Voir [SaveFormat](../../com.aspose.cells/saveformat).

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

