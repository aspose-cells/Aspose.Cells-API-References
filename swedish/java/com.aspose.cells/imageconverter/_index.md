---
title: "ImageConverter"
second_title: "Aspose.Cells för Java API-referens"
description: "Konverterare för att konvertera mallfil till bilder."
type: docs
url: /sv/java/com.aspose.cells/imageconverter/
---

**Inheritance:**
java.lang.Object
```
public class ImageConverter
```

Konverterare för att konvertera mallfil till bilder.

**Example**

```
         ImageConverter.process("template.xlsx", "res.png");
```
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions)](#process-com.aspose.cells.LowCodeLoadOptions-com.aspose.cells.LowCodeSaveOptions-) | Konverterar mallfil till bilder |
| [process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, AbstractLowCodeSaveOptionsProvider provider)](#process-com.aspose.cells.LowCodeLoadOptions-com.aspose.cells.LowCodeSaveOptions-com.aspose.cells.AbstractLowCodeSaveOptionsProvider-) | Konverterar mallfil till bilder |
| [process(String templateFile, String resultFile)](#process-java.lang.String-java.lang.String-) | Konverterar mallfil till bilder. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
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


Konverterar mallfil till bilder

**Remarks**

När du konverterar till en bild av format som stöder flera sidor (t.ex. tiff), den angivna [LowCodeSaveOptions.getOutputFile()](../../com.aspose.cells/lowcodesaveoptions\#getOutputFile--) eller [LowCodeSaveOptions.getOutputStream()](../../com.aspose.cells/lowcodesaveoptions\#getOutputStream--) kommer att användas direkt för den resulterande bilden.

För andra bildtyper, om sparalternativen har specificerat Stream som utdata, kommer alla resulterande bilder att sparas till samma Stream. Annars kommer utdatafilerna att byggas från den specificerade utdatafilen i sparalternativen genom att lägga till sekvensnummer för bladet och delningsdelen. Till exempel, om den specificerade utdatafilen är Image.png, kommer de genererade bildfilerna att vara Image\_0\_0.png, Image\_0\_1.png, ..., Image\_1\_0.png, ...

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| loadOptions | [LowCodeLoadOptions](../../com.aspose.cells/lowcodeloadoptions) | Alternativ för inmatning och inläsning |
| saveOptions | [LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions) | Alternativ för utmatning och sparande |

### process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, AbstractLowCodeSaveOptionsProvider provider) {#process-com.aspose.cells.LowCodeLoadOptions-com.aspose.cells.LowCodeSaveOptions-com.aspose.cells.AbstractLowCodeSaveOptionsProvider-}
```
public static void process(LowCodeLoadOptions loadOptions, LowCodeSaveOptions saveOptions, AbstractLowCodeSaveOptionsProvider provider)
```


Konverterar mallfil till bilder

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| loadOptions | [LowCodeLoadOptions](../../com.aspose.cells/lowcodeloadoptions) | Alternativ för inmatning och inläsning |
| saveOptions | [LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions) | Alternativ för sparande. Dess utdata([LowCodeSaveOptions.getOutputFile()](../../com.aspose.cells/lowcodesaveoptions\#getOutputFile--) eller [LowCodeSaveOptions.getOutputStream()](../../com.aspose.cells/lowcodesaveoptions\#getOutputStream--)) har ingen effekt eftersom alla utdata kommer att specificeras av parametern \"provider\" |
| provider | [AbstractLowCodeSaveOptionsProvider](../../com.aspose.cells/abstractlowcodesaveoptionsprovider) | Leverantör av sparalternativ för att spara de genererade bilderna |

### process(String templateFile, String resultFile) {#process-java.lang.String-java.lang.String-}
```
public static void process(String templateFile, String resultFile)
```


Konverterar mallfil till bilder.

**Remarks**

Utdatafilerna kommer att byggas från den specificerade resultatfilen genom att lägga till sekvensnummer för bladet och delningsdelen. Till exempel, om den specificerade utdatafilen är Image.png, kommer de genererade bildfilerna att vara Image\_0\_0.png, Image\_0\_1.png, ..., Image\_1\_0.png, ...

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| templateFile | java.lang.String | Mallfilen som ska konverteras till bilder. |
| resultFile | java.lang.String | Den resulterande filen (namnmönster) för genererade bilder. |

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

