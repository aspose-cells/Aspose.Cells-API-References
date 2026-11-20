---
title: "LowCodePdfSaveOptions"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Opzioni per salvare pdf in modalità low‑code."
type: docs
url: /it/java/com.aspose.cells/lowcodepdfsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions)
```
public class LowCodePdfSaveOptions extends LowCodeSaveOptions
```

Opzioni per salvare pdf in modalità low‑code.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [LowCodePdfSaveOptions()](#LowCodePdfSaveOptions--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getOutputFile()](#getOutputFile--) | Ottiene il file(con percorso se necessario) per salvare i dati generati. |
| [getOutputStream()](#getOutputStream--) | Ottiene lo Stream per scrivere i dati generati. |
| [getPdfOptions()](#getPdfOptions--) | Le opzioni per salvare il file Pdf. |
| [getSaveFormat()](#getSaveFormat--) | Il formato di salvataggio per l'output. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setOutputFile(String value)](#setOutputFile-java.lang.String-) | Imposta il file(con percorso se necessario) per salvare i dati generati. |
| [setOutputStream(InputStream value)](#setOutputStream-java.io.InputStream-) | Imposta lo Stream per scrivere i dati generati. |
| [setPdfOptions(PdfSaveOptions value)](#setPdfOptions-com.aspose.cells.PdfSaveOptions-) | Le opzioni per salvare il file Pdf. |
| [setSaveFormat(int value)](#setSaveFormat-int-) | Il formato di salvataggio per l'output. |
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
### getPdfOptions() {#getPdfOptions--}
```
public PdfSaveOptions getPdfOptions()
```


Le opzioni per salvare il file Pdf.

**Returns:**
[PdfSaveOptions](../../com.aspose.cells/pdfsaveoptions)
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Il formato di salvataggio per l'output. Per la conversione in pdf, può essere solo [SaveFormat.PDF](../../com.aspose.cells/saveformat\#PDF).

Vedi [SaveFormat](../../com.aspose.cells/saveformat).

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

### setPdfOptions(PdfSaveOptions value) {#setPdfOptions-com.aspose.cells.PdfSaveOptions-}
```
public void setPdfOptions(PdfSaveOptions value)
```


Le opzioni per salvare il file Pdf.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [PdfSaveOptions](../../com.aspose.cells/pdfsaveoptions) |  |

### setSaveFormat(int value) {#setSaveFormat-int-}
```
public void setSaveFormat(int value)
```


Il formato di salvataggio per l'output. Per la conversione in pdf, può essere solo [SaveFormat.PDF](../../com.aspose.cells/saveformat\#PDF).

Vedi [SaveFormat](../../com.aspose.cells/saveformat).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

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

