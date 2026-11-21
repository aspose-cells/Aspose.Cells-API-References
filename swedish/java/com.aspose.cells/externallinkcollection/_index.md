---
title: "ExternalLinkCollection"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar samling av externa länkar i en arbetsbok."
type: docs
url: /sv/java/com.aspose.cells/externallinkcollection/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class ExternalLinkCollection implements Iterable
```

Representerar samling av externa länkar i en arbetsbok.

**Example**

```
         //Open a file with external links
         Workbook workbook = new Workbook("book1.xls");
 
         //Change external link data source
         workbook.getWorksheets().getExternalLinks().get(0).setDataSource("d:\\link.xls");
```
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [add(int directoryType, String fileName, String[] sheetNames)](#add-int-java.lang.String-java.lang.String---) | Lägg till en extern länk. |
| [add(String fileName, String[] sheetNames)](#add-java.lang.String-java.lang.String---) | Lägger till en extern länk. |
| [clear()](#clear--) | Tar bort alla externa länkar. |
| [clear(boolean updateReferencesAsLocal)](#clear-boolean-) | Tar bort alla externa länkar. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Hämtar [ExternalLink](../../com.aspose.cells/externallink) elementet vid det angivna indexet. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Hämtar antalet element som faktiskt finns i samlingen. |
| [hashCode()](#hashCode--) |  |
| [iterator()](#iterator--) | Hämta en enumerator som itererar genom den här samlingen. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Tar bort den angivna externa länken från arbetsboken. |
| [removeAt(int index, boolean updateReferencesAsLocal)](#removeAt-int-boolean-) | Tar bort den angivna externa länken från arbetsboken. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int directoryType, String fileName, String[] sheetNames) {#add-int-java.lang.String-java.lang.String---}
```
public int add(int directoryType, String fileName, String[] sheetNames)
```


Lägg till en extern länk.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| directoryType | int | [DirectoryType](../../com.aspose.cells/directorytype). Katalogtypen för filnamnet. |
| fileName | java.lang.String | filnamnet. |
| sheetNames | java.lang.String[] | Alla bladnamn i den externa filen. |

**Returns:**
int - Positionen för det externa namnet i den här listan.
### add(String fileName, String[] sheetNames) {#add-java.lang.String-java.lang.String---}
```
public int add(String fileName, String[] sheetNames)
```


Lägger till en extern länk.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fileName | java.lang.String | Det externa filnamnet. |
| sheetNames | java.lang.String[] | Alla bladnamn i den externa filen. |

**Returns:**
int - Positionen för det externa namnet i den här listan.
### clear() {#clear--}
```
public void clear()
```


Tar bort alla externa länkar.

**Remarks**

När externa länkar tas bort kommer alla formler som refererar till dem också att tas bort eftersom referenserna blir ogiltiga.

### clear(boolean updateReferencesAsLocal) {#clear-boolean-}
```
public void clear(boolean updateReferencesAsLocal)
```


Tar bort alla externa länkar.

**Remarks**

Om referenser ska uppdateras kommer referenserna till externa länkar i formler att ändras till den aktuella arbetsboken när det är möjligt. Till exempel, en cells ursprungliga formel är "='externalsource.xlam'!customfunction()", efter att externa länkar tagits bort blir formeln "=customfunction()"; När den ursprungliga formeln är "='[externalsource.xlam]Sheet1'!$A$1", beroende på om det finns ett blad med namnet "Sheet1" i den aktuella arbetsboken: om sant blir formeln "=Sheet1!$A$1"; om falskt blir formeln "=\#REF!$A$1".

Om referenser inte behöver uppdateras kommer alla formler med referenser till externa länkar också att tas bort eftersom dessa referenser blir ogiltiga.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| updateReferencesAsLocal | boolean | Om alla referenser till externa länkar i formler ska uppdateras till referenser till den aktuella arbetsboken. |

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
### get(int index) {#get-int-}
```
public ExternalLink get(int index)
```


Hämtar [ExternalLink](../../com.aspose.cells/externallink) elementet vid det angivna indexet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Det nollbaserade indexet för elementet. |

**Returns:**
[ExternalLink](../../com.aspose.cells/externallink) - The element at the specified index.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCount() {#getCount--}
```
public int getCount()
```


Hämtar antalet element som faktiskt finns i samlingen.

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### iterator() {#iterator--}
```
public Iterator iterator()
```


Hämta en enumerator som itererar genom den här samlingen.

**Returns:**
java.util.Iterator -
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Tar bort den angivna externa länken från arbetsboken.

**Remarks**

När den externa länken tas bort kommer alla formler som refererar till den också att tas bort eftersom referenserna blir ogiltiga.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | indexet för den externa länken som ska tas bort. |

### removeAt(int index, boolean updateReferencesAsLocal) {#removeAt-int-boolean-}
```
public void removeAt(int index, boolean updateReferencesAsLocal)
```


Tar bort den angivna externa länken från arbetsboken.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | indexet för den externa länken som ska tas bort. |
| updateReferencesAsLocal | boolean | Om alla referenser för den angivna externa länken ska uppdateras till referenser till den aktuella arbetsboken. Kontrollera [clear(boolean)](../../com.aspose.cells/externallinkcollection\#clear-boolean-) för att få mer detaljer om denna parameter. |

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

