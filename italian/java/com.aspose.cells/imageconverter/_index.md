---
title: "ImageConverter"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Convertitore per trasformare il file modello in immagini."
type: docs
url: /it/java/com.aspose.cells/imageconverter/
---

**Inheritance:**
java.lang.Object
```
public class ImageConverter
```

Convertitore per trasformare il file modello in immagini.

**Example**

```
         ImageConverter.process("template.xlsx", "res.png");
```
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions)](#process-com.aspose.cells.LowCodeLoadOptions-com.aspose.cells.LowCodeSaveOptions-) | Converte il file modello in immagini |
| [process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, AbstractLowCodeSaveOptionsProvider provider)](#process-com.aspose.cells.LowCodeLoadOptions-com.aspose.cells.LowCodeSaveOptions-com.aspose.cells.AbstractLowCodeSaveOptionsProvider-) | Converte il file modello in immagini |
| [process(String templateFile, String resultFile)](#process-java.lang.String-java.lang.String-) | Converte il file modello in immagini. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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




### process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions) {#process-com.aspose.cells.LowCodeLoadOptions-com.aspose.cells.LowCodeSaveOptions-}
```
public static void process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions)
```


Converte il file modello in immagini

**Remarks**

Durante la conversione in un'immagine di formato che supporta più pagine (come tiff), il [LowCodeSaveOptions.getOutputFile()](../../com.aspose.cells/lowcodesaveoptions\#getOutputFile--) o il [LowCodeSaveOptions.getOutputStream()](../../com.aspose.cells/lowcodesaveoptions\#getOutputStream--) specificati verranno utilizzati direttamente per l'immagine risultante.

Per altri tipi di immagine, se le opzioni di salvataggio hanno specificato uno Stream come output, tutte le immagini risultanti verranno salvate nello stesso Stream. Altrimenti, i file di output saranno generati dal file di output specificato nelle opzioni di salvataggio aggiungendo il numero di sequenza del foglio e la parte divisa. Ad esempio, se il file di output specificato è Image.png, i file immagine generati saranno Image\_0\_0.png, Image\_0\_1.png, ..., Image\_1\_0.png, ...

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| loadOptions | [LowCodeLoadOptions](../../com.aspose.cells/lowcodeloadoptions) | Opzioni per l'input e il caricamento |
| saveOptions | [LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions) | Opzioni per l'output e il salvataggio |

### process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, AbstractLowCodeSaveOptionsProvider provider) {#process-com.aspose.cells.LowCodeLoadOptions-com.aspose.cells.LowCodeSaveOptions-com.aspose.cells.AbstractLowCodeSaveOptionsProvider-}
```
public static void process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, AbstractLowCodeSaveOptionsProvider provider)
```


Converte il file modello in immagini

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| loadOptions | [LowCodeLoadOptions](../../com.aspose.cells/lowcodeloadoptions) | Opzioni per l'input e il caricamento |
| saveOptions | [LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions) | Opzioni per il salvataggio. Il suo output ([LowCodeSaveOptions.getOutputFile()](../../com.aspose.cells/lowcodesaveoptions\#getOutputFile--) o [LowCodeSaveOptions.getOutputStream()](../../com.aspose.cells/lowcodesaveoptions\#getOutputStream--)) non ha effetto perché tutti gli output saranno specificati dal parametro "provider". |
| provider | [AbstractLowCodeSaveOptionsProvider](../../com.aspose.cells/abstractlowcodesaveoptionsprovider) | Provider delle opzioni di salvataggio per salvare le immagini generate |

### process(String templateFile, String resultFile) {#process-java.lang.String-java.lang.String-}
```
public static void process(String templateFile, String resultFile)
```


Converte il file modello in immagini.

**Remarks**

I file di output saranno generati dal file di risultato specificato aggiungendo il numero di sequenza del foglio e la parte divisa. Ad esempio, se il file di output specificato è Image.png, i file immagine generati saranno Image\_0\_0.png, Image\_0\_1.png, ..., Image\_1\_0.png, ...

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| templateFile | java.lang.String | Il file modello da convertire in immagini. |
| resultFile | java.lang.String | Il file risultante (modello di nome) per le immagini generate. |

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

