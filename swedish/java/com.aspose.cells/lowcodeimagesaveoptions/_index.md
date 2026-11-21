---
title: "LowCodeImageSaveOptions"
second_title: "Aspose.Cells för Java API-referens"
description: "Alternativ för att spara bild på ett low‑code‑sätt."
type: docs
url: /sv/java/com.aspose.cells/lowcodeimagesaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions)
```
public class LowCodeImageSaveOptions extends LowCodeSaveOptions
```

Alternativ för att spara bild på ett low‑code‑sätt.
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [LowCodeImageSaveOptions()](#LowCodeImageSaveOptions--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getImageOptions()](#getImageOptions--) | Alternativen för rendering av bilder. |
| [getOutputFile()](#getOutputFile--) | Hämtar filen (med sökväg om behövs) för att spara den genererade datan. |
| [getOutputStream()](#getOutputStream--) | Hämtar strömmen för att skriva den genererade datan till. |
| [getSaveFormat()](#getSaveFormat--) | Hämtar sparformatet. |
| [getSaveOptionsProvider()](#getSaveOptionsProvider--) | Leverantör av sparalternativ för att spara genererade bilder. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setImageOptions(ImageOrPrintOptions value)](#setImageOptions-com.aspose.cells.ImageOrPrintOptions-) | Alternativen för rendering av bilder. |
| [setOutputFile(String value)](#setOutputFile-java.lang.String-) | Ställer in filen (med sökväg om behövs) för att spara den genererade datan. |
| [setOutputStream(InputStream value)](#setOutputStream-java.io.InputStream-) | Ställer in strömmen för att skriva den genererade datan till. |
| [setSaveFormat(int value)](#setSaveFormat-int-) | Ställer in sparformatet. |
| [setSaveOptionsProvider(AbstractLowCodeSaveOptionsProvider value)](#setSaveOptionsProvider-com.aspose.cells.AbstractLowCodeSaveOptionsProvider-) | Leverantör av sparalternativ för att spara genererade bilder. |
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
### getImageOptions() {#getImageOptions--}
```
public ImageOrPrintOptions getImageOptions()
```


Alternativen för rendering av bilder.

**Remarks**

När en [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions)‑instans anges, kommer [getSaveFormat()](../../com.aspose.cells/lowcodeimagesaveoptions\#getSaveFormat--) att skrivas över (om den tidigare har angetts).

**Returns:**
[ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions)
### getOutputFile() {#getOutputFile--}
```
public String getOutputFile()
```


Hämtar filen (med sökväg om behövs) för att spara den genererade datan. När denna egenskap sätts till ett värde som inte är null eller en tom sträng, kommer [getOutputStream()](../../com.aspose.cells/lowcodesaveoptions\#getOutputStream--) att ignoreras.

**Returns:**
java.lang.String
### getOutputStream() {#getOutputStream--}
```
public InputStream getOutputStream()
```


Hämtar strömmen för att skriva den genererade datan till. När egenskapen sätts till ett värde annat än null, kommer [getOutputFile()](../../com.aspose.cells/lowcodesaveoptions\#getOutputFile--) att ignoreras.

**Returns:**
java.io.InputStream
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Hämtar sparformatet.

Se [SaveFormat](../../com.aspose.cells/saveformat).

**Remarks**

Om [getImageOptions()](../../com.aspose.cells/lowcodeimagesaveoptions\#getImageOptions--) har angetts, kommer inställning av denna egenskap också att ändra värdet för [ImageOrPrintOptions.getImageType()](../../com.aspose.cells/imageorprintoptions\#getImageType--) i den.

**Returns:**
int
### getSaveOptionsProvider() {#getSaveOptionsProvider--}
```
public AbstractLowCodeSaveOptionsProvider getSaveOptionsProvider()
```


Leverantör av sparalternativ för att spara genererade bilder.

**Remarks**

Den utdata ([LowCodeSaveOptions.getOutputFile()](../../com.aspose.cells/lowcodesaveoptions\#getOutputFile--) eller [LowCodeSaveOptions.getOutputStream()](../../com.aspose.cells/lowcodesaveoptions\#getOutputStream--)) som anges av detta objekt kommer inte att ha någon effekt när denna egenskap anges. Istället kommer utdata för varje genererad bild att specificeras av leverantören.

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


Alternativen för rendering av bilder.

**Remarks**

När en [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions)‑instans anges, kommer [getSaveFormat()](../../com.aspose.cells/lowcodeimagesaveoptions\#getSaveFormat--) att skrivas över (om den tidigare har angetts).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) |  |

### setOutputFile(String value) {#setOutputFile-java.lang.String-}
```
public void setOutputFile(String value)
```


Anger filen (med sökväg om behövs) för att spara den genererade datan. När egenskapen sätts till ett värde annat än null eller en tom sträng, kommer [getOutputStream()](../../com.aspose.cells/lowcodesaveoptions\#getOutputStream--) att ignoreras.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setOutputStream(InputStream value) {#setOutputStream-java.io.InputStream-}
```
public void setOutputStream(InputStream value)
```


Anger strömmen för att skriva den genererade datan till. När egenskapen sätts till ett värde annat än null, kommer [getOutputFile()](../../com.aspose.cells/lowcodesaveoptions\#getOutputFile--) att ignoreras.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.io.InputStream |  |

### setSaveFormat(int value) {#setSaveFormat-int-}
```
public void setSaveFormat(int value)
```


Ställer in sparformatet.

Se [SaveFormat](../../com.aspose.cells/saveformat).

**Remarks**

Om [getImageOptions()](../../com.aspose.cells/lowcodeimagesaveoptions\#getImageOptions--) har angetts, kommer inställning av denna egenskap också att ändra värdet för [ImageOrPrintOptions.getImageType()](../../com.aspose.cells/imageorprintoptions\#getImageType--) i den.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setSaveOptionsProvider(AbstractLowCodeSaveOptionsProvider value) {#setSaveOptionsProvider-com.aspose.cells.AbstractLowCodeSaveOptionsProvider-}
```
public void setSaveOptionsProvider(AbstractLowCodeSaveOptionsProvider value)
```


Leverantör av sparalternativ för att spara genererade bilder.

**Remarks**

Den utdata ([LowCodeSaveOptions.getOutputFile()](../../com.aspose.cells/lowcodesaveoptions\#getOutputFile--) eller [LowCodeSaveOptions.getOutputStream()](../../com.aspose.cells/lowcodesaveoptions\#getOutputStream--)) som anges av detta objekt kommer inte att ha någon effekt när denna egenskap anges. Istället kommer utdata för varje genererad bild att specificeras av leverantören.

**Parameters:**
| Parameter | Typ | Beskrivning |
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

