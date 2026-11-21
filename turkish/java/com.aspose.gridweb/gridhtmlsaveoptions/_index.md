---
title: "GridHtmlSaveOptions"
second_title: "Aspose.Cells for Java API Referansı"
description: "HTML dosyasını kaydetme seçeneklerini temsil eder."
type: docs
url: /tr/java/com.aspose.gridweb/gridhtmlsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.GridSaveOptions](../../com.aspose.gridweb/gridsaveoptions)
```
public class GridHtmlSaveOptions extends GridSaveOptions
```

HTML dosyasını kaydetme seçeneklerini temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [GridHtmlSaveOptions()](#GridHtmlSaveOptions--) | html dosyası kaydetmek için seçenekler oluşturur. |
| [GridHtmlSaveOptions(int format)](#GridHtmlSaveOptions-int-) | htm dosyası kaydetmek için seçenekler oluşturur. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAttachedFilesDirectory()](#getAttachedFilesDirectory--) | Ekli dosyaların kaydedileceği dizin. |
| [getAttachedFilesUrlPrefix()](#getAttachedFilesUrlPrefix--) | HTML dosyasındaki resim gibi ekli dosyaların URL önekini belirtin. |
| [getCachedFileFolder()](#getCachedFileFolder--) | Önbelleğe alınmış dosya klasörü, bazı büyük verileri depolamak için kullanılır. |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | Dosya kaydedildikten sonra çalışma kitabını boşalt. |
| [getCreateDirectory()](#getCreateDirectory--) | Doğru ise ve dizin mevcut değilse, dosya kaydedilmeden önce dizin otomatik olarak oluşturulur. |
| [getDefaultFontName()](#getDefaultFontName--) | HTML dışa aktarımı için varsayılan yazı tipi adını belirtin, stilin yazı tipi mevcut değilse varsayılan yazı tipi kullanılacaktır. Bu özellik null ise, Aspose.Cells aynı aileye sahip evrensel bir yazı tipi kullanır, varsayılan değer null'dur. |
| [getEncoding()](#getEncoding--) | Ayarlanmamışsa, varsayılan kodlama türü olarak Encoding.UTF8 kullanılır. |
| [getExportActiveWorksheetOnly()](#getExportActiveWorksheetOnly--) | Tüm çalışma kitabının html dosyasına aktarılıp aktarılmayacağını gösterir. |
| [getExportArea()](#getExportArea--) | Mevcut etkin Çalışma Sayfasının dışa aktarım CellArea'ını alır. |
| [getExportGridLines()](#getExportGridLines--) | Izgara çizgilerinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'tur. |
| [getExportHeadings()](#getExportHeadings--) | Dosya html olarak kaydedilirken başlıkların aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'tur. |
| [getExportHiddenWorksheet()](#getExportHiddenWorksheet--) | Gizli çalışma sayfası içeriğinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer true'tur. |
| [getExportImagesAsBase64()](#getExportImagesAsBase64--) | Görüntülerin HTML, MHTML veya EPUB'a Base64 formatında kaydedilip kaydedilmeyeceğini belirtir. |
| [getExportPrintAreaOnly()](#getExportPrintAreaOnly--) | Yazdırma alanının yalnızca HTML dosyasına dışa aktarılıp aktarılmayacağını gösterir. |
| [getExportSingleTab()](#getExportSingleTab--) | Dosyada yalnızca bir çalışma sayfası olduğunda tek sekmenin dışa aktarılıp aktarılmayacağını gösterir. |
| [getMergeAreas()](#getMergeAreas--) | Dosya kaydedilmeden önce koşullu biçimlendirme ve doğrulama alanlarının birleştirilip birleştirilmeyeceğini gösterir. |
| [getPageTitle()](#getPageTitle--) | HTML sayfasının başlığı. |
|  | [getParseHtmlTagInCell()](#getParseHtmlTagInCell--) | Hücrede html etiketini ayrıştır, örnek |

 , hücre değeri olarak, ya da html etiketi olarak, varsayılan true |
| [getPresentationPreference()](#getPresentationPreference--) | Html veya mht dosyasının sunum tercihi olup olmadığını gösterir. Varsayılan değer false'tur. Daha güzel bir sunum istiyorsanız, değeri true olarak ayarlayın. |
| [getRefreshChartCache()](#getRefreshChartCache--) | Grafik önbellek verisinin yenilenip yenilenmediğini gösterir. |
| [getSaveFormat()](#getSaveFormat--) | Kaydetme dosya formatını alır. |
| [getSortNames()](#getSortNames--) | Dosya kaydedilmeden önce tanımlı adların sıralanıp sıralanmayacağını gösterir. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | Dosya kaydedilmeden önce birleştirilmiş hücrelerin doğrulanıp doğrulanmayacağını gösterir. |
| [hashCode()](#hashCode--) |  |
| [isExportComments()](#isExportComments--) | Dosya HTML'ye kaydedilirken yorumların dışa aktarılıp aktarılmayacağını gösterir, varsayılan değer false'tur. |
| [isFullPathLink()](#isFullPathLink--) | sheet00x.htm, filelist.xml ve tabstrip.htm dosyalarında tam yol bağlantısı kullanılıp kullanılmayacağını belirtiyor. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAttachedFilesDirectory(String value)](#setAttachedFilesDirectory-java.lang.String-) | Ekli dosyaların kaydedileceği dizin. |
| [setAttachedFilesUrlPrefix(String value)](#setAttachedFilesUrlPrefix-java.lang.String-) | HTML dosyasındaki resim gibi ekli dosyaların URL önekini belirtin. |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | Önbelleğe alınmış dosya klasörü, bazı büyük verileri depolamak için kullanılır. |
| [setClearData(boolean value)](#setClearData-boolean-) | Dosya kaydedildikten sonra çalışma kitabını boşalt. |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | Doğru ise ve dizin mevcut değilse, dosya kaydedilmeden önce dizin otomatik olarak oluşturulur. |
| [setDefaultFontName(String value)](#setDefaultFontName-java.lang.String-) | HTML dışa aktarımı için varsayılan yazı tipi adını belirtin, stilin yazı tipi mevcut değilse varsayılan yazı tipi kullanılacaktır. Bu özellik null ise, Aspose.Cells aynı aileye sahip evrensel bir yazı tipi kullanır, varsayılan değer null'dur. |
| [setEncoding(Encoding value)](#setEncoding-com.aspose.gridweb.Encoding-) | Ayarlanmamışsa, varsayılan kodlama türü olarak Encoding.UTF8 kullanılır. |
| [setExportActiveWorksheetOnly(boolean value)](#setExportActiveWorksheetOnly-boolean-) | Tüm çalışma kitabının html dosyasına aktarılıp aktarılmayacağını gösterir. |
| [setExportArea(GridCellArea value)](#setExportArea-com.aspose.gridweb.GridCellArea-) | Geçerli aktif Worksheet'ın dışa aktarma CellArea'sını ayarlar. |
| [setExportComments(boolean value)](#setExportComments-boolean-) | Dosya HTML'ye kaydedilirken yorumların dışa aktarılıp aktarılmayacağını gösterir, varsayılan değer false'tur. |
| [setExportGridLines(boolean value)](#setExportGridLines-boolean-) | Izgara çizgilerinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'tur. |
| [setExportHeadings(boolean value)](#setExportHeadings-boolean-) | Dosya html olarak kaydedilirken başlıkların aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'tur. |
| [setExportHiddenWorksheet(boolean value)](#setExportHiddenWorksheet-boolean-) | Gizli çalışma sayfası içeriğinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer true'tur. |
| [setExportImagesAsBase64(boolean value)](#setExportImagesAsBase64-boolean-) | Görüntülerin HTML, MHTML veya EPUB'a Base64 formatında kaydedilip kaydedilmeyeceğini belirtir. |
| [setExportPrintAreaOnly(boolean value)](#setExportPrintAreaOnly-boolean-) | Yazdırma alanının yalnızca HTML dosyasına dışa aktarılıp aktarılmayacağını gösterir. |
| [setExportSingleTab(boolean value)](#setExportSingleTab-boolean-) | Dosyada yalnızca bir çalışma sayfası olduğunda tek sekmenin dışa aktarılıp aktarılmayacağını gösterir. |
| [setFullPathLink(boolean value)](#setFullPathLink-boolean-) | sheet00x.htm, filelist.xml ve tabstrip.htm dosyalarında tam yol bağlantısı kullanılıp kullanılmayacağını belirtiyor. |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | Dosya kaydedilmeden önce koşullu biçimlendirme ve doğrulama alanlarının birleştirilip birleştirilmeyeceğini gösterir. |
| [setPageTitle(String value)](#setPageTitle-java.lang.String-) | HTML sayfasının başlığı. |
|  | [setParseHtmlTagInCell(boolean value)](#setParseHtmlTagInCell-boolean-) | Hücrede html etiketini ayrıştır, örnek |

 , hücre değeri olarak, ya da html etiketi olarak, varsayılan true |
| [setPresentationPreference(boolean value)](#setPresentationPreference-boolean-) | Html veya mht dosyasının sunum tercihi olup olmadığını gösterir. Varsayılan değer false'tur. Daha güzel bir sunum istiyorsanız, değeri true olarak ayarlayın. |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | Grafik önbellek verisinin yenilenip yenilenmediğini gösterir. |
| [setSortNames(boolean value)](#setSortNames-boolean-) | Dosya kaydedilmeden önce tanımlı adların sıralanıp sıralanmayacağını gösterir. |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | Dosya kaydedilmeden önce birleştirilmiş hücrelerin doğrulanıp doğrulanmayacağını gösterir. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridHtmlSaveOptions() {#GridHtmlSaveOptions--}
```
public GridHtmlSaveOptions()
```


html dosyası kaydetmek için seçenekler oluşturur.

### GridHtmlSaveOptions(int format) {#GridHtmlSaveOptions-int-}
```
public GridHtmlSaveOptions(int format)
```


htm dosyası kaydetmek için seçenekler oluşturur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| format | int | [GridSaveFormat](../../com.aspose.gridweb/gridsaveformat). Kaydedilen dosya formatı. |

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
### getAttachedFilesDirectory() {#getAttachedFilesDirectory--}
```
public String getAttachedFilesDirectory()
```


Ekli dosyaların kaydedileceği dizin. Yalnızca html akışına kaydederken kullanılır.

**Returns:**
java.lang.String
### getAttachedFilesUrlPrefix() {#getAttachedFilesUrlPrefix--}
```
public String getAttachedFilesUrlPrefix()
```


Html dosyasındaki resim gibi ekli dosyaların Url önekini belirtin. Yalnızca html akışına kaydederken kullanılır.

**Returns:**
java.lang.String
### getCachedFileFolder() {#getCachedFileFolder--}
```
public String getCachedFileFolder()
```


Önbelleğe alınmış dosya klasörü, bazı büyük verileri depolamak için kullanılır.

**Returns:**
java.lang.String
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getClearData() {#getClearData--}
```
public boolean getClearData()
```


Dosya kaydedildikten sonra çalışma kitabını boşalt.

**Returns:**
boolean
### getCreateDirectory() {#getCreateDirectory--}
```
public boolean getCreateDirectory()
```


Doğru ise ve dizin mevcut değilse, dosya kaydedilmeden önce dizin otomatik olarak oluşturulur.

**Remarks**

Varsayılan değer false'tur.

**Returns:**
boolean
### getDefaultFontName() {#getDefaultFontName--}
```
public String getDefaultFontName()
```


HTML dışa aktarımı için varsayılan yazı tipi adını belirtin, stilin yazı tipi mevcut değilse varsayılan yazı tipi kullanılacaktır. Bu özellik null ise, Aspose.Cells aynı aileye sahip evrensel bir yazı tipi kullanır, varsayılan değer null'dur.

**Returns:**
java.lang.String
### getEncoding() {#getEncoding--}
```
public Encoding getEncoding()
```


Ayarlanmamışsa, varsayılan kodlama türü olarak Encoding.UTF8 kullanılır.

**Returns:**
[Encoding](../../com.aspose.gridweb/encoding)
### getExportActiveWorksheetOnly() {#getExportActiveWorksheetOnly--}
```
public boolean getExportActiveWorksheetOnly()
```


Tüm çalışma kitabının html dosyasına aktarılıp aktarılmayacağını gösterir.

**Returns:**
boolean
### getExportArea() {#getExportArea--}
```
public GridCellArea getExportArea()
```


Mevcut aktif Worksheet'in dışa aktarılan CellArea'sını alır. Bu özelliği ayarlarsanız, mevcut aktif Worksheet'in yazdırma alanı göz ardı edilir. Dosya html olarak kaydedilirken yalnızca belirtilen alan dışa aktarılır.

**Returns:**
[GridCellArea](../../com.aspose.gridweb/gridcellarea)
### getExportGridLines() {#getExportGridLines--}
```
public boolean getExportGridLines()
```


Izgara çizgilerinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'tur.

**Returns:**
boolean
### getExportHeadings() {#getExportHeadings--}
```
public boolean getExportHeadings()
```


Dosya html olarak kaydedilirken başlıkların aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'tur. Html dosyasını excel'e aktarmak istiyorsanız, varsayılan değeri koruyun.

**Returns:**
boolean
### getExportHiddenWorksheet() {#getExportHiddenWorksheet--}
```
public boolean getExportHiddenWorksheet()
```


Gizli çalışma sayfası içeriğinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer true'tur.

**Returns:**
boolean
### getExportImagesAsBase64() {#getExportImagesAsBase64--}
```
public boolean getExportImagesAsBase64()
```


Görüntülerin HTML, MHTML veya EPUB'a Base64 formatında kaydedilip kaydedilmeyeceğini belirtir.

**Remarks**

Bu özellik true olarak ayarlandığında görüntü verileri doğrudan img öğelerine dışa aktarılır ve ayrı dosyalar oluşturulmaz.

**Returns:**
boolean
### getExportPrintAreaOnly() {#getExportPrintAreaOnly--}
```
public boolean getExportPrintAreaOnly()
```


Yalnızca yazdırma alanının html dosyasına dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'tur.

**Returns:**
boolean
### getExportSingleTab() {#getExportSingleTab--}
```
public boolean getExportSingleTab()
```


Dosyada yalnızca bir çalışma sayfası olduğunda tek sekmenin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'tur.

**Returns:**
boolean
### getMergeAreas() {#getMergeAreas--}
```
public boolean getMergeAreas()
```


Dosya kaydedilmeden önce koşullu biçimlendirme ve doğrulama alanlarının birleştirilip birleştirilmeyeceğini gösterir.

**Remarks**

Varsayılan değer false'tur.

**Returns:**
boolean
### getPageTitle() {#getPageTitle--}
```
public String getPageTitle()
```


HTML sayfasının başlığı. Yalnızca HTML akışına kaydetmek için.

**Returns:**
java.lang.String
### getParseHtmlTagInCell() {#getParseHtmlTagInCell--}
```
public boolean getParseHtmlTagInCell()
```


Hücrede html etiketini ayrıştır, örnek

 , hücre değeri olarak, ya da html etiketi olarak, varsayılan true

**Returns:**
boolean
### getPresentationPreference() {#getPresentationPreference--}
```
public boolean getPresentationPreference()
```


Html veya mht dosyasının sunum tercihi olup olmadığını gösterir. Varsayılan değer false'tur. Daha güzel bir sunum istiyorsanız, değeri true olarak ayarlayın.

**Returns:**
boolean
### getRefreshChartCache() {#getRefreshChartCache--}
```
public boolean getRefreshChartCache()
```


Grafik önbellek verisinin yenilenip yenilenmediğini gösterir.

**Returns:**
boolean
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Kaydetme dosya formatını alır.

Bakınız [GridSaveFormat](../../com.aspose.gridweb/gridsaveformat).

**Returns:**
int
### getSortNames() {#getSortNames--}
```
public boolean getSortNames()
```


Dosya kaydedilmeden önce tanımlı adların sıralanıp sıralanmayacağını gösterir.

**Returns:**
boolean
### getValidateMergedAreas() {#getValidateMergedAreas--}
```
public boolean getValidateMergedAreas()
```


Dosya kaydedilmeden önce birleştirilmiş hücrelerin doğrulanıp doğrulanmayacağını gösterir.

**Remarks**

Varsayılan değer false'tur.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isExportComments() {#isExportComments--}
```
public boolean isExportComments()
```


Dosya HTML'ye kaydedilirken yorumların dışa aktarılıp aktarılmayacağını gösterir, varsayılan değer false'tur.

**Returns:**
boolean
### isFullPathLink() {#isFullPathLink--}
```
public boolean isFullPathLink()
```


sheet00x.htm, filelist.xml ve tabstrip.htm dosyalarında tam yol bağlantısı kullanılıp kullanılmayacağını belirtir. Varsayılan değer false'tur.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setAttachedFilesDirectory(String value) {#setAttachedFilesDirectory-java.lang.String-}
```
public void setAttachedFilesDirectory(String value)
```


Ekli dosyaların kaydedileceği dizin. Yalnızca html akışına kaydederken kullanılır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setAttachedFilesUrlPrefix(String value) {#setAttachedFilesUrlPrefix-java.lang.String-}
```
public void setAttachedFilesUrlPrefix(String value)
```


Html dosyasındaki resim gibi ekli dosyaların Url önekini belirtin. Yalnızca html akışına kaydederken kullanılır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setCachedFileFolder(String value) {#setCachedFileFolder-java.lang.String-}
```
public void setCachedFileFolder(String value)
```


Önbelleğe alınmış dosya klasörü, bazı büyük verileri depolamak için kullanılır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setClearData(boolean value) {#setClearData-boolean-}
```
public void setClearData(boolean value)
```


Dosya kaydedildikten sonra çalışma kitabını boşalt.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setCreateDirectory(boolean value) {#setCreateDirectory-boolean-}
```
public void setCreateDirectory(boolean value)
```


Doğru ise ve dizin mevcut değilse, dosya kaydedilmeden önce dizin otomatik olarak oluşturulur.

**Remarks**

Varsayılan değer false'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setDefaultFontName(String value) {#setDefaultFontName-java.lang.String-}
```
public void setDefaultFontName(String value)
```


HTML dışa aktarımı için varsayılan yazı tipi adını belirtin, stilin yazı tipi mevcut değilse varsayılan yazı tipi kullanılacaktır. Bu özellik null ise, Aspose.Cells aynı aileye sahip evrensel bir yazı tipi kullanır, varsayılan değer null'dur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setEncoding(Encoding value) {#setEncoding-com.aspose.gridweb.Encoding-}
```
public void setEncoding(Encoding value)
```


Ayarlanmamışsa, varsayılan kodlama türü olarak Encoding.UTF8 kullanılır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Encoding](../../com.aspose.gridweb/encoding) |  |

### setExportActiveWorksheetOnly(boolean value) {#setExportActiveWorksheetOnly-boolean-}
```
public void setExportActiveWorksheetOnly(boolean value)
```


Tüm çalışma kitabının html dosyasına aktarılıp aktarılmayacağını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setExportArea(GridCellArea value) {#setExportArea-com.aspose.gridweb.GridCellArea-}
```
public void setExportArea(GridCellArea value)
```


Mevcut aktif Worksheet'in dışa aktarılan CellArea'sını ayarlar. Bu özelliği ayarlarsanız, mevcut aktif Worksheet'in yazdırma alanı göz ardı edilir. Dosya html olarak kaydedilirken yalnızca belirtilen alan dışa aktarılır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [GridCellArea](../../com.aspose.gridweb/gridcellarea) |  |

### setExportComments(boolean value) {#setExportComments-boolean-}
```
public void setExportComments(boolean value)
```


Dosya HTML'ye kaydedilirken yorumların dışa aktarılıp aktarılmayacağını gösterir, varsayılan değer false'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setExportGridLines(boolean value) {#setExportGridLines-boolean-}
```
public void setExportGridLines(boolean value)
```


Izgara çizgilerinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setExportHeadings(boolean value) {#setExportHeadings-boolean-}
```
public void setExportHeadings(boolean value)
```


Dosya html olarak kaydedilirken başlıkların aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'tur. Html dosyasını excel'e aktarmak istiyorsanız, varsayılan değeri koruyun.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setExportHiddenWorksheet(boolean value) {#setExportHiddenWorksheet-boolean-}
```
public void setExportHiddenWorksheet(boolean value)
```


Gizli çalışma sayfası içeriğinin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer true'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setExportImagesAsBase64(boolean value) {#setExportImagesAsBase64-boolean-}
```
public void setExportImagesAsBase64(boolean value)
```


Görüntülerin HTML, MHTML veya EPUB'a Base64 formatında kaydedilip kaydedilmeyeceğini belirtir.

**Remarks**

Bu özellik true olarak ayarlandığında görüntü verileri doğrudan img öğelerine dışa aktarılır ve ayrı dosyalar oluşturulmaz.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setExportPrintAreaOnly(boolean value) {#setExportPrintAreaOnly-boolean-}
```
public void setExportPrintAreaOnly(boolean value)
```


Yalnızca yazdırma alanının html dosyasına dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setExportSingleTab(boolean value) {#setExportSingleTab-boolean-}
```
public void setExportSingleTab(boolean value)
```


Dosyada yalnızca bir çalışma sayfası olduğunda tek sekmenin dışa aktarılıp aktarılmayacağını gösterir. Varsayılan değer false'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setFullPathLink(boolean value) {#setFullPathLink-boolean-}
```
public void setFullPathLink(boolean value)
```


sheet00x.htm, filelist.xml ve tabstrip.htm dosyalarında tam yol bağlantısı kullanılıp kullanılmayacağını belirtir. Varsayılan değer false'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setMergeAreas(boolean value) {#setMergeAreas-boolean-}
```
public void setMergeAreas(boolean value)
```


Dosya kaydedilmeden önce koşullu biçimlendirme ve doğrulama alanlarının birleştirilip birleştirilmeyeceğini gösterir.

**Remarks**

Varsayılan değer false'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setPageTitle(String value) {#setPageTitle-java.lang.String-}
```
public void setPageTitle(String value)
```


HTML sayfasının başlığı. Yalnızca HTML akışına kaydetmek için.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setParseHtmlTagInCell(boolean value) {#setParseHtmlTagInCell-boolean-}
```
public void setParseHtmlTagInCell(boolean value)
```


Hücrede html etiketini ayrıştır, örnek

 , hücre değeri olarak, ya da html etiketi olarak, varsayılan true

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setPresentationPreference(boolean value) {#setPresentationPreference-boolean-}
```
public void setPresentationPreference(boolean value)
```


Html veya mht dosyasının sunum tercihi olup olmadığını gösterir. Varsayılan değer false'tur. Daha güzel bir sunum istiyorsanız, değeri true olarak ayarlayın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setRefreshChartCache(boolean value) {#setRefreshChartCache-boolean-}
```
public void setRefreshChartCache(boolean value)
```


Grafik önbellek verisinin yenilenip yenilenmediğini gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setSortNames(boolean value) {#setSortNames-boolean-}
```
public void setSortNames(boolean value)
```


Dosya kaydedilmeden önce tanımlı adların sıralanıp sıralanmayacağını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setValidateMergedAreas(boolean value) {#setValidateMergedAreas-boolean-}
```
public void setValidateMergedAreas(boolean value)
```


Dosya kaydedilmeden önce birleştirilmiş hücrelerin doğrulanıp doğrulanmayacağını gösterir.

**Remarks**

Varsayılan değer false'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

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

