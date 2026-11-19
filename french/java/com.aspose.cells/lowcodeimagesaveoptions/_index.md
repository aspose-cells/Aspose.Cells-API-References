---
title: "LowCodeImageSaveOptions"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Options pour enregistrer l'image de manière low‑code."
type: docs
url: /fr/java/com.aspose.cells/lowcodeimagesaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions)
```
public class LowCodeImageSaveOptions extends LowCodeSaveOptions
```

Options pour enregistrer l'image de manière low‑code.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [LowCodeImageSaveOptions()](#LowCodeImageSaveOptions--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getImageOptions()](#getImageOptions--) | Les options pour le rendu des images. |
| [getOutputFile()](#getOutputFile--) | Obtient le fichier (avec le chemin si nécessaire) pour enregistrer les données générées. |
| [getOutputStream()](#getOutputStream--) | Obtient le Stream pour écrire les données générées. |
| [getSaveFormat()](#getSaveFormat--) | Obtient le format d'enregistrement. |
| [getSaveOptionsProvider()](#getSaveOptionsProvider--) | Fournisseur d'options d'enregistrement pour enregistrer les images générées. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setImageOptions(ImageOrPrintOptions value)](#setImageOptions-com.aspose.cells.ImageOrPrintOptions-) | Les options pour le rendu des images. |
| [setOutputFile(String value)](#setOutputFile-java.lang.String-) | Définit le fichier (avec le chemin si nécessaire) pour enregistrer les données générées. |
| [setOutputStream(InputStream value)](#setOutputStream-java.io.InputStream-) | Définit le Stream pour écrire les données générées. |
| [setSaveFormat(int value)](#setSaveFormat-int-) | Définit le format d'enregistrement. |
| [setSaveOptionsProvider(AbstractLowCodeSaveOptionsProvider value)](#setSaveOptionsProvider-com.aspose.cells.AbstractLowCodeSaveOptionsProvider-) | Fournisseur d'options d'enregistrement pour enregistrer les images générées. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### LowCodeImageSaveOptions() {#LowCodeImageSaveOptions--}
```
public LowCodeImageSaveOptions()
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
### getImageOptions() {#getImageOptions--}
```
public ImageOrPrintOptions getImageOptions()
```


Les options pour le rendu des images.

**Remarks**

Lorsque une instance de [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) est spécifiée, la [getSaveFormat()](../../com.aspose.cells/lowcodeimagesaveoptions\#getSaveFormat--) sera écrasée (si elle avait été spécifiée auparavant).

**Returns:**
[ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions)
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


Obtient le format d'enregistrement.

Voir [SaveFormat](../../com.aspose.cells/saveformat).

**Remarks**

Si [getImageOptions()](../../com.aspose.cells/lowcodeimagesaveoptions\#getImageOptions--) a été spécifiée, la définition de cette propriété modifiera également la valeur de [ImageOrPrintOptions.getImageType()](../../com.aspose.cells/imageorprintoptions\#getImageType--) correspondante.

**Returns:**
int
### getSaveOptionsProvider() {#getSaveOptionsProvider--}
```
public AbstractLowCodeSaveOptionsProvider getSaveOptionsProvider()
```


Fournisseur d'options d'enregistrement pour enregistrer les images générées.

**Remarks**

La sortie ([LowCodeSaveOptions.getOutputFile()](../../com.aspose.cells/lowcodesaveoptions\#getOutputFile--) ou [LowCodeSaveOptions.getOutputStream()](../../com.aspose.cells/lowcodesaveoptions\#getOutputStream--)) spécifiée par cette instance n'aura aucun effet lorsque cette propriété est définie. À la place, la sortie de chaque image générée sera spécifiée par le fournisseur.

**Returns:**
[AbstractLowCodeSaveOptionsProvider](../../com.aspose.cells/abstractlowcodesaveoptionsprovider)
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




### setImageOptions(ImageOrPrintOptions value) {#setImageOptions-com.aspose.cells.ImageOrPrintOptions-}
```
public void setImageOptions(ImageOrPrintOptions value)
```


Les options pour le rendu des images.

**Remarks**

Lorsque une instance de [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) est spécifiée, la [getSaveFormat()](../../com.aspose.cells/lowcodeimagesaveoptions\#getSaveFormat--) sera écrasée (si elle avait été spécifiée auparavant).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) |  |

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


Définit le format d'enregistrement.

Voir [SaveFormat](../../com.aspose.cells/saveformat).

**Remarks**

Si [getImageOptions()](../../com.aspose.cells/lowcodeimagesaveoptions\#getImageOptions--) a été spécifiée, la définition de cette propriété modifiera également la valeur de [ImageOrPrintOptions.getImageType()](../../com.aspose.cells/imageorprintoptions\#getImageType--) correspondante.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

### setSaveOptionsProvider(AbstractLowCodeSaveOptionsProvider value) {#setSaveOptionsProvider-com.aspose.cells.AbstractLowCodeSaveOptionsProvider-}
```
public void setSaveOptionsProvider(AbstractLowCodeSaveOptionsProvider value)
```


Fournisseur d'options d'enregistrement pour enregistrer les images générées.

**Remarks**

La sortie ([LowCodeSaveOptions.getOutputFile()](../../com.aspose.cells/lowcodesaveoptions\#getOutputFile--) ou [LowCodeSaveOptions.getOutputStream()](../../com.aspose.cells/lowcodesaveoptions\#getOutputStream--)) spécifiée par cette instance n'aura aucun effet lorsque cette propriété est définie. À la place, la sortie de chaque image générée sera spécifiée par le fournisseur.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [AbstractLowCodeSaveOptionsProvider](../../com.aspose.cells/abstractlowcodesaveoptionsprovider) |  |

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

