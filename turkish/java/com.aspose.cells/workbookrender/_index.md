---
title: "WorkbookRender"
second_title: "Aspose.Cells for Java API Referansı"
description: "Bir Çalışma Kitabı render'ını temsil eder."
type: docs
url: /tr/java/com.aspose.cells/workbookrender/
---

**Inheritance:**
java.lang.Object
```
public class WorkbookRender
```

Bir Workbook render'ını temsil eder. Bu sınıfın yapıcı yöntemi, pagesetup ve hücre stili değiştirildikten sonra kullanılmalıdır.

**Remarks**
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [WorkbookRender(Workbook workbook, ImageOrPrintOptions options)](#WorkbookRender-com.aspose.cells.Workbook-com.aspose.cells.ImageOrPrintOptions-) | WorkbookRender yapısı |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [dispose()](#dispose--) | Render için oluşturulan ve kullanılan kaynakları serbest bırakır. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getPageCount()](#getPageCount--) | Workbook'un toplam sayfa sayısını alır. |
| [getPageSizeInch(int pageIndex)](#getPageSizeInch-int-) | Çıktı görüntüsünün inç cinsinden sayfa boyutunu al. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toImage(int pageIndex, InputStream stream)](#toImage-int-java.io.InputStream-) | Belirli bir sayfayı akışa render eder. |
| [toImage(int pageIndex, OutputStream stream)](#toImage-int-java.io.OutputStream-) | Belirli bir sayfayı akışa render eder. |
| [toImage(int pageIndex, String fileName)](#toImage-int-java.lang.String-) | Belirli bir sayfayı dosyaya render eder. |
| [toImage(OutputStream stream)](#toImage-java.io.OutputStream-) | Tüm workbook'u Tiff görüntüsü olarak akışa render eder. |
| [toImage(String filename)](#toImage-java.lang.String-) | Tüm workbook'u Tiff görüntüsü olarak bir dosyaya render eder. |
| [toPrinter(String printerName)](#toPrinter-java.lang.String-) | Workbook'u yazıcıya render eder |
| [toPrinter(String printerName, int printPageIndex, int printPageCount)](#toPrinter-java.lang.String-int-int-) | Workbook'u yazıcıya render eder |
| [toPrinter(String printerName, String jobName)](#toPrinter-java.lang.String-java.lang.String-) | Workbook'u yazıcıya render eder |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### WorkbookRender(Workbook workbook, ImageOrPrintOptions options) {#WorkbookRender-com.aspose.cells.Workbook-com.aspose.cells.ImageOrPrintOptions-}
```
public WorkbookRender(Workbook workbook, ImageOrPrintOptions options)
```


WorkbookRender yapısı

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| workbook | [Workbook](../../com.aspose.cells/workbook) | Hangi workbook'un render edileceğini belirt. |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | ImageOrPrintOptions, çıktı görüntüsünün bazı özelliklerini içerir. |

### dispose() {#dispose--}
```
public void dispose()
```


Render için oluşturulan ve kullanılan kaynakları serbest bırakır.

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parametre | Tür | Açıklama |
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
### getPageCount() {#getPageCount--}
```
public int getPageCount()
```


Workbook'un toplam sayfa sayısını alır.

**Returns:**
int
### getPageSizeInch(int pageIndex) {#getPageSizeInch-int-}
```
public float[] getPageSizeInch(int pageIndex)
```


Çıktı görüntüsünün inç cinsinden sayfa boyutunu al.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| pageIndex | int | Sayfa indeksi sıfırdan başlar. |

**Returns:**
float[] - Görüntünün sayfa boyutu, [0] genişlik ve [1] yükseklik için
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




### toImage(int pageIndex, InputStream stream) {#toImage-int-java.io.InputStream-}
```
public void toImage(int pageIndex, InputStream stream)
```


Belirli bir sayfayı akışa render eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| pageIndex | int | Hangi sayfanın dönüştürüleceğini belirt. |
| stream | java.io.InputStream | çıktı görüntüsünün akışı. |

### toImage(int pageIndex, OutputStream stream) {#toImage-int-java.io.OutputStream-}
```
public void toImage(int pageIndex, OutputStream stream)
```


Belirli bir sayfayı akışa render eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| pageIndex | int | Hangi sayfanın dönüştürüleceğini belirt. |
| stream | java.io.OutputStream | çıktı görüntüsünün akışı. |

### toImage(int pageIndex, String fileName) {#toImage-int-java.lang.String-}
```
public void toImage(int pageIndex, String fileName)
```


Belirli bir sayfayı dosyaya render eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| pageIndex | int | Hangi sayfanın dönüştürüleceğini belirt. |
| fileName | java.lang.String | çıktı görüntüsünün dosya adı. |

### toImage(OutputStream stream) {#toImage-java.io.OutputStream-}
```
public void toImage(OutputStream stream)
```


Tüm workbook'u Tiff görüntüsü olarak akışa render eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stream | java.io.OutputStream | çıktı görüntüsünün akışı. |

### toImage(String filename) {#toImage-java.lang.String-}
```
public void toImage(String filename)
```


Tüm workbook'u Tiff görüntüsü olarak bir dosyaya render eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dosya adı | java.lang.String | çıktı görüntüsünün dosya adı. |

### toPrinter(String printerName) {#toPrinter-java.lang.String-}
```
public void toPrinter(String printerName)
```


Workbook'u yazıcıya render eder

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| printerName | java.lang.String | yazıcının adı, örneğin: "Microsoft Office Document Image Writer" |

### toPrinter(String printerName, int printPageIndex, int printPageCount) {#toPrinter-java.lang.String-int-int-}
```
public void toPrinter(String printerName, int printPageIndex, int printPageCount)
```


Workbook'u yazıcıya render eder

**Remarks**

NOT: Bu yöntem artık kullanılmıyor. Bunun yerine, lütfen ilk sayfayı ve yazdırılacak sayfa sayısını ayarlamak için ToPrinter(string PrinterName) ve ImageOrPrintOptions.PageIndex, PageCount kullanın. Bu özellik Aralık 2021'den itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| printerName | java.lang.String | yazıcının adı, örneğin: "Microsoft Office Document Image Writer" |
| printPageIndex | int | yazdırılacak ilk sayfanın 0 tabanlı indeksi, aralık [0, WorkbookRender.PageCount-1] içinde olmalıdır |
| printPageCount | int | yazdırılacak sayfa sayısı, sıfırdan büyük olmalıdır |

### toPrinter(String printerName, String jobName) {#toPrinter-java.lang.String-java.lang.String-}
```
public void toPrinter(String printerName, String jobName)
```


Workbook'u yazıcıya render eder

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| printerName | java.lang.String | yazıcının adı, örneğin: "Microsoft Office Document Image Writer" |
| jobName | java.lang.String | yazdırma işi adını ayarla |

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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

