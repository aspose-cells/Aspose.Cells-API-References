---
title: "LoadFilter"
second_title: "Aspose.Cells for Java API Referansı"
description: "Şablondan çalışma kitabı yüklenirken veri yükleme seçeneklerini sağlayan filtreyi temsil eder."
type: docs
url: /tr/java/com.aspose.cells/loadfilter/
---

**Inheritance:**
java.lang.Object
```
public class LoadFilter
```

Şablondan çalışma kitabı yüklenirken veri yükleme seçeneklerini sağlayan filtreyi temsil eder.

**Remarks**

Kullanıcı, filtre seçeneklerini belirtebilir veya verilerin nasıl yükleneceğini belirtmek için kendi LoadFilter'ını uygulayabilir.

**Example**

Aşağıdaki örnek, çalışma sayfasının özelliklerine göre filtre seçeneklerinin nasıl belirleneceğini gösterir.

```
         class LoadFilterSheet extends LoadFilter
         {
             public /*override*/ void startSheet(Worksheet sheet) 
             {
                 if ("Sheet1".equals(sheet.getName()))
                 {
                     setLoadDataFilterOptions(LoadDataFilterOptions.ALL);
                 }
                 else
                 {
                     setLoadDataFilterOptions(LoadDataFilterOptions.STRUCTURE);
                 }
             }
         }
         LoadOptions opts = new LoadOptions();
         opts.setLoadFilter(new LoadFilterSheet());
         Workbook wb = new Workbook("template.xlsx", opts);
         //Custom LoadFilter implementation
```
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [LoadFilter()](#LoadFilter--) | Varsayılan filtre seçenekleri LoadDataFilterOptions.All ile bir LoadFilter oluşturur. |
| [LoadFilter(int opts)](#LoadFilter-int-) | Verilen filtre seçenekleriyle bir LoadFilter oluşturur. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getLoadDataFilterOptions()](#getLoadDataFilterOptions--) | Yüklenmesi gereken verileri belirtmek için filtre seçenekleri. |
| [getSheetsInLoadingOrder()](#getSheetsInLoadingOrder--) | Yüklenmesi gereken sayfaları (indekslerini) ve sıralamayı belirtir. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setLoadDataFilterOptions(int value)](#setLoadDataFilterOptions-int-) | Yüklenmesi gereken verileri belirtmek için filtre seçenekleri. |
| [startSheet(Worksheet sheet)](#startSheet-com.aspose.cells.Worksheet-) | Verilen çalışma sayfası yüklenmeden önce filtre seçeneklerini hazırlar. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### LoadFilter() {#LoadFilter--}
```
public LoadFilter()
```


Varsayılan filtre seçenekleri LoadDataFilterOptions.All ile bir LoadFilter oluşturur.

### LoadFilter(int opts) {#LoadFilter-int-}
```
public LoadFilter(int opts)
```


Verilen filtre seçenekleriyle bir LoadFilter oluşturur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| opts | int | [LoadDataFilterOptions](../../com.aspose.cells/loaddatafilteroptions). varsayılan filtre seçenekleri |

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
### getLoadDataFilterOptions() {#getLoadDataFilterOptions--}
```
public int getLoadDataFilterOptions()
```


Yüklenmesi gereken verileri belirtmek için filtre seçenekleri.

[LoadDataFilterOptions](../../com.aspose.cells/loaddatafilteroptions) adresine bakın.

**Returns:**
int
### getSheetsInLoadingOrder() {#getSheetsInLoadingOrder--}
```
public int[] getSheetsInLoadingOrder()
```


Yüklenmesi gereken sayfaları (indekslerini) ve sıralamayı belirtir. Varsayılan değer null'dır, bu da şablon dosyasındaki tüm sayfaların varsayılan sırayla yükleneceği anlamına gelir. Null değilse ve bazı sayfa indeksleri dönen dizide yoksa, o sayfa yüklenmez.

**Returns:**
int[]
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




### setLoadDataFilterOptions(int value) {#setLoadDataFilterOptions-int-}
```
public void setLoadDataFilterOptions(int value)
```


Yüklenmesi gereken verileri belirtmek için filtre seçenekleri.

[LoadDataFilterOptions](../../com.aspose.cells/loaddatafilteroptions) adresine bakın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### startSheet(Worksheet sheet) {#startSheet-com.aspose.cells.Worksheet-}
```
public void startSheet(Worksheet sheet)
```


Verilen çalışma sayfası yüklenmeden önce filtre seçeneklerini hazırlar. Kullanıcının LoadFilter uygulaması, bu çalışma sayfası için verilerin nasıl yükleneceğini belirtmek amacıyla LoadDataFilterOptions'ı burada değiştirebilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sheet | [Worksheet](../../com.aspose.cells/worksheet) | Yüklenecek çalışma sayfası. Burada verilen çalışma sayfası nesnesi için yalnızca birkaç özellik kullanılabilir çünkü çoğu veri ve özellik yüklenmemiştir. Kullanılabilir özellikler: Name, Index, VisibilityType |

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

