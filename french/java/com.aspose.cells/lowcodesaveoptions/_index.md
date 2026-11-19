---
title: "LowCodeSaveOptions"
second_title: "Référence API d'Aspose.Cells pour Java"
description: "Options pour enregistrer les résultats générés de manière low‑code."
type: docs
url: /fr/java/com.aspose.cells/lowcodesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class LowCodeSaveOptions
```

Options pour enregistrer les résultats générés de manière low‑code.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [LowCodeSaveOptions()](#LowCodeSaveOptions--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getOutputFile()](#getOutputFile--) | Obtient le fichier (avec le chemin si nécessaire) pour enregistrer les données générées. |
| [getOutputStream()](#getOutputStream--) | Obtient le Stream pour écrire les données générées. |
| [getSaveFormat()](#getSaveFormat--) | Obtient le format d'enregistrement pour la sortie. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setOutputFile(String value)](#setOutputFile-java.lang.String-) | Définit le fichier (avec le chemin si nécessaire) pour enregistrer les données générées. |
| [setOutputStream(InputStream value)](#setOutputStream-java.io.InputStream-) | Définit le Stream pour écrire les données générées. |
| [setSaveFormat(int value)](#setSaveFormat-int-) | Définit le format d'enregistrement pour la sortie. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### LowCodeSaveOptions() {#LowCodeSaveOptions--}
```
public LowCodeSaveOptions()
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
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Obtient le format d'enregistrement pour la sortie. En général, pour un processus spécifique en mode low‑code, seuls certains formats spécifiques sont autorisés. Veuillez spécifier le format correct pour le processus correspondant, sinon un résultat inattendu ou même une exception peut se produire.

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

### setSaveFormat(int value) {#setSaveFormat-int-}
```
public void setSaveFormat(int value)
```


Définit le format d'enregistrement pour la sortie. En général, pour un processus spécifique en mode low‑code, seuls certains formats spécifiques sont autorisés. Veuillez spécifier le format correct pour le processus correspondant, sinon un résultat inattendu ou même une exception peut se produire.

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

