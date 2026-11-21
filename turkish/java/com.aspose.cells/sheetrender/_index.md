---
title: "SheetRender"
second_title: "Aspose.Cells for Java API Referansı"
description: "Bir çalışma sayfası render'ını temsil eder ve çalışma sayfasını BMP, PNG, JPEG, TIFF gibi çeşitli görüntülere render edebilir."
type: docs
url: /tr/java/com.aspose.cells/sheetrender/
---

**Inheritance:**
java.lang.Object
```
public class SheetRender
```

Bir çalışma sayfası render'ını temsil eder ve çalışma sayfasını (BMP, PNG, JPEG, TIFF..) gibi çeşitli görüntülere render edebilir. Bu sınıfın yapıcı yöntemi, sayfa ayarı ve hücre stilinde değişiklik yapıldıktan sonra kullanılmalıdır.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [SheetRender(Worksheet worksheet, ImageOrPrintOptions options)](#SheetRender-com.aspose.cells.Worksheet-com.aspose.cells.ImageOrPrintOptions-) | SheetRender yapısı, çalışma sayfası ve ImageOrPrintOptions parametrelerini gerektirir. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [dispose()](#dispose--) | Render için oluşturulan ve kullanılan kaynakları serbest bırakır. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getPageCount()](#getPageCount--) | Mevcut çalışma sayfasının toplam sayfa sayısını alır. |
| [getPageScale()](#getPageScale--) | Sayfanın hesaplanan ölçeğini alır. |
| [getPageSizeInch(int pageIndex)](#getPageSizeInch-int-) | Çıktı görüntüsünün inç cinsinden sayfa boyutunu al. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toImage(int pageIndex, InputStream stream)](#toImage-int-java.io.InputStream-) | Belirli bir sayfayı akışa render eder. |
| [toImage(int pageIndex, OutputStream stream)](#toImage-int-java.io.OutputStream-) | Belirli bir sayfayı akışa render eder. |
| [toImage(int pageIndex, String fileName)](#toImage-int-java.lang.String-) | Belirli bir sayfayı dosyaya render eder. |
| [toPrinter(String printerName)](#toPrinter-java.lang.String-) | Çalışma sayfasını Yazıcıya render eder. |
| [toPrinter(String printerName, int printPageIndex, int printPageCount)](#toPrinter-java.lang.String-int-int-) | Çalışma sayfasını Yazıcıya render eder. |
| [toPrinter(String printerName, String jobName)](#toPrinter-java.lang.String-java.lang.String-) | Çalışma sayfasını Yazıcıya render eder. |
| [toString()](#toString--) |  |
| [toTiff(InputStream stream)](#toTiff-java.io.InputStream-) | Tüm çalışma sayfasını akışa Tiff Görüntüsü olarak render eder. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### SheetRender(Worksheet worksheet, ImageOrPrintOptions options) {#SheetRender-com.aspose.cells.Worksheet-com.aspose.cells.ImageOrPrintOptions-}
```
public SheetRender(Worksheet worksheet, ImageOrPrintOptions options)
```


SheetRender yapısı, çalışma sayfası ve ImageOrPrintOptions parametrelerini gerektirir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| worksheet | [Worksheet](../../com.aspose.cells/worksheet) | Hangi elektronik tabloyun render edileceğini belirt. |
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


Mevcut çalışma sayfasının toplam sayfa sayısını alır.

**Returns:**
int
### getPageScale() {#getPageScale--}
```
public double getPageScale()
```


Sayfanın hesaplanan ölçeğini alır. [PageSetup.getZoom()](../../com.aspose.cells/pagesetup\#getZoom--) ayarlıysa ayarlanan ölçeği döndürür. Aksi takdirde, [PageSetup.getFitToPagesWide()](../../com.aspose.cells/pagesetup\#getFitToPagesWide--) ve [PageSetup.getFitToPagesTall()](../../com.aspose.cells/pagesetup\#getFitToPagesTall--) değerlerine göre hesaplanan ölçeği döndürür.

**Example**

```
         Workbook wb = new Workbook("Book1.xlsx");
 
         SheetRender sheetRender = new SheetRender(wb.getWorksheets().get(0), new ImageOrPrintOptions());
 
         //Gets calculated page scale of the sheet.
         double pageScale = sheetRender.getPageScale();
```

**Returns:**
double
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

**Example**

Aşağıdaki kod, ilk sayfanın ilk sayfasını png görüntüsü olarak çıkarır.

```
         //load the source file with images.
         Workbook wb = new Workbook("Book1.xlsx");
 
         ImageOrPrintOptions imgOpt = new ImageOrPrintOptions();
 
         //set output image type.
         imgOpt.setImageType(ImageType.PNG);
 
         //render the first sheet.
         SheetRender sr = new SheetRender(wb.getWorksheets().get(0), imgOpt);
 
         //output the first page of the sheet to image.
         sr.toImage(0, "output.png");
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| pageIndex | int | Hangi sayfanın dönüştürüleceğini belirt. |
| fileName | java.lang.String | çıktı görüntüsünün dosya adı. |

### toPrinter(String printerName) {#toPrinter-java.lang.String-}
```
public void toPrinter(String printerName)
```


Çalışma sayfasını Yazıcıya render eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| printerName | java.lang.String | yazıcının adı, örneğin: "Microsoft Office Document Image Writer" |

### toPrinter(String printerName, int printPageIndex, int printPageCount) {#toPrinter-java.lang.String-int-int-}
```
public void toPrinter(String printerName, int printPageIndex, int printPageCount)
```


Çalışma sayfasını Yazıcıya render eder.

**Remarks**

NOT: Bu yöntem artık kullanılmıyor. Bunun yerine, lütfen ilk sayfayı ve yazdırılacak sayfa sayısını ayarlamak için ToPrinter(string PrinterName) ve ImageOrPrintOptions.PageIndex, PageCount kullanın. Bu özellik Aralık 2021'den itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| printerName | java.lang.String | yazıcının adı, örneğin: "Microsoft Office Document Image Writer" |
| printPageIndex | int | Yazdırılacak ilk sayfanın 0 tabanlı indeksi, [0, SheetRender.PageCount-1] aralığında olmalıdır. |
| printPageCount | int | yazdırılacak sayfa sayısı, sıfırdan büyük olmalıdır |

### toPrinter(String printerName, String jobName) {#toPrinter-java.lang.String-java.lang.String-}
```
public void toPrinter(String printerName, String jobName)
```


Çalışma sayfasını Yazıcıya render eder.

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
### toTiff(InputStream stream) {#toTiff-java.io.InputStream-}
```
public void toTiff(InputStream stream)
```


Tüm çalışma sayfasını akışa Tiff Görüntüsü olarak render eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stream | java.io.InputStream | çıktı görüntüsünün akışı. |

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

