---
title: "LowCodeHtmlSaveOptions"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Opzioni per salvare html in modalità low‑code."
type: docs
url: /it/java/com.aspose.cells/lowcodehtmlsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions)
```
public class LowCodeHtmlSaveOptions extends LowCodeSaveOptions
```

Opzioni per salvare html in modalità low‑code.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [LowCodeHtmlSaveOptions()](#LowCodeHtmlSaveOptions--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getHtmlOptions()](#getHtmlOptions--) | Le opzioni generali per il salvataggio di HTML. |
| [getOutputFile()](#getOutputFile--) | Ottiene il file(con percorso se necessario) per salvare i dati generati. |
| [getOutputStream()](#getOutputStream--) | Ottiene lo Stream per scrivere i dati generati. |
| [getSaveFormat()](#getSaveFormat--) | Ottiene il formato del foglio di calcolo. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setHtmlOptions(HtmlSaveOptions value)](#setHtmlOptions-com.aspose.cells.HtmlSaveOptions-) | Le opzioni generali per il salvataggio di HTML. |
| [setOutputFile(String value)](#setOutputFile-java.lang.String-) | Imposta il file(con percorso se necessario) per salvare i dati generati. |
| [setOutputStream(InputStream value)](#setOutputStream-java.io.InputStream-) | Imposta lo Stream per scrivere i dati generati. |
| [setSaveFormat(int value)](#setSaveFormat-int-) | Imposta il formato del foglio di calcolo. |
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
### getHtmlOptions() {#getHtmlOptions--}
```
public HtmlSaveOptions getHtmlOptions()
```


Le opzioni generali per il salvataggio di HTML.

**Remarks**

Quando viene specificata un'istanza di [HtmlSaveOptions](../../com.aspose.cells/htmlsaveoptions), il metodo [getSaveFormat()](../../com.aspose.cells/lowcodehtmlsaveoptions\#getSaveFormat--) verrà sovrascritto (se era stato specificato in precedenza).

**Returns:**
[HtmlSaveOptions](../../com.aspose.cells/htmlsaveoptions)
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


Ottiene il formato del foglio di calcolo.

Vedi [SaveFormat](../../com.aspose.cells/saveformat).

**Remarks**

Quando si modifica questa proprietà, il formato di salvataggio specificato da [getHtmlOptions()](../../com.aspose.cells/lowcodehtmlsaveoptions\#getHtmlOptions--) verrà ignorato (se era stato specificato in precedenza).

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


Le opzioni generali per il salvataggio di HTML.

**Remarks**

Quando viene specificata un'istanza di [HtmlSaveOptions](../../com.aspose.cells/htmlsaveoptions), il metodo [getSaveFormat()](../../com.aspose.cells/lowcodehtmlsaveoptions\#getSaveFormat--) verrà sovrascritto (se era stato specificato in precedenza).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [HtmlSaveOptions](../../com.aspose.cells/htmlsaveoptions) |  |

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


Imposta il formato del foglio di calcolo.

Vedi [SaveFormat](../../com.aspose.cells/saveformat).

**Remarks**

Quando si modifica questa proprietà, il formato di salvataggio specificato da [getHtmlOptions()](../../com.aspose.cells/lowcodehtmlsaveoptions\#getHtmlOptions--) verrà ignorato (se era stato specificato in precedenza).

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

