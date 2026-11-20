---
title: "LowCodeImageSaveOptions"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Opzioni per salvare immagine in modalità low‑code."
type: docs
url: /it/java/com.aspose.cells/lowcodeimagesaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions)
```
public class LowCodeImageSaveOptions extends LowCodeSaveOptions
```

Opzioni per salvare immagine in modalità low‑code.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [LowCodeImageSaveOptions()](#LowCodeImageSaveOptions--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getImageOptions()](#getImageOptions--) | Le opzioni per il rendering delle immagini. |
| [getOutputFile()](#getOutputFile--) | Ottiene il file(con percorso se necessario) per salvare i dati generati. |
| [getOutputStream()](#getOutputStream--) | Ottiene lo Stream per scrivere i dati generati. |
| [getSaveFormat()](#getSaveFormat--) | Ottiene il formato di salvataggio. |
| [getSaveOptionsProvider()](#getSaveOptionsProvider--) | Provider delle opzioni di salvataggio per salvare le immagini generate. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setImageOptions(ImageOrPrintOptions value)](#setImageOptions-com.aspose.cells.ImageOrPrintOptions-) | Le opzioni per il rendering delle immagini. |
| [setOutputFile(String value)](#setOutputFile-java.lang.String-) | Imposta il file(con percorso se necessario) per salvare i dati generati. |
| [setOutputStream(InputStream value)](#setOutputStream-java.io.InputStream-) | Imposta lo Stream per scrivere i dati generati. |
| [setSaveFormat(int value)](#setSaveFormat-int-) | Imposta il formato di salvataggio. |
| [setSaveOptionsProvider(AbstractLowCodeSaveOptionsProvider value)](#setSaveOptionsProvider-com.aspose.cells.AbstractLowCodeSaveOptionsProvider-) | Provider delle opzioni di salvataggio per salvare le immagini generate. |
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
| Parametro | Tipo | Descrizione |
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


Le opzioni per il rendering delle immagini.

**Remarks**

Quando viene specificata un'istanza di [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions), il metodo [getSaveFormat()](../../com.aspose.cells/lowcodeimagesaveoptions\#getSaveFormat--) verrà sovrascritto (se era stato specificato in precedenza).

**Returns:**
[ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions)
### getOutputFile() {#getOutputFile--}
```
public String getOutputFile()
```


Ottiene il file(con percorso se necessario) per salvare i dati generati. Quando si imposta questa proprietà con un valore diverso da null o stringa vuota, [getOutputStream()](../../com.aspose.cells/lowcodesaveoptions\#getOutputStream--) verrà ignorato.

**Returns:**
java.lang.String
### getOutputStream() {#getOutputStream--}
```
public InputStream getOutputStream()
```


Ottiene lo Stream per scrivere i dati generati. Quando si imposta questa proprietà con un valore diverso da null, [getOutputFile()](../../com.aspose.cells/lowcodesaveoptions\#getOutputFile--) verrà ignorato.

**Returns:**
java.io.InputStream
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Ottiene il formato di salvataggio.

Vedi [SaveFormat](../../com.aspose.cells/saveformat).

**Remarks**

Se è stato specificato [getImageOptions()](../../com.aspose.cells/lowcodeimagesaveoptions\#getImageOptions--), impostare questa proprietà cambierà anche il valore di [ImageOrPrintOptions.getImageType()](../../com.aspose.cells/imageorprintoptions\#getImageType--) di essa.

**Returns:**
int
### getSaveOptionsProvider() {#getSaveOptionsProvider--}
```
public AbstractLowCodeSaveOptionsProvider getSaveOptionsProvider()
```


Provider delle opzioni di salvataggio per salvare le immagini generate.

**Remarks**

L'output ([LowCodeSaveOptions.getOutputFile()](../../com.aspose.cells/lowcodesaveoptions\#getOutputFile--) o [LowCodeSaveOptions.getOutputStream()](../../com.aspose.cells/lowcodesaveoptions\#getOutputStream--)) specificato da questa istanza non avrà effetto quando questa proprietà è impostata. Invece, l'output di ogni immagine generata sarà specificato dal provider.

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


Le opzioni per il rendering delle immagini.

**Remarks**

Quando viene specificata un'istanza di [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions), il metodo [getSaveFormat()](../../com.aspose.cells/lowcodeimagesaveoptions\#getSaveFormat--) verrà sovrascritto (se era stato specificato in precedenza).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) |  |

### setOutputFile(String value) {#setOutputFile-java.lang.String-}
```
public void setOutputFile(String value)
```


Imposta il file(con percorso se necessario) per salvare i dati generati. Quando si imposta questa proprietà con un valore diverso da null o stringa vuota, [getOutputStream()](../../com.aspose.cells/lowcodesaveoptions\#getOutputStream--) verrà ignorato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setOutputStream(InputStream value) {#setOutputStream-java.io.InputStream-}
```
public void setOutputStream(InputStream value)
```


Imposta lo Stream per scrivere i dati generati. Quando si imposta questa proprietà con un valore diverso da null, [getOutputFile()](../../com.aspose.cells/lowcodesaveoptions\#getOutputFile--) verrà ignorato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.io.InputStream |  |

### setSaveFormat(int value) {#setSaveFormat-int-}
```
public void setSaveFormat(int value)
```


Imposta il formato di salvataggio.

Vedi [SaveFormat](../../com.aspose.cells/saveformat).

**Remarks**

Se è stato specificato [getImageOptions()](../../com.aspose.cells/lowcodeimagesaveoptions\#getImageOptions--), impostare questa proprietà cambierà anche il valore di [ImageOrPrintOptions.getImageType()](../../com.aspose.cells/imageorprintoptions\#getImageType--) di essa.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setSaveOptionsProvider(AbstractLowCodeSaveOptionsProvider value) {#setSaveOptionsProvider-com.aspose.cells.AbstractLowCodeSaveOptionsProvider-}
```
public void setSaveOptionsProvider(AbstractLowCodeSaveOptionsProvider value)
```


Provider delle opzioni di salvataggio per salvare le immagini generate.

**Remarks**

L'output ([LowCodeSaveOptions.getOutputFile()](../../com.aspose.cells/lowcodesaveoptions\#getOutputFile--) o [LowCodeSaveOptions.getOutputStream()](../../com.aspose.cells/lowcodesaveoptions\#getOutputStream--)) specificato da questa istanza non avrà effetto quando questa proprietà è impostata. Invece, l'output di ogni immagine generata sarà specificato dal provider.

**Parameters:**
| Parametro | Tipo | Descrizione |
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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

