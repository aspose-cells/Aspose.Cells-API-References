---
title: "PdfSecurityOptions"
second_title: "Aspose.Cells for Java API Referansı"
description: "Bir PDF belgesi için şifreleme ve erişim izinleri seçenekleri."
type: docs
url: /tr/java/com.aspose.cells/pdfsecurityoptions/
---

**Inheritance:**
java.lang.Object
```
public class PdfSecurityOptions
```

Bir PDF belgesi için şifreleme ve erişim izinleri seçenekleri. PDF/A güvenlik ayarına izin vermez.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [PdfSecurityOptions()](#PdfSecurityOptions--) | PdfSecurityOptions sınıfının yapıcı metodu |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAccessibilityExtractContent()](#getAccessibilityExtractContent--) | Metin ve grafik çıkarılmasına izin verilip verilmediğini gösterir (engelli kullanıcıların erişilebilirliğini desteklemek veya diğer amaçlar için). |
| [getAnnotationsPermission()](#getAnnotationsPermission--) | Metin açıklamaları eklenmesine veya değiştirilmesine, etkileşimli form alanlarının doldurulmasına izin verilip verilmediğini gösterir. |
| [getAssembleDocumentPermission()](#getAssembleDocumentPermission--) | Belgenin birleştirilmesine (sayfaları ekleme, döndürme veya silme ve yer imleri veya küçük resimler oluşturma) izin verilip verilmediğini gösterir, hatta [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) temiz olsa bile. |
| [getClass()](#getClass--) |  |
| [getExtractContentPermission()](#getExtractContentPermission--) | Belgeden metin ve grafikleri kopyalamaya veya başka yollarla çıkarmaya izin verilip verilmediğini gösterir; bu, [getAccessibilityExtractContent()](../../com.aspose.cells/pdfsecurityoptions\#getAccessibilityExtractContent--) tarafından kontrol edilen işlemler dışında gerçekleşir. |
| [getExtractContentPermissionObsolete()](#getExtractContentPermissionObsolete--) | PDF referansına göre kopyalama veya içerik çıkarma izni artık kullanılmamaktadır. |
| [getFillFormsPermission()](#getFillFormsPermission--) | Mevcut etkileşimli form alanlarını (imza alanları dahil) doldurmaya izin verilip verilmediğini gösterir, hatta [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) temiz olsa bile. |
| [getFullQualityPrintPermission()](#getFullQualityPrintPermission--) | PDF içeriğinin doğru bir dijital kopyasının oluşturulabileceği bir temsile belgeyi yazdırmaya izin verilip verilmediğini gösterir. |
| [getModifyDocumentPermission()](#getModifyDocumentPermission--) | Belgenin içeriğini, [getAnnotationsPermission()](../../com.aspose.cells/pdfsecurityoptions\#getAnnotationsPermission--), [getFillFormsPermission()](../../com.aspose.cells/pdfsecurityoptions\#getFillFormsPermission--) ve [getAssembleDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getAssembleDocumentPermission--) tarafından kontrol edilen işlemler dışındaki işlemlerle değiştirmeye izin verilip verilmediğini gösterir. |
| [getOwnerPassword()](#getOwnerPassword--) | Şifrelenmiş PDF belgesi için sahibi şifresini alır. |
| [getPrintPermission()](#getPrintPermission--) | Belgenin yazdırılmasına izin verilip verilmediğini gösterir. |
| [getUserPassword()](#getUserPassword--) | Şifrelenmiş PDF belgesini açmak için gereken kullanıcı şifresini alır. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAccessibilityExtractContent(boolean value)](#setAccessibilityExtractContent-boolean-) | Metin ve grafik çıkarılmasına izin verilip verilmediğini gösterir (engelli kullanıcıların erişilebilirliğini desteklemek veya diğer amaçlar için). |
| [setAnnotationsPermission(boolean value)](#setAnnotationsPermission-boolean-) | Metin açıklamaları eklenmesine veya değiştirilmesine, etkileşimli form alanlarının doldurulmasına izin verilip verilmediğini gösterir. |
| [setAssembleDocumentPermission(boolean value)](#setAssembleDocumentPermission-boolean-) | Belgenin birleştirilmesine (sayfaları ekleme, döndürme veya silme ve yer imleri veya küçük resimler oluşturma) izin verilip verilmediğini gösterir, hatta [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) temiz olsa bile. |
| [setExtractContentPermission(boolean value)](#setExtractContentPermission-boolean-) | Belgeden metin ve grafikleri kopyalamaya veya başka yollarla çıkarmaya izin verilip verilmediğini gösterir; bu, [getAccessibilityExtractContent()](../../com.aspose.cells/pdfsecurityoptions\#getAccessibilityExtractContent--) tarafından kontrol edilen işlemler dışında gerçekleşir. |
| [setExtractContentPermissionObsolete(boolean value)](#setExtractContentPermissionObsolete-boolean-) | PDF referansına göre kopyalama veya içerik çıkarma izni artık kullanılmamaktadır. |
| [setFillFormsPermission(boolean value)](#setFillFormsPermission-boolean-) | Mevcut etkileşimli form alanlarını (imza alanları dahil) doldurmaya izin verilip verilmediğini gösterir, hatta [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) temiz olsa bile. |
| [setFullQualityPrintPermission(boolean value)](#setFullQualityPrintPermission-boolean-) | PDF içeriğinin doğru bir dijital kopyasının oluşturulabileceği bir temsile belgeyi yazdırmaya izin verilip verilmediğini gösterir. |
| [setModifyDocumentPermission(boolean value)](#setModifyDocumentPermission-boolean-) | Belgenin içeriğini, [getAnnotationsPermission()](../../com.aspose.cells/pdfsecurityoptions\#getAnnotationsPermission--), [getFillFormsPermission()](../../com.aspose.cells/pdfsecurityoptions\#getFillFormsPermission--) ve [getAssembleDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getAssembleDocumentPermission--) tarafından kontrol edilen işlemler dışındaki işlemlerle değiştirmeye izin verilip verilmediğini gösterir. |
| [setOwnerPassword(String value)](#setOwnerPassword-java.lang.String-) | Şifrelenmiş PDF belgesi için sahibi şifresini ayarlar. |
| [setPrintPermission(boolean value)](#setPrintPermission-boolean-) | Belgenin yazdırılmasına izin verilip verilmediğini gösterir. |
| [setUserPassword(String value)](#setUserPassword-java.lang.String-) | Şifrelenmiş PDF belgesini açmak için gereken kullanıcı şifresini ayarlar. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PdfSecurityOptions() {#PdfSecurityOptions--}
```
public PdfSecurityOptions()
```


PdfSecurityOptions sınıfının yapıcı metodu

**Example**

Aşağıdaki kod, çıktı PDF'si için yüksek çözünürlüklü yazdırma izni ayarlar.

```
         Workbook wb = new Workbook();
         wb.getWorksheets().get(0).getCells().get("A1").setValue("Aspose");
 
         PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
 
 
         PdfSecurityOptions pdfSecurityOptions = new PdfSecurityOptions();
 
         //set owner password
         pdfSecurityOptions.setOwnerPassword("YourOwnerPassword");
 
         //set user password
         pdfSecurityOptions.setUserPassword("YourUserPassword");
 
         //set print permisson
         pdfSecurityOptions.setPrintPermission(true);
 
         //set high resolution for print
         pdfSecurityOptions.setFullQualityPrintPermission(true);
 
 
         pdfSaveOptions.setSecurityOptions(pdfSecurityOptions);
 
         wb.save("output.pdf", pdfSaveOptions);
```

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
### getAccessibilityExtractContent() {#getAccessibilityExtractContent--}
```
public boolean getAccessibilityExtractContent()
```


Metin ve grafik çıkarılmasına izin verilip verilmediğini gösterir (engelli kullanıcıların erişilebilirliğini desteklemek veya diğer amaçlar için).

**Returns:**
boolean
### getAnnotationsPermission() {#getAnnotationsPermission--}
```
public boolean getAnnotationsPermission()
```


Metin açıklamaları eklenmesine veya değiştirilmesine, etkileşimli form alanlarının doldurulmasına izin verilip verilmediğini gösterir.

**Remarks**

Eğer [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) de ayarlanmışsa, etkileşimli form alanlarını (imza alanları dahil) oluşturur veya değiştirir.

**Returns:**
boolean
### getAssembleDocumentPermission() {#getAssembleDocumentPermission--}
```
public boolean getAssembleDocumentPermission()
```


Belgenin birleştirilmesine (sayfaları ekleme, döndürme veya silme ve yer imleri veya küçük resimler oluşturma) izin verilip verilmediğini gösterir, hatta [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) temiz olsa bile.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getExtractContentPermission() {#getExtractContentPermission--}
```
public boolean getExtractContentPermission()
```


Belgeden metin ve grafikleri kopyalamaya veya başka yollarla çıkarmaya izin verilip verilmediğini gösterir; bu, [getAccessibilityExtractContent()](../../com.aspose.cells/pdfsecurityoptions\#getAccessibilityExtractContent--) tarafından kontrol edilen işlemler dışında gerçekleşir.

**Returns:**
boolean
### getExtractContentPermissionObsolete() {#getExtractContentPermissionObsolete--}
```
public boolean getExtractContentPermissionObsolete()
```


PDF referansına göre kopyalama veya içerik çıkarma izni artık kullanılmamaktadır.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen ExtractContentPermission özelliğini kullanın. Bu özellik Eylül 2023'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
boolean
### getFillFormsPermission() {#getFillFormsPermission--}
```
public boolean getFillFormsPermission()
```


Mevcut etkileşimli form alanlarını (imza alanları dahil) doldurmaya izin verilip verilmediğini gösterir, hatta [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) temiz olsa bile.

**Returns:**
boolean
### getFullQualityPrintPermission() {#getFullQualityPrintPermission--}
```
public boolean getFullQualityPrintPermission()
```


PDF içeriğinin doğru bir dijital kopyasının oluşturulabileceği bir temsile belgeyi yazdırmaya izin verilip verilmediğini gösterir.

**Remarks**

Bu açık olduğunda (ve [getPrintPermission()](../../com.aspose.cells/pdfsecurityoptions\#getPrintPermission--) ayarlanmışsa), yazdırma, görünümün düşük seviyeli bir temsiliyle sınırlıdır; muhtemelen kalite kaybı yaşanabilir.

**Returns:**
boolean
### getModifyDocumentPermission() {#getModifyDocumentPermission--}
```
public boolean getModifyDocumentPermission()
```


Belgenin içeriğini, [getAnnotationsPermission()](../../com.aspose.cells/pdfsecurityoptions\#getAnnotationsPermission--), [getFillFormsPermission()](../../com.aspose.cells/pdfsecurityoptions\#getFillFormsPermission--) ve [getAssembleDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getAssembleDocumentPermission--) tarafından kontrol edilen işlemler dışındaki işlemlerle değiştirmeye izin verilip verilmediğini gösterir.

**Returns:**
boolean
### getOwnerPassword() {#getOwnerPassword--}
```
public String getOwnerPassword()
```


Şifrelenmiş PDF belgesi için sahibi şifresini alır.

**Remarks**

Sahibi şifresi, kullanıcının belirtilen herhangi bir erişim kısıtlaması olmadan şifrelenmiş bir PDF belgesini açmasına izin verir.

**Returns:**
java.lang.String
### getPrintPermission() {#getPrintPermission--}
```
public boolean getPrintPermission()
```


Belgenin yazdırılmasına izin verilip verilmediğini gösterir.

**Remarks**

Muhtemelen en yüksek kalite seviyesinde olmayabilir, [getFullQualityPrintPermission()](../../com.aspose.cells/pdfsecurityoptions\#getFullQualityPrintPermission--) de ayarlanmış olup olmadığına bağlı olarak.

**Returns:**
boolean
### getUserPassword() {#getUserPassword--}
```
public String getUserPassword()
```


Şifrelenmiş PDF belgesini açmak için gereken kullanıcı şifresini alır.

**Remarks**

Sahip şifresi veya kullanıcı şifresi, şifrelenmiş bir PDF belgesini görüntülemek için açarken gerekecektir.

Kullanıcı şifresi null veya boş bir dize olabilir, bu durumda PDF belgesi açılırken kullanıcıdan şifre istenmez.

Belgeyi doğru sahip şifresiyle açmak, belgeye tam erişim sağlar.

Belgeyi doğru kullanıcı şifresiyle (veya kullanıcı şifresi olmayan bir belgeyi) açmak, belirtilen izinler doğrultusunda sınırlı erişim sağlar.

**Returns:**
java.lang.String
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




### setAccessibilityExtractContent(boolean value) {#setAccessibilityExtractContent-boolean-}
```
public void setAccessibilityExtractContent(boolean value)
```


Metin ve grafik çıkarılmasına izin verilip verilmediğini gösterir (engelli kullanıcıların erişilebilirliğini desteklemek veya diğer amaçlar için).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setAnnotationsPermission(boolean value) {#setAnnotationsPermission-boolean-}
```
public void setAnnotationsPermission(boolean value)
```


Metin açıklamaları eklenmesine veya değiştirilmesine, etkileşimli form alanlarının doldurulmasına izin verilip verilmediğini gösterir.

**Remarks**

Eğer [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) de ayarlanmışsa, etkileşimli form alanlarını (imza alanları dahil) oluşturur veya değiştirir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setAssembleDocumentPermission(boolean value) {#setAssembleDocumentPermission-boolean-}
```
public void setAssembleDocumentPermission(boolean value)
```


Belgenin birleştirilmesine (sayfaları ekleme, döndürme veya silme ve yer imleri veya küçük resimler oluşturma) izin verilip verilmediğini gösterir, hatta [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) temiz olsa bile.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setExtractContentPermission(boolean value) {#setExtractContentPermission-boolean-}
```
public void setExtractContentPermission(boolean value)
```


Belgeden metin ve grafikleri kopyalamaya veya başka yollarla çıkarmaya izin verilip verilmediğini gösterir; bu, [getAccessibilityExtractContent()](../../com.aspose.cells/pdfsecurityoptions\#getAccessibilityExtractContent--) tarafından kontrol edilen işlemler dışında gerçekleşir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setExtractContentPermissionObsolete(boolean value) {#setExtractContentPermissionObsolete-boolean-}
```
public void setExtractContentPermissionObsolete(boolean value)
```


PDF referansına göre kopyalama veya içerik çıkarma izni artık kullanılmamaktadır.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen ExtractContentPermission özelliğini kullanın. Bu özellik Eylül 2023'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setFillFormsPermission(boolean value) {#setFillFormsPermission-boolean-}
```
public void setFillFormsPermission(boolean value)
```


Mevcut etkileşimli form alanlarını (imza alanları dahil) doldurmaya izin verilip verilmediğini gösterir, hatta [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getModifyDocumentPermission--) temiz olsa bile.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setFullQualityPrintPermission(boolean value) {#setFullQualityPrintPermission-boolean-}
```
public void setFullQualityPrintPermission(boolean value)
```


PDF içeriğinin doğru bir dijital kopyasının oluşturulabileceği bir temsile belgeyi yazdırmaya izin verilip verilmediğini gösterir.

**Remarks**

Bu açık olduğunda (ve [getPrintPermission()](../../com.aspose.cells/pdfsecurityoptions\#getPrintPermission--) ayarlanmışsa), yazdırma, görünümün düşük seviyeli bir temsiliyle sınırlıdır; muhtemelen kalite kaybı yaşanabilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setModifyDocumentPermission(boolean value) {#setModifyDocumentPermission-boolean-}
```
public void setModifyDocumentPermission(boolean value)
```


Belgenin içeriğini, [getAnnotationsPermission()](../../com.aspose.cells/pdfsecurityoptions\#getAnnotationsPermission--), [getFillFormsPermission()](../../com.aspose.cells/pdfsecurityoptions\#getFillFormsPermission--) ve [getAssembleDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\#getAssembleDocumentPermission--) tarafından kontrol edilen işlemler dışındaki işlemlerle değiştirmeye izin verilip verilmediğini gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setOwnerPassword(String value) {#setOwnerPassword-java.lang.String-}
```
public void setOwnerPassword(String value)
```


Şifrelenmiş PDF belgesi için sahibi şifresini ayarlar.

**Remarks**

Sahibi şifresi, kullanıcının belirtilen herhangi bir erişim kısıtlaması olmadan şifrelenmiş bir PDF belgesini açmasına izin verir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setPrintPermission(boolean value) {#setPrintPermission-boolean-}
```
public void setPrintPermission(boolean value)
```


Belgenin yazdırılmasına izin verilip verilmediğini gösterir.

**Remarks**

Muhtemelen en yüksek kalite seviyesinde olmayabilir, [getFullQualityPrintPermission()](../../com.aspose.cells/pdfsecurityoptions\#getFullQualityPrintPermission--) de ayarlanmış olup olmadığına bağlı olarak.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setUserPassword(String value) {#setUserPassword-java.lang.String-}
```
public void setUserPassword(String value)
```


Şifrelenmiş PDF belgesini açmak için gereken kullanıcı şifresini ayarlar.

**Remarks**

Sahip şifresi veya kullanıcı şifresi, şifrelenmiş bir PDF belgesini görüntülemek için açarken gerekecektir.

Kullanıcı şifresi null veya boş bir dize olabilir, bu durumda PDF belgesi açılırken kullanıcıdan şifre istenmez.

Belgeyi doğru sahip şifresiyle açmak, belgeye tam erişim sağlar.

Belgeyi doğru kullanıcı şifresiyle (veya kullanıcı şifresi olmayan bir belgeyi) açmak, belirtilen izinler doğrultusunda sınırlı erişim sağlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

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

