---
title: "Workbook"
second_title: "Aspose.Cells for Java API Referansı"
description: "Excel çalışma sayfası oluşturmak için bir kök nesneyi temsil eder."
type: docs
url: /tr/java/com.aspose.cells/workbook/
---

**Inheritance:**
java.lang.Object
```
public class Workbook
```

Excel çalışma sayfası oluşturmak için bir kök nesneyi temsil eder.

**Remarks**

Workbook sınıfı bir Excel çalışma sayfasını temsil eder. Her çalışma sayfası birden fazla çalışma sayfası (worksheet) içerebilir. Sınıfın temel özelliği yerel Excel dosyalarını açmak ve kaydetmektir. Sınıf, diğer Workbook'lerden veri kopyalama, iki Workbook'ı birleştirme, Excel'i PDF'ye dönüştürme, Excel'i görüntüye renderleme ve Excel çalışma sayfasını koruma gibi gelişmiş özelliklere sahiptir.

**Example**

Aşağıdaki örnek, designer.xls adlı bir Excel dosyasından bir Workbook yükler ve yatay ve dikey kaydırma çubuklarını görünmez yapar. Ardından, çalışma sayfası içinde iki dize değerini sırasıyla bir Tam sayı değeri ve bir dize değeriyle değiştirir ve sonunda workbook'u Excel xlsx dosyası olarak kaydeder.

```
         //Open a designer file
         String designerFile = "designer.xls";
         Workbook workbook = new Workbook(designerFile);
 
         //Set scroll bars
         workbook.getSettings().setHScrollBarVisible(false);
         workbook.getSettings().setVScrollBarVisible(false);
 
         //Replace the placeholder string with new values
         int newInt = 100;
         workbook.replace("OldInt", newInt);
 
         String newString = "Hello!";
         workbook.replace("OldString", newString);
         workbook.save("result.xlsx");
```
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [Workbook()](#Workbook--) | Yeni bir [Workbook](../../com.aspose.cells/workbook) sınıf örneği başlatır. |
| [Workbook(int fileFormatType)](#Workbook-int-) | Yeni bir [Workbook](../../com.aspose.cells/workbook) sınıf örneği başlatır. |
| [Workbook(LoadOptions loadOptions)](#Workbook-com.aspose.cells.LoadOptions-) | Seçeneklerle yeni boş bir [Workbook](../../com.aspose.cells/workbook) sınıf örneği başlatır |
| [Workbook(String file)](#Workbook-java.lang.String-) | Yeni bir [Workbook](../../com.aspose.cells/workbook) sınıf örneği başlatır ve bir dosya açar. |
| [Workbook(InputStream stream)](#Workbook-java.io.InputStream-) | Yeni bir [Workbook](../../com.aspose.cells/workbook) sınıf örneği başlatır ve bir akış açar. |
| [Workbook(String file, LoadOptions loadOptions)](#Workbook-java.lang.String-com.aspose.cells.LoadOptions-) | Yeni bir [Workbook](../../com.aspose.cells/workbook) sınıf örneği başlatır ve bir dosya açar. |
| [Workbook(InputStream stream, LoadOptions loadOptions)](#Workbook-java.io.InputStream-com.aspose.cells.LoadOptions-) | Yeni bir [Workbook](../../com.aspose.cells/workbook) sınıf örneği başlatır ve akışı açar. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [acceptAllRevisions()](#acceptAllRevisions--) | Çalışma kitabındaki tüm izlenen değişiklikleri kabul eder. |
| [addDigitalSignature(DigitalSignatureCollection digitalSignatureCollection)](#addDigitalSignature-com.aspose.cells.DigitalSignatureCollection-) | OOXML elektronik tablo dosyasına (Excel2007 ve sonrası) dijital imza ekler. |
| [calculateFormula()](#calculateFormula--) | Formüllerin sonucunu hesaplar. |
| [calculateFormula(boolean ignoreError)](#calculateFormula-boolean-) | Formüllerin sonucunu hesaplar. |
| [calculateFormula(CalculationOptions options)](#calculateFormula-com.aspose.cells.CalculationOptions-) | Bu çalışma kitabındaki formüller hesaplanıyor. |
| [changePalette(Color color, int index)](#changePalette-com.aspose.cells.Color-int-) | Belirtilen indeksteki elektronik tablo için paleti değiştirir. |
| [closeAccessCache(int opts)](#closeAccessCache-int-) | Veriye erişmek için önbellek kullanan oturumu kapatır. |
| [combine(Workbook secondWorkbook)](#combine-com.aspose.cells.Workbook-) | Başka bir Workbook nesnesiyle birleştirir. |
| [copy(Workbook source)](#copy-com.aspose.cells.Workbook-) | Kaynak bir Workbook nesnesinden verileri kopyalar. |
| [copy(Workbook source, CopyOptions copyOptions)](#copy-com.aspose.cells.Workbook-com.aspose.cells.CopyOptions-) | Başka bir Workbook nesnesini kopyalar. |
| [copyTheme(Workbook source)](#copyTheme-com.aspose.cells.Workbook-) | Başka bir çalışma kitabından temayı kopyalar. |
| [createBuiltinStyle(int type)](#createBuiltinStyle-int-) | Verilen tipe göre yerleşik stil oluşturur. |
| [createCellsColor()](#createCellsColor--) | Bir [CellsColor](../../com.aspose.cells/cellscolor) nesnesi oluşturur. |
| [createStyle()](#createStyle--) | Yeni bir stil oluşturur. |
| [createStyle(boolean cloneDefaultStyle)](#createStyle-boolean-) | Yeni bir stil oluşturur. |
| [customTheme(String themeName, Color[] colors)](#customTheme-java.lang.String-com.aspose.cells.Color---) | Temayı özelleştirir. |
| [dispose()](#dispose--) | Yönetilmeyen kaynakların serbest bırakılması, salınması veya sıfırlanmasıyla ilgili uygulama tanımlı görevleri yürütür. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [exportXml(String mapName, OutputStream stream)](#exportXml-java.lang.String-java.io.OutputStream-) | Belirtilen XML haritası ile bağlanan XML verilerini dışa aktarır. |
| [exportXml(String mapName, String path)](#exportXml-java.lang.String-java.lang.String-) | Belirtilen XML haritası ile bağlanan XML verilerini dışa aktarır. |
| [getAbsolutePath()](#getAbsolutePath--) | Dosyanın mutlak yolunu alır. |
| [getBuiltInDocumentProperties()](#getBuiltInDocumentProperties--) | Bir [DocumentProperty](../../com.aspose.cells/documentproperty) koleksiyonu döndürür; bu koleksiyon elektronik tablonun tüm yerleşik belge özelliklerini temsil eder. |
| [getCellsDataTableFactory()](#getCellsDataTableFactory--) | Özel nesnelerden ICellsDataTable oluşturmak için fabrikayı alır |
| [getClass()](#getClass--) |  |
| [getColors()](#getColors--) | Elektronik tablo için palet içindeki renkleri döndürür. |
| [getContentTypeProperties()](#getContentTypeProperties--) | Çalışma kitabındaki [ContentTypeProperty](../../com.aspose.cells/contenttypeproperty) nesnelerinin listesini alır. |
| [getCountOfStylesInPool()](#getCountOfStylesInPool--) | Stil havuzundaki stil sayısını alır. |
| [getCustomDocumentProperties()](#getCustomDocumentProperties--) | Bir [DocumentProperty](../../com.aspose.cells/documentproperty) koleksiyonu döndürür; bu koleksiyon elektronik tablonun tüm özel belge özelliklerini temsil eder. |
| [getCustomXmlParts()](#getCustomXmlParts--) | Bir Özel XML Veri Depolama Bölümünü temsil eder (paket içindeki özel XML verileri). |
| [getDataConnections()](#getDataConnections--) | [ExternalConnection](../../com.aspose.cells/externalconnection) koleksiyonunu alır. |
| [getDataMashup()](#getDataMashup--) | Karışım verilerini alır. |
| [getDataModel()](#getDataModel--) | Çalışma kitabındaki veri modelini alır. |
| [getDataSorter()](#getDataSorter--) | Verileri sıralamak için bir DataSorter nesnesi alır. |
| [getDefaultStyle()](#getDefaultStyle--) | Çalışma kitabının varsayılan [Style](../../com.aspose.cells/style) nesnesini alır. |
| [getDigitalSignature()](#getDigitalSignature--) | Dosyadan dijital imzayı alır. |
| [getFileFormat()](#getFileFormat--) | Dosya biçimini alır. |
| [getFileName()](#getFileName--) | Geçerli dosya adını alır. |
| [getFonts()](#getFonts--) | Stil havuzundaki tüm yazı tiplerini alır. |
| [getInterruptMonitor()](#getInterruptMonitor--) | Kesinti izleyicisini alır. |
| [getMatchingColor(Color rawColor)](#getMatchingColor-com.aspose.cells.Color-) | Mevcut palet içinde en iyi eşleşen rengi bulur. |
| [getNamedStyle(String name)](#getNamedStyle-java.lang.String-) | Stil havuzundaki adlandırılmış stili alır. |
| [getRibbonXml()](#getRibbonXml--) | Ribbon UI'yi tanımlayan XML dosyasını alır. |
| [getSettings()](#getSettings--) | Çalışma kitabı ayarlarını temsil eder. |
| [getStyleInPool(int index)](#getStyleInPool-int-) | Stil havuzundaki stili alır. |
| [getTheme()](#getTheme--) | Tema adını alır. |
| [getThemeColor(int type)](#getThemeColor-int-) | Tema rengini alır. |
| [getVbaProject()](#getVbaProject--) | Bir elektronik tabloda [getVbaProject()](../../com.aspose.cells/workbook\#getVbaProject--) alır. |
| [getWorksheets()](#getWorksheets--) | Elektronik tabloda [WorksheetCollection](../../com.aspose.cells/worksheetcollection) koleksiyonunu alır. |
| [hasCustomFunction()](#hasCustomFunction--) | Bu çalışma kitabında, hücre formüllerinde veya tanımlı adlarda kullanılan özel işlevlerin olup olmadığını algılar... |
| [hasExernalLinks()](#hasExernalLinks--) | Bu çalışma kitabının diğer veri kaynaklarına dış bağlantılar içerip içermediğini gösterir. |
| [hasMacro()](#hasMacro--) | Bu elektronik tablonun makro/VBA içerip içermediğini gösterir. |
| [hasRevisions()](#hasRevisions--) | Çalışma kitabının izlenen değişiklikleri olup olmadığını alır |
| [hashCode()](#hashCode--) |  |
| [importXml(InputStream stream, String sheetName, int row, int col)](#importXml-java.io.InputStream-java.lang.String-int-int-) | Bir XML veri dosyasını çalışma kitabına içe aktarır/günceller. |
| [importXml(String url, String sheetName, int row, int col)](#importXml-java.lang.String-java.lang.String-int-int-) | Bir XML veri dosyasını çalışma kitabına içe aktarır/günceller. |
| [isColorInPalette(Color color)](#isColorInPalette-com.aspose.cells.Color-) | Bir rengin elektronik tablo paletinde olup olmadığını kontrol eder. |
| [isDigitallySigned()](#isDigitallySigned--) | Bu elektronik tablonun dijital olarak imzalı olup olmadığını gösterir. |
| [isLicensed()](#isLicensed--) | Lisansın ayarlanıp ayarlanmadığını gösterir. |
| [isWorkbookProtectedWithPassword()](#isWorkbookProtectedWithPassword--) | Yapının veya pencerenin şifreyle korunduğunu gösterir. |
| [mergeNamedStyles(Workbook source)](#mergeNamedStyles-com.aspose.cells.Workbook-) | Diğer Excel dosyasından adlandırılmış stilleri birleştirir. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [parseFormulas(boolean ignoreError)](#parseFormulas-boolean-) | Şablon dosyasından yüklendiğinde veya bir hücreye ayarlandığında henüz ayrıştırılmamış tüm formülleri ayrıştırır. |
| [protect(int protectionType, String password)](#protect-int-java.lang.String-) | Bir çalışma kitabını korur. |
| [protectSharedWorkbook(String password)](#protectSharedWorkbook-java.lang.String-) | Paylaşılan bir çalışma kitabını korur. |
| [refreshAll()](#refreshAll--) | Bağlantılı şekilleri, pivot kaynağına sahip tüm pivot tablolarını ve grafiklerini yenileyin. |
| [refreshDynamicArrayFormulas(boolean calculate)](#refreshDynamicArrayFormulas-boolean-) | Dinamik dizi formüllerini (geçerli verilere göre komşu hücrelerde yeni bir aralığa yayılır) yeniler. Çalışma kitabındaki diğer formüller, dinamik dizi formülleri tarafından kullanılsa bile, yinelemeli olarak hesaplanmayacaktır. |
| [refreshDynamicArrayFormulas(boolean calculate, CalculationOptions copts)](#refreshDynamicArrayFormulas-boolean-com.aspose.cells.CalculationOptions-) | Dinamik dizi formüllerini (geçerli verilere göre komşu hücrelerde yeni bir aralığa yayılır) yeniler. |
| [removeDigitalSignature()](#removeDigitalSignature--) | Bu elektronik tablodan dijital imzayı kaldırır. |
| [removeExternalLinks()](#removeExternalLinks--) | Çalışma kitabındaki tüm dış bağlantıları kaldırır. |
| [removeMacro()](#removeMacro--) | Bu elektronik tablodan VBA/makroyu kaldırır. |
| [removePersonalInformation()](#removePersonalInformation--) | Kişisel bilgileri kaldırır. |
| [removeUnusedStyles()](#removeUnusedStyles--) | Kullanılmayan tüm stilleri kaldır. |
| [replace(boolean boolValue, Object newValue)](#replace-boolean-java.lang.Object-) | Hücre değerlerini yeni veriyle değiştirir. |
| [replace(int intValue, Object newValue)](#replace-int-java.lang.Object-) | Hücre değerlerini yeni veriyle değiştirir. |
| [replace(String placeHolder, double newValue)](#replace-java.lang.String-double-) | Bir hücrenin değerini yeni bir double ile değiştirir. |
| [replace(String placeHolder, double[] newValues, boolean isVertical)](#replace-java.lang.String-double---boolean-) | Hücre değerlerini bir double dizisiyle değiştirir. |
| [replace(String placeHolder, int newValue)](#replace-java.lang.String-int-) | Bir hücrenin değerini yeni bir tam sayı ile değiştirir. |
| [replace(String placeHolder, int[] newValues, boolean isVertical)](#replace-java.lang.String-int---boolean-) | Hücre değerlerini bir tam sayı dizisiyle değiştirir. |
| [replace(String placeHolder, String newValue)](#replace-java.lang.String-java.lang.String-) | Bir hücrenin değerini yeni bir dize ile değiştirir. |
| [replace(String placeHolder, String newValue, ReplaceOptions options)](#replace-java.lang.String-java.lang.String-com.aspose.cells.ReplaceOptions-) | Bir hücrenin değerini yeni bir dize ile değiştirir. |
| [replace(String placeHolder, String[] newValues, boolean isVertical)](#replace-java.lang.String-java.lang.String---boolean-) | Bir hücrenin değerini yeni bir dize dizisiyle değiştirir. |
| [save(OutputStream stream, SaveOptions saveOptions)](#save-java.io.OutputStream-com.aspose.cells.SaveOptions-) | Çalışma kitabını akışa kaydet. |
| [save(OutputStream stream, int saveFormat)](#save-java.io.OutputStream-int-) | Çalışma kitabını akışa kaydet. |
| [save(String fileName)](#save-java.lang.String-) | Çalışma kitabını diske kaydet. |
| [save(String fileName, SaveOptions saveOptions)](#save-java.lang.String-com.aspose.cells.SaveOptions-) | Çalışma kitabını diske kaydeder. |
| [save(String fileName, int saveFormat)](#save-java.lang.String-int-) | Çalışma kitabını diske kaydeder. |
| [setAbsolutePath(String value)](#setAbsolutePath-java.lang.String-) | Dosyanın mutlak yolunu ayarlar. |
| [setDefaultStyle(Style value)](#setDefaultStyle-com.aspose.cells.Style-) | Çalışma kitabının varsayılan [Style](../../com.aspose.cells/style) nesnesini ayarlar. |
| [setDigitalSignature(DigitalSignatureCollection digitalSignatureCollection)](#setDigitalSignature-com.aspose.cells.DigitalSignatureCollection-) | Bir elektronik tablo dosyasına (Excel2007 ve sonrası) dijital imza ayarlar. |
| [setEncryptionOptions(int encryptionType, int keyLength)](#setEncryptionOptions-int-int-) | Şifreleme seçeneklerini ayarla. |
| [setFileFormat(int value)](#setFileFormat-int-) | Dosya biçimini ayarlar. |
| [setFileName(String value)](#setFileName-java.lang.String-) | Geçerli dosya adını ayarlar. |
| [setInterruptMonitor(AbstractInterruptMonitor value)](#setInterruptMonitor-com.aspose.cells.AbstractInterruptMonitor-) | Kesinti izleyicisini ayarlar. |
| [setRibbonXml(String value)](#setRibbonXml-java.lang.String-) | Ribbon UI'yi tanımlayan XML dosyasını ayarlar. |
| [setThemeColor(int type, Color color)](#setThemeColor-int-com.aspose.cells.Color-) | Tema rengini ayarlar |
| [startAccessCache(int opts)](#startAccessCache-int-) | Veriye erişmek için önbellekleri kullanan oturumu başlatır. |
| [toString()](#toString--) |  |
| [unprotect(String password)](#unprotect-java.lang.String-) | Bir çalışma kitabının korumasını kaldırır. |
| [unprotectSharedWorkbook(String password)](#unprotectSharedWorkbook-java.lang.String-) | Paylaşılan bir çalışma kitabının korumasını kaldırır. |
| [updateCustomFunctionDefinition(CustomFunctionDefinition definition)](#updateCustomFunctionDefinition-com.aspose.cells.CustomFunctionDefinition-) | Özel işlevlerin tanımını günceller. |
| [updateLinkedDataSource(Workbook[] externalWorkbooks)](#updateLinkedDataSource-com.aspose.cells.Workbook---) | Bu çalışma kitabı başka veri kaynaklarına dış bağlantılar içeriyorsa, Aspose.Cells verilen kaynaklardan en son verileri almaya çalışacaktır. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### Workbook() {#Workbook--}
```
public Workbook()
```


Yeni bir [Workbook](../../com.aspose.cells/workbook) sınıf örneği başlatır.

**Remarks**

Varsayılan dosya formatı Xlsx'tir. Başka dosya türleri oluşturmak istiyorsanız, lütfen Workbook(FileFormatType) kullanın.

**Example**

Aşağıdaki kod, sınıfın yeni bir örneğini oluşturmak ve başlatmak için Workbook yapıcısının nasıl kullanılacağını gösterir.

```
         Workbook workbook = new Workbook();
```

### Workbook(int fileFormatType) {#Workbook-int-}
```
public Workbook(int fileFormatType)
```


Yeni bir [Workbook](../../com.aspose.cells/workbook) sınıf örneği başlatır.

**Remarks**

Varsayılan dosya formatı Excel97To2003'tür.

**Example**

Aşağıdaki kod, farklı dosya formatlarıyla sınıfın yeni bir örneğini oluşturmak ve başlatmak için Workbook yapıcısının nasıl kullanılacağını gösterir.

```
         Workbook workbook = new Workbook(FileFormatType.XLSX);
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fileFormatType | int | [FileFormatType](../../com.aspose.cells/fileformattype). Yeni dosya formatı. |

### Workbook(LoadOptions loadOptions) {#Workbook-com.aspose.cells.LoadOptions-}
```
public Workbook(LoadOptions loadOptions)
```


Seçeneklerle yeni boş bir [Workbook](../../com.aspose.cells/workbook) sınıf örneği başlatır

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| loadOptions | [LoadOptions](../../com.aspose.cells/loadoptions) | Seçenekler. |

### Workbook(String file) {#Workbook-java.lang.String-}
```
public Workbook(String file)
```


Yeni bir [Workbook](../../com.aspose.cells/workbook) sınıf örneği başlatır ve bir dosya açar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dosya | java.lang.String | Dosya adı. |

### Workbook(InputStream stream) {#Workbook-java.io.InputStream-}
```
public Workbook(InputStream stream)
```


Yeni bir [Workbook](../../com.aspose.cells/workbook) sınıf örneği başlatır ve bir akış açar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stream | java.io.InputStream | Akış. |

### Workbook(String file, LoadOptions loadOptions) {#Workbook-java.lang.String-com.aspose.cells.LoadOptions-}
```
public Workbook(String file, LoadOptions loadOptions)
```


Yeni bir [Workbook](../../com.aspose.cells/workbook) sınıf örneği başlatır ve bir dosya açar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dosya | java.lang.String | Dosya adı. |
| loadOptions | [LoadOptions](../../com.aspose.cells/loadoptions) | Yükleme seçenekleri |

### Workbook(InputStream stream, LoadOptions loadOptions) {#Workbook-java.io.InputStream-com.aspose.cells.LoadOptions-}
```
public Workbook(InputStream stream, LoadOptions loadOptions)
```


Yeni bir [Workbook](../../com.aspose.cells/workbook) sınıf örneği başlatır ve akışı açar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stream | java.io.InputStream | Akış. |
| loadOptions | [LoadOptions](../../com.aspose.cells/loadoptions) | Yükleme seçenekleri |

### acceptAllRevisions() {#acceptAllRevisions--}
```
public void acceptAllRevisions()
```


Çalışma kitabındaki tüm izlenen değişiklikleri kabul eder.

### addDigitalSignature(DigitalSignatureCollection digitalSignatureCollection) {#addDigitalSignature-com.aspose.cells.DigitalSignatureCollection-}
```
public void addDigitalSignature(DigitalSignatureCollection digitalSignatureCollection)
```


OOXML elektronik tablo dosyasına (Excel2007 ve sonrası) dijital imza ekler.

**Remarks**

Yalnızca OOXML elektronik tablo dosyasına Xmldsig Dijital İmza eklemeyi destekler

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| digitalSignatureCollection | [DigitalSignatureCollection](../../com.aspose.cells/digitalsignaturecollection) |  |

### calculateFormula() {#calculateFormula--}
```
public void calculateFormula()
```


Formüllerin sonucunu hesaplar.

**Remarks**

Desteklenen tüm formüller için lütfen https://docs.aspose.com/display/cellsnet/Supported+Formula+Functions adresindeki listeye bakın.

### calculateFormula(boolean ignoreError) {#calculateFormula-boolean-}
```
public void calculateFormula(boolean ignoreError)
```


Formüllerin sonucunu hesaplar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ignoreError | boolean | Formüllerin hesaplanmasında hatanın gizlenip gizlenmeyeceğini belirtir. Hata, desteklenmeyen işlev, dış bağlantılar vb. olabilir. |

### calculateFormula(CalculationOptions options) {#calculateFormula-com.aspose.cells.CalculationOptions-}
```
public void calculateFormula(CalculationOptions options)
```


Bu çalışma kitabındaki formüller hesaplanıyor.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| options | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Hesaplama seçenekleri |

### changePalette(Color color, int index) {#changePalette-com.aspose.cells.Color-int-}
```
public void changePalette(Color color, int index)
```


Belirtilen indeksteki elektronik tablo için paleti değiştirir.

**Remarks**

Palet, her biri bir RGB değeriyle temsil edilen 56 girişe sahiptir.

Palet içinde olmayan bir renk ayarlarsanız, etkili olmayacaktır.

Bu nedenle özel bir renk ayarlamak istiyorsanız, önce paleti değiştirin.

Aşağıdaki standart renk paletidir.

| Color | Kırmızı | Yeşil | Mavi |
| ------- | --- | ----- | ---- |
| Siyah | 0 | 0 | 0 |
| Beyaz | 255 | 255 | 255 |
| Kırmızı | 255 | 0 | 0 |
| Limon | 0 | 255 | 0 |
| Mavi | 0 | 0 | 255 |
| Sarı | 255 | 255 | 0 |
| Macenta | 255 | 0 | 255 |
| Camgöbeği | 0 | 255 | 255 |
| Kestane | 128 | 0 | 0 |
| Yeşil | 0 | 128 | 0 |
| Lacivert | 0 | 0 | 128 |
| Zeytin | 128 | 128 | 0 |
| Mor | 128 | 0 | 128 |
| Turkuaz | 0 | 128 | 128 |
| Gümüş | 192 | 192 | 192 |
| Gri | 128 | 128 | 128 |
| Color17 | 153 | 153 | 255 |
| Color18 | 153 | 51 | 102 |
| Color19 | 255 | 255 | 204 |
| Color20 | 204 | 255 | 255 |
| Color21 | 102 | 0 | 102 |
| Renk22 | 255 | 128 | 128 |
| Renk23 | 0 | 102 | 204 |
| Renk24 | 204 | 204 | 255 |
| Renk25 | 0 | 0 | 128 |
| Renk26 | 255 | 0 | 255 |
| Renk27 | 255 | 255 | 0 |
| Renk28 | 0 | 255 | 255 |
| Renk29 | 128 | 0 | 128 |
| Renk30 | 128 | 0 | 0 |
| Renk31 | 0 | 128 | 128 |
| Renk32 | 0 | 0 | 255 |
| Renk33 | 0 | 204 | 255 |
| Renk34 | 204 | 255 | 255 |
| Renk35 | 204 | 255 | 204 |
| Renk36 | 255 | 255 | 153 |
| Renk37 | 153 | 204 | 255 |
| Renk38 | 255 | 153 | 204 |
| Renk39 | 204 | 153 | 255 |
| Renk40 | 255 | 204 | 153 |
| Renk41 | 51 | 102 | 255 |
| Renk42 | 51 | 204 | 204 |
| Renk43 | 153 | 204 | 0 |
| Renk44 | 255 | 204 | 0 |
| Renk45 | 255 | 153 | 0 |
| Renk46 | 255 | 102 | 0 |
| Color47 | 102 | 102 | 153 |
| Color48 | 150 | 150 | 150 |
| Color49 | 0 | 51 | 102 |
| Color50 | 51 | 153 | 102 |
| Color51 | 0 | 51 | 0 |
| Color52 | 51 | 51 | 0 |
| Color53 | 153 | 51 | 0 |
| Color54 | 153 | 51 | 102 |
| Color55 | 51 | 51 | 153 |
| Color56 | 51 | 51 | 51 |

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| color | [Color](../../com.aspose.cells/color) | Renk yapısı. |
| dizin | int | Palet indeksi, 0 - 55. |

### closeAccessCache(int opts) {#closeAccessCache-int-}
```
public void closeAccessCache(int opts)
```


Veriye erişmek için önbellek kullanan oturumu kapatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| opts | int | [AccessCacheOptions](../../com.aspose.cells/accesscacheoptions). veri erişim seçenekleri |

### combine(Workbook secondWorkbook) {#combine-com.aspose.cells.Workbook-}
```
public void combine(Workbook secondWorkbook)
```


Başka bir Workbook nesnesiyle birleştirir.

**Remarks**

Excel, ODS, CSV ve diğer dosyaları tek bir dosyada birleştirin.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| secondWorkbook | [Workbook](../../com.aspose.cells/workbook) | Başka bir Workbook nesnesi. |

### copy(Workbook source) {#copy-com.aspose.cells.Workbook-}
```
public void copy(Workbook source)
```


Kaynak bir Workbook nesnesinden verileri kopyalar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| source | [Workbook](../../com.aspose.cells/workbook) | Kaynak Workbook nesnesi. |

### copy(Workbook source, CopyOptions copyOptions) {#copy-com.aspose.cells.Workbook-com.aspose.cells.CopyOptions-}
```
public void copy(Workbook source, CopyOptions copyOptions)
```


Başka bir Workbook nesnesini kopyalar.

**Remarks**

Excel dosyasını klonlamak çok basittir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| source | [Workbook](../../com.aspose.cells/workbook) | Kaynak Workbook nesnesi. |
| copyOptions | [CopyOptions](../../com.aspose.cells/copyoptions) | Diğer Workbook kopyalama seçenekleri. |

### copyTheme(Workbook source) {#copyTheme-com.aspose.cells.Workbook-}
```
public void copyTheme(Workbook source)
```


Başka bir çalışma kitabından temayı kopyalar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| source | [Workbook](../../com.aspose.cells/workbook) | Kaynak workbook. |

### createBuiltinStyle(int type) {#createBuiltinStyle-int-}
```
public Style createBuiltinStyle(int type)
```


Verilen tipe göre yerleşik stil oluşturur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | int | [BuiltinStyleType](../../com.aspose.cells/builtinstyletype). Yerleşik stil türü. |

**Returns:**
[Style](../../com.aspose.cells/style) - [Style](../../com.aspose.cells/style) object
### createCellsColor() {#createCellsColor--}
```
public CellsColor createCellsColor()
```


Bir [CellsColor](../../com.aspose.cells/cellscolor) nesnesi oluşturur.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor) - Returns a [CellsColor](../../com.aspose.cells/cellscolor) object.
### createStyle() {#createStyle--}
```
public Style createStyle()
```


Yeni bir stil oluşturur.

**Returns:**
[Style](../../com.aspose.cells/style) - Returns a style object.
### createStyle(boolean cloneDefaultStyle) {#createStyle-boolean-}
```
public Style createStyle(boolean cloneDefaultStyle)
```


Yeni bir stil oluşturur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cloneDefaultStyle | boolean | Varsayılan stilin kopyalanıp kopyalanmadığını gösterir |

**Returns:**
[Style](../../com.aspose.cells/style) - Returns a style object.
### customTheme(String themeName, Color[] colors) {#customTheme-java.lang.String-com.aspose.cells.Color---}
```
public void customTheme(String themeName, Color[] colors)
```


Temayı özelleştirir.

**Remarks**

Renklerin uzunluğu 12 olmalıdır.

| Dizi indeksi | Tema türü |
| ----------- | ------------------ |
| 0 | Backgournd1 |
| 1 | Text1 |
| 2 | Backgournd2 |
| 3 | Text2 |
| 4 | Accent1 |
| 5 | Accent2 |
| 6 | Accent3 |
| 7 | Accent4 |
| 8 | Accent5 |
| 9 | Accent6 |
| 10 | Köprü |
| 11 | Takip edilen Köprü |

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| themeName | java.lang.String | Tema adı |
| colors | [Color\[\]](../../com.aspose.cells/color) | Tema renkleri |

### dispose() {#dispose--}
```
public void dispose()
```


Yönetilmeyen kaynakların serbest bırakılması, salınması veya sıfırlanmasıyla ilgili uygulama tanımlı görevleri yürütür.

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
### exportXml(String mapName, OutputStream stream) {#exportXml-java.lang.String-java.io.OutputStream-}
```
public void exportXml(String mapName, OutputStream stream)
```


Belirtilen XML haritası ile bağlanan XML verilerini dışa aktarır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| mapName | java.lang.String | dışa aktarılması gereken XML haritasının adı |
| stream | java.io.OutputStream | dışa aktarma akışı |

### exportXml(String mapName, String path) {#exportXml-java.lang.String-java.lang.String-}
```
public void exportXml(String mapName, String path)
```


Belirtilen XML haritası ile bağlanan XML verilerini dışa aktarır.

**Example**

Aşağıdaki kod, ilk XmlMap tarafından bağlanan verileri dışa aktardı.

```
         Workbook wb = new Workbook("Book1.xlsx");
 
         //Make sure that the source xlsx file contains a XmlMap.
         XmlMap xmlMap = wb.getWorksheets().getXmlMaps().get(0);
 
         wb.exportXml(xmlMap.getName(), "output.xml");
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| mapName | java.lang.String | dışa aktarılması gereken XML haritasının adı |
| yol | java.lang.String | dışa aktarma yolu |

### getAbsolutePath() {#getAbsolutePath--}
```
public String getAbsolutePath()
```


Dosyanın mutlak yolunu alır.

**Remarks**

Yalnızca dış bağlantılar için kullanılır.

**Returns:**
java.lang.String
### getBuiltInDocumentProperties() {#getBuiltInDocumentProperties--}
```
public BuiltInDocumentPropertyCollection getBuiltInDocumentProperties()
```


Bir [DocumentProperty](../../com.aspose.cells/documentproperty) koleksiyonu döndürür; bu koleksiyon elektronik tablonun tüm yerleşik belge özelliklerini temsil eder.

**Remarks**

Yerleşik belge özellikleri listesine yeni bir özellik eklenemez. Yalnızca bir yerleşik özelliği alabilir ve değerini değiştirebilirsiniz. Aşağıda yerleşik özelliklerin ad listesi verilmiştir:

Title

Konu

Yazar

Anahtar Kelimeler

Yorumlar

Şablon

Son Yazar

Revizyon Numarası

Uygulama Adı

Son Yazdırma Tarihi

Oluşturma Tarihi

Son Kaydetme Zamanı

Toplam Düzenleme Süresi

Sayfa Sayısı

Kelime Sayısı

Karakter Sayısı

Güvenlik

Kategori

Biçim

Yönetici

Şirket

Bayt Sayısı

Satır Sayısı

Paragraf Sayısı

Slayt Sayısı

Not Sayısı

Gizli Slayt Sayısı

Multimedya Klip Sayısı

**Example**

```
         Workbook workbook = new Workbook();
         DocumentProperty doc = workbook.getBuiltInDocumentProperties().get("Author");
         doc.setValue("John Smith");
```

**Returns:**
[BuiltInDocumentPropertyCollection](../../com.aspose.cells/builtindocumentpropertycollection)
### getCellsDataTableFactory() {#getCellsDataTableFactory--}
```
public CellsDataTableFactory getCellsDataTableFactory()
```


Özel nesnelerden ICellsDataTable oluşturmak için fabrikayı alır

**Returns:**
[CellsDataTableFactory](../../com.aspose.cells/cellsdatatablefactory)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColors() {#getColors--}
```
public Color[] getColors()
```


Elektronik tablo için palet içindeki renkleri döndürür.

**Remarks**

Palet, her biri bir RGB değeriyle temsil edilen 56 girişe sahiptir.

**Returns:**
com.aspose.cells.Color[]
### getContentTypeProperties() {#getContentTypeProperties--}
```
public ContentTypePropertyCollection getContentTypeProperties()
```


Çalışma kitabındaki [ContentTypeProperty](../../com.aspose.cells/contenttypeproperty) nesnelerinin listesini alır.

**Returns:**
[ContentTypePropertyCollection](../../com.aspose.cells/contenttypepropertycollection)
### getCountOfStylesInPool() {#getCountOfStylesInPool--}
```
public int getCountOfStylesInPool()
```


Stil havuzundaki stil sayısını alır.

**Returns:**
int
### getCustomDocumentProperties() {#getCustomDocumentProperties--}
```
public CustomDocumentPropertyCollection getCustomDocumentProperties()
```


Bir [DocumentProperty](../../com.aspose.cells/documentproperty) koleksiyonu döndürür; bu koleksiyon elektronik tablonun tüm özel belge özelliklerini temsil eder.

**Example**

```
         Workbook excel = new Workbook();
         excel.getCustomDocumentProperties().add("Checked by", "Jane");
```

**Returns:**
[CustomDocumentPropertyCollection](../../com.aspose.cells/customdocumentpropertycollection)
### getCustomXmlParts() {#getCustomXmlParts--}
```
public CustomXmlPartCollection getCustomXmlParts()
```


Bir Özel XML Veri Depolama Bölümünü temsil eder (paket içindeki özel XML verileri).

**Returns:**
[CustomXmlPartCollection](../../com.aspose.cells/customxmlpartcollection)
### getDataConnections() {#getDataConnections--}
```
public ExternalConnectionCollection getDataConnections()
```


[ExternalConnection](../../com.aspose.cells/externalconnection) koleksiyonunu alır.

**Returns:**
[ExternalConnectionCollection](../../com.aspose.cells/externalconnectioncollection)
### getDataMashup() {#getDataMashup--}
```
public DataMashup getDataMashup()
```


Karışım verilerini alır.

**Returns:**
[DataMashup](../../com.aspose.cells/datamashup)
### getDataModel() {#getDataModel--}
```
public DataModel getDataModel()
```


Çalışma kitabındaki veri modelini alır.

**Returns:**
[DataModel](../../com.aspose.cells/datamodel)
### getDataSorter() {#getDataSorter--}
```
public DataSorter getDataSorter()
```


Verileri sıralamak için bir DataSorter nesnesi alır.

**Returns:**
[DataSorter](../../com.aspose.cells/datasorter)
### getDefaultStyle() {#getDefaultStyle--}
```
public Style getDefaultStyle()
```


Çalışma kitabının varsayılan [Style](../../com.aspose.cells/style) nesnesini alır.

**Remarks**

DefaultStyle özelliği, tüm Workbook için bir Style uygulamak için yararlıdır.

**Example**

Aşağıdaki kod yeni bir Workbook oluşturur ve örnekler ve ona varsayılan bir [Style](../../com.aspose.cells/style) atar.

```
         Workbook workbook = new Workbook();
         Style defaultStyle = workbook.getDefaultStyle();
         defaultStyle.getFont().setName("Tahoma");
         workbook.setDefaultStyle(defaultStyle);
```

**Returns:**
[Style](../../com.aspose.cells/style)
### getDigitalSignature() {#getDigitalSignature--}
```
public DigitalSignatureCollection getDigitalSignature()
```


Dosyadan dijital imzayı alır.

**Returns:**
[DigitalSignatureCollection](../../com.aspose.cells/digitalsignaturecollection)
### getFileFormat() {#getFileFormat--}
```
public int getFileFormat()
```


Dosya biçimini alır.

Bakınız [FileFormatType](../../com.aspose.cells/fileformattype).

**Returns:**
int
### getFileName() {#getFileName--}
```
public String getFileName()
```


Geçerli dosya adını alır.

**Remarks**

Dosya akışla açıldıysa ve bazı dış formül referansları varsa, lütfen dosya adını ayarlayın.

**Returns:**
java.lang.String
### getFonts() {#getFonts--}
```
public Font[] getFonts()
```


Stil havuzundaki tüm yazı tiplerini alır.

**Returns:**
com.aspose.cells.Font[]
### getInterruptMonitor() {#getInterruptMonitor--}
```
public AbstractInterruptMonitor getInterruptMonitor()
```


Kesinti izleyicisini alır.

**Returns:**
[AbstractInterruptMonitor](../../com.aspose.cells/abstractinterruptmonitor)
### getMatchingColor(Color rawColor) {#getMatchingColor-com.aspose.cells.Color-}
```
public Color getMatchingColor(Color rawColor)
```


Mevcut palet içinde en iyi eşleşen rengi bulur.

**Remarks**

Excel 97-2003'te renk paletinde yalnızca 56 renk vardır. Renk paletinde yoksa, benzer bir renk ayarlanacaktır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rawColor | [Color](../../com.aspose.cells/color) | Ham renk. |

**Returns:**
[Color](../../com.aspose.cells/color) - Best matching color.
### getNamedStyle(String name) {#getNamedStyle-java.lang.String-}
```
public Style getNamedStyle(String name)
```


Stil havuzundaki adlandırılmış stili alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String | stilin adı |

**Returns:**
[Style](../../com.aspose.cells/style) - named style, maybe null.
### getRibbonXml() {#getRibbonXml--}
```
public String getRibbonXml()
```


Ribbon UI'yi tanımlayan XML dosyasını alır.

**Returns:**
java.lang.String
### getSettings() {#getSettings--}
```
public WorkbookSettings getSettings()
```


Çalışma kitabı ayarlarını temsil eder.

**Returns:**
[WorkbookSettings](../../com.aspose.cells/workbooksettings)
### getStyleInPool(int index) {#getStyleInPool-int-}
```
public Style getStyleInPool(int index)
```


Stil havuzundaki stili alır. Çalışma kitabındaki tüm stiller bir havuza toplanır. Hücrelerde yalnızca basit bir referans indeksi bulunur.

**Remarks**

Döndürülen stil değiştirilirse, bu stile referans veren tüm hücrelerin stili değişecektir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | İndeks. |

**Returns:**
[Style](../../com.aspose.cells/style) - The style in the pool corresponds to given index, may be null.
### getTheme() {#getTheme--}
```
public String getTheme()
```


Tema adını alır.

**Returns:**
java.lang.String
### getThemeColor(int type) {#getThemeColor-int-}
```
public Color getThemeColor(int type)
```


Tema rengini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | int | [ThemeColorType](../../com.aspose.cells/themecolortype). Tema renk türü. |

**Returns:**
[Color](../../com.aspose.cells/color) - The theme color.
### getVbaProject() {#getVbaProject--}
```
public VbaProject getVbaProject()
```


Bir elektronik tabloda [getVbaProject()](../../com.aspose.cells/workbook\#getVbaProject--) alır.

**Returns:**
[VbaProject](../../com.aspose.cells/vbaproject)
### getWorksheets() {#getWorksheets--}
```
public WorksheetCollection getWorksheets()
```


Elektronik tabloda [WorksheetCollection](../../com.aspose.cells/worksheetcollection) koleksiyonunu alır.

**Returns:**
[WorksheetCollection](../../com.aspose.cells/worksheetcollection) - [WorksheetCollection](../../com.aspose.cells/worksheetcollection) collection
### hasCustomFunction() {#hasCustomFunction--}
```
public boolean hasCustomFunction()
```


Bu çalışma kitabında, hücre formüllerinde veya tanımlı adlarda kullanılan özel işlevlerin olup olmadığını algılar...

**Returns:**
boolean
### hasExernalLinks() {#hasExernalLinks--}
```
public boolean hasExernalLinks()
```


Bu çalışma kitabının diğer veri kaynaklarına dış bağlantılar içerip içermediğini gösterir.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine, bu çalışma kitabında dış bağlantıların olup olmadığını kontrol etmek için ExternalLinkCollection.Count kullanın. Bu yöntem, Aralık 2021'den itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
boolean - Bu çalışma kitabının diğer veri kaynaklarına dış bağlantılar içerip içermediği.
### hasMacro() {#hasMacro--}
```
public boolean hasMacro()
```


Bu elektronik tablonun makro/VBA içerip içermediğini gösterir.

**Returns:**
boolean
### hasRevisions() {#hasRevisions--}
```
public boolean hasRevisions()
```


Çalışma kitabının izlenen değişiklikleri olup olmadığını alır

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### importXml(InputStream stream, String sheetName, int row, int col) {#importXml-java.io.InputStream-java.lang.String-int-int-}
```
public void importXml(InputStream stream, String sheetName, int row, int col)
```


Bir XML veri dosyasını çalışma kitabına içe aktarır/günceller.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stream | java.io.InputStream | xml dosya akışı. |
| sheetName | java.lang.String | hedef sayfa adı. |
| satır | int | hedef satır. |
| col | int | hedef sütun. |

### importXml(String url, String sheetName, int row, int col) {#importXml-java.lang.String-java.lang.String-int-int-}
```
public void importXml(String url, String sheetName, int row, int col)
```


Bir XML veri dosyasını çalışma kitabına içe aktarır/günceller.

**Example**

Aşağıdaki kod, XML verilerini 'Sheet 1' çalışma sayfasına A1 hücresine aktarır.

```
         Workbook wb = new Workbook("Book1.xlsx");
 
         wb.importXml("xml.xml", "Sheet1", 0, 0);
 
         wb.save("output.xlsx");
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| url | java.lang.String | xml dosyasının url/yolu. |
| sheetName | java.lang.String | hedef sayfa adı. |
| satır | int | hedef satır |
| col | int | hedef sütun |

### isColorInPalette(Color color) {#isColorInPalette-com.aspose.cells.Color-}
```
public boolean isColorInPalette(Color color)
```


Bir rengin elektronik tablo paletinde olup olmadığını kontrol eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| color | [Color](../../com.aspose.cells/color) | Renk yapısı. |

**Returns:**
boolean - Palet içinde bu renk varsa true döndürür. Aksi takdirde false döndürür.
### isDigitallySigned() {#isDigitallySigned--}
```
public boolean isDigitallySigned()
```


Bu elektronik tablonun dijital olarak imzalı olup olmadığını gösterir.

**Returns:**
boolean
### isLicensed() {#isLicensed--}
```
public boolean isLicensed()
```


Lisansın ayarlanıp ayarlanmadığını gösterir.

**Returns:**
boolean
### isWorkbookProtectedWithPassword() {#isWorkbookProtectedWithPassword--}
```
public boolean isWorkbookProtectedWithPassword()
```


Yapının veya pencerenin şifreyle korunduğunu gösterir.

**Returns:**
boolean
### mergeNamedStyles(Workbook source) {#mergeNamedStyles-com.aspose.cells.Workbook-}
```
public void mergeNamedStyles(Workbook source)
```


Diğer Excel dosyasından adlandırılmış stilleri birleştirir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| source | [Workbook](../../com.aspose.cells/workbook) | Diğer dosya |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### parseFormulas(boolean ignoreError) {#parseFormulas-boolean-}
```
public void parseFormulas(boolean ignoreError)
```


Şablon dosyasından yüklendiğinde veya bir hücreye ayarlandığında henüz ayrıştırılmamış tüm formülleri ayrıştırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ignoreError | boolean | Geçersiz formül için hatanın göz ardı edilip edilmeyeceği. Bir geçersiz formül için, hata göz ardı edilirse bu formül atlanır ve süreç diğer formülleri ayrıştırmaya devam eder, aksi takdirde istisna fırlatılır. |

### protect(int protectionType, String password) {#protect-int-java.lang.String-}
```
public void protect(int protectionType, String password)
```


Bir çalışma kitabını korur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| protectionType | int | [ProtectionType](../../com.aspose.cells/protectiontype). Koruma türü. |
| password | java.lang.String | Çalışma kitabını korumak için şifre. |

### protectSharedWorkbook(String password) {#protectSharedWorkbook-java.lang.String-}
```
public void protectSharedWorkbook(String password)
```


Paylaşılan bir çalışma kitabını korur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| password | java.lang.String | Çalışma kitabını korumak için şifre. |

### refreshAll() {#refreshAll--}
```
public void refreshAll()
```


Bağlantılı şekilleri, pivot kaynağına sahip tüm pivot tablolarını ve grafiklerini yenileyin.

### refreshDynamicArrayFormulas(boolean calculate) {#refreshDynamicArrayFormulas-boolean-}
```
public void refreshDynamicArrayFormulas(boolean calculate)
```


Dinamik dizi formüllerini (geçerli verilere göre komşu hücrelerde yeni bir aralığa yayılır) yeniler. Çalışma kitabındaki diğer formüller, dinamik dizi formülleri tarafından kullanılsa bile, yinelemeli olarak hesaplanmayacaktır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| hesapla | boolean | Dinamik dizi formülleri için hücre değerlerini hesaplayıp güncelleyip güncellemeyeceği |

### refreshDynamicArrayFormulas(boolean calculate, CalculationOptions copts) {#refreshDynamicArrayFormulas-boolean-com.aspose.cells.CalculationOptions-}
```
public void refreshDynamicArrayFormulas(boolean calculate, CalculationOptions copts)
```


Dinamik dizi formüllerini (geçerli verilere göre komşu hücrelerde yeni bir aralığa yayılır) yeniler.

**Remarks**

Performans açısından, formül kendisi veya başvurduğu veri değiştiğinde tüm dinamik dizi formüllerini otomatik olarak yenilemeyiz. Bu nedenle kullanıcı, hücre değerlerini içe aktarma/ayarlama, satır/sütun/aralık ekleme/silme gibi dinamik dizi formüllerini etkileyebilecek işlemlerden sonra bu yöntemi manuel olarak çağırmalıdır, ...etc.

Fonksiyon içeren çoğu formül için, taşma aralığını hesaplamak da formülün hesaplanmasını gerektirir, bu yüzden genellikle \"calculate\" bayrağı için true değeri tercih edilir. Formül basit bir aralık referansı veya dizi ise (örneğin \"=C1:E5\", \"=\\{1,2;3,4\\}\", ...), bir aralık veya dizi üzerindeki basit bir fonksiyon ise (örneğin \"=ABS(C1:E5)\", \"=1+\\{1,2;3,4\\}\", ...), ve tüm formüller daha sonra (örneğin [calculateFormula(CalculationOptions)](../../com.aspose.cells/workbook\#calculateFormula-CalculationOptions-)) tarafından hesaplanacaksa, \"calculate\" bayrağı için false değeri kullanmak, performans açısından faydalı olacak şekilde yinelenen hesaplamayı önleyebilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| hesapla | boolean | Dinamik dizi formülleri için hücre değerlerini hesaplayıp güncelleyip güncellemeyeceği |
| copts | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Formülleri hesaplamak için seçenekler |

### removeDigitalSignature() {#removeDigitalSignature--}
```
public void removeDigitalSignature()
```


Bu elektronik tablodan dijital imzayı kaldırır.

### removeExternalLinks() {#removeExternalLinks--}
```
public void removeExternalLinks()
```


Çalışma kitabındaki tüm dış bağlantıları kaldırır.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine lütfen ExternalLinkCollection.Clear() metodunu kullanın. Bu metod, Aralık 2021'den itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### removeMacro() {#removeMacro--}
```
public void removeMacro()
```


Bu elektronik tablodan VBA/makroyu kaldırır.

### removePersonalInformation() {#removePersonalInformation--}
```
public void removePersonalInformation()
```


Kişisel bilgileri kaldırır.

### removeUnusedStyles() {#removeUnusedStyles--}
```
public void removeUnusedStyles()
```


Kullanılmayan tüm stilleri kaldır.

### replace(boolean boolValue, Object newValue) {#replace-boolean-java.lang.Object-}
```
public int replace(boolean boolValue, Object newValue)
```


Hücre değerlerini yeni veriyle değiştirir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| boolValue | boolean | Değiştirilecek boolean değer. |
| newValue | java.lang.Object | Yeni değer. String, integer, double veya DateTime değeri olabilir. |

**Returns:**
int
### replace(int intValue, Object newValue) {#replace-int-java.lang.Object-}
```
public int replace(int intValue, Object newValue)
```


Hücre değerlerini yeni veriyle değiştirir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| intValue | int | Değiştirilecek tam sayı değeri. |
| newValue | java.lang.Object | Yeni değer. String, integer, double veya DateTime değeri olabilir. |

**Returns:**
int
### replace(String placeHolder, double newValue) {#replace-java.lang.String-double-}
```
public int replace(String placeHolder, double newValue)
```


Bir hücrenin değerini yeni bir double ile değiştirir.

**Example**

```
         Workbook workbook = new Workbook();
         //......
         double newValue = 100.0;
         workbook.replace("AnOldValue", newValue);
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| placeHolder | java.lang.String | Hücre yer tutucu |
| newValue | double | Değiştirilecek double değer |

**Returns:**
int
### replace(String placeHolder, double[] newValues, boolean isVertical) {#replace-java.lang.String-double---boolean-}
```
public int replace(String placeHolder, double[] newValues, boolean isVertical)
```


Hücre değerlerini bir double dizisiyle değiştirir.

**Example**

```
         Workbook workbook = new Workbook();
         //......
         double[] newValues = new double[]{1.23, 2.56, 3.14159};
         workbook.replace("AnOldValue", newValues, true);
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| placeHolder | java.lang.String | Hücre yer tutucu |
| newValues | double[] | Değiştirilecek Double dizisi |
| isVertical | boolean | Doğru - Dikey, Yanlış - Yatay |

**Returns:**
int
### replace(String placeHolder, int newValue) {#replace-java.lang.String-int-}
```
public int replace(String placeHolder, int newValue)
```


Bir hücrenin değerini yeni bir tam sayı ile değiştirir.

**Example**

```
         Workbook workbook = new Workbook();
         //......
         int newValue = 100;
         workbook.replace("AnOldValue", newValue);
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| placeHolder | java.lang.String | Hücre yer tutucu |
| newValue | int | Değiştirilecek tam sayı değeri |

**Returns:**
int
### replace(String placeHolder, int[] newValues, boolean isVertical) {#replace-java.lang.String-int---boolean-}
```
public int replace(String placeHolder, int[] newValues, boolean isVertical)
```


Hücre değerlerini bir tam sayı dizisiyle değiştirir.

**Example**

```
         Workbook workbook = new Workbook();
         //......
         int[] newValues = new int[]{1, 2, 3};
         workbook.replace("AnOldValue", newValues, true);
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| placeHolder | java.lang.String | Hücre yer tutucu |
| newValues | int[] | Değiştirilecek tam sayı dizisi |
| isVertical | boolean | Doğru - Dikey, Yanlış - Yatay |

**Returns:**
int
### replace(String placeHolder, String newValue) {#replace-java.lang.String-java.lang.String-}
```
public int replace(String placeHolder, String newValue)
```


Bir hücrenin değerini yeni bir dize ile değiştirir.

**Example**

```
         Workbook workbook = new Workbook();
         //......
         workbook.replace("AnOldValue", "NewValue");
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| placeHolder | java.lang.String | Hücre yer tutucu |
| newValue | java.lang.String | Değiştirilecek metin değeri |

**Returns:**
int
### replace(String placeHolder, String newValue, ReplaceOptions options) {#replace-java.lang.String-java.lang.String-com.aspose.cells.ReplaceOptions-}
```
public int replace(String placeHolder, String newValue, ReplaceOptions options)
```


Bir hücrenin değerini yeni bir dize ile değiştirir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| placeHolder | java.lang.String | Hücre yer tutucu |
| newValue | java.lang.String | Değiştirilecek metin değeri |
| options | [ReplaceOptions](../../com.aspose.cells/replaceoptions) | Değiştirme seçenekleri |

**Returns:**
int
### replace(String placeHolder, String[] newValues, boolean isVertical) {#replace-java.lang.String-java.lang.String---boolean-}
```
public int replace(String placeHolder, String[] newValues, boolean isVertical)
```


Bir hücrenin değerini yeni bir dize dizisiyle değiştirir.

**Example**

```
         Workbook workbook = new Workbook();
         //......
         String[] newValues = new String[]{"Tom", "Alice", "Jerry"};
         workbook.replace("AnOldValue", newValues, true);
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| placeHolder | java.lang.String | Hücre yer tutucu |
| newValues | java.lang.String[] | Değiştirilecek metin dizisi |
| isVertical | boolean | Doğru - Dikey, Yanlış - Yatay |

**Returns:**
int
### save(OutputStream stream, SaveOptions saveOptions) {#save-java.io.OutputStream-com.aspose.cells.SaveOptions-}
```
public void save(OutputStream stream, SaveOptions saveOptions)
```


Çalışma kitabını akışa kaydet.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stream | java.io.OutputStream | Dosya akışı. |
| saveOptions | [SaveOptions](../../com.aspose.cells/saveoptions) | Kaydetme seçenekleri. |

### save(OutputStream stream, int saveFormat) {#save-java.io.OutputStream-int-}
```
public void save(OutputStream stream, int saveFormat)
```


Çalışma kitabını akışa kaydet.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stream | java.io.OutputStream | Dosya akışı. |
| saveFormat | int | [SaveFormat](../../com.aspose.cells/saveformat). Kaydetme dosya formatı türü. |

### save(String fileName) {#save-java.lang.String-}
```
public void save(String fileName)
```


Çalışma kitabını diske kaydet.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fileName | java.lang.String |  |

### save(String fileName, SaveOptions saveOptions) {#save-java.lang.String-com.aspose.cells.SaveOptions-}
```
public void save(String fileName, SaveOptions saveOptions)
```


Çalışma kitabını diske kaydeder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fileName | java.lang.String | Dosya adı. |
| saveOptions | [SaveOptions](../../com.aspose.cells/saveoptions) | Kaydetme seçenekleri. |

### save(String fileName, int saveFormat) {#save-java.lang.String-int-}
```
public void save(String fileName, int saveFormat)
```


Çalışma kitabını diske kaydeder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fileName | java.lang.String | Dosya adı. |
| saveFormat | int | [SaveFormat](../../com.aspose.cells/saveformat). Kaydetme formatı türü. |

### setAbsolutePath(String value) {#setAbsolutePath-java.lang.String-}
```
public void setAbsolutePath(String value)
```


Dosyanın mutlak yolunu ayarlar.

**Remarks**

Yalnızca dış bağlantılar için kullanılır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setDefaultStyle(Style value) {#setDefaultStyle-com.aspose.cells.Style-}
```
public void setDefaultStyle(Style value)
```


Çalışma kitabının varsayılan [Style](../../com.aspose.cells/style) nesnesini ayarlar.

**Remarks**

DefaultStyle özelliği, tüm Workbook için bir Style uygulamak için yararlıdır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [Style](../../com.aspose.cells/style) |  |

### setDigitalSignature(DigitalSignatureCollection digitalSignatureCollection) {#setDigitalSignature-com.aspose.cells.DigitalSignatureCollection-}
```
public void setDigitalSignature(DigitalSignatureCollection digitalSignatureCollection)
```


Bir elektronik tablo dosyasına (Excel2007 ve sonrası) dijital imza ayarlar.

**Remarks**

Yalnızca Xmldsig Dijital İmzası eklemeyi destekler

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| digitalSignatureCollection | [DigitalSignatureCollection](../../com.aspose.cells/digitalsignaturecollection) |  |

### setEncryptionOptions(int encryptionType, int keyLength) {#setEncryptionOptions-int-int-}
```
public void setEncryptionOptions(int encryptionType, int keyLength)
```


Şifreleme seçeneklerini ayarla.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| encryptionType | int | [EncryptionType](../../com.aspose.cells/encryptiontype). Şifreleme türü. |
| keyLength | int | Anahtar uzunluğu. |

### setFileFormat(int value) {#setFileFormat-int-}
```
public void setFileFormat(int value)
```


Dosya biçimini ayarlar.

Bakınız [FileFormatType](../../com.aspose.cells/fileformattype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setFileName(String value) {#setFileName-java.lang.String-}
```
public void setFileName(String value)
```


Geçerli dosya adını ayarlar.

**Remarks**

Dosya akışla açıldıysa ve bazı dış formül referansları varsa, lütfen dosya adını ayarlayın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setInterruptMonitor(AbstractInterruptMonitor value) {#setInterruptMonitor-com.aspose.cells.AbstractInterruptMonitor-}
```
public void setInterruptMonitor(AbstractInterruptMonitor value)
```


Kesinti izleyicisini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [AbstractInterruptMonitor](../../com.aspose.cells/abstractinterruptmonitor) |  |

### setRibbonXml(String value) {#setRibbonXml-java.lang.String-}
```
public void setRibbonXml(String value)
```


Ribbon UI'yi tanımlayan XML dosyasını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setThemeColor(int type, Color color) {#setThemeColor-int-com.aspose.cells.Color-}
```
public void setThemeColor(int type, Color color)
```


Tema rengini ayarlar

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | int | [ThemeColorType](../../com.aspose.cells/themecolortype). Tema renk türü. |
| color | [Color](../../com.aspose.cells/color) | tema rengi |

### startAccessCache(int opts) {#startAccessCache-int-}
```
public void startAccessCache(int opts)
```


Veriye erişmek için önbellekleri kullanan oturumu başlatır.

**Remarks**

Belirtilen veri erişiminin önbelleği, çalışma sayfasındaki bazı veri modellerinin "yalnızca okunabilir" olmasını gerektiriyorsa, bu çalışma kitabındaki her çalışma sayfasındaki ilgili veri modelleri "yalnızca okunabilir" olarak kabul edilir ve kullanıcı bunları değiştirmemelidir.

Veriye erişim tamamlandıktan sonra, tüm önbellekleri temizlemek ve normal erişim modunu geri kazanmak için aynı seçeneklerle [closeAccessCache(int)](../../com.aspose.cells/workbook\#closeAccessCache-int-) çağrılmalıdır.



**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| opts | int | [AccessCacheOptions](../../com.aspose.cells/accesscacheoptions). veri erişim seçenekleri |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### unprotect(String password) {#unprotect-java.lang.String-}
```
public void unprotect(String password)
```


Bir çalışma kitabının korumasını kaldırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| password | java.lang.String | Çalışma kitabının korumasını kaldırmak için şifre. |

### unprotectSharedWorkbook(String password) {#unprotectSharedWorkbook-java.lang.String-}
```
public void unprotectSharedWorkbook(String password)
```


Paylaşılan bir çalışma kitabının korumasını kaldırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| password | java.lang.String | Çalışma kitabının korumasını kaldırmak için şifre. |

### updateCustomFunctionDefinition(CustomFunctionDefinition definition) {#updateCustomFunctionDefinition-com.aspose.cells.CustomFunctionDefinition-}
```
public void updateCustomFunctionDefinition(CustomFunctionDefinition definition)
```


Özel işlevlerin tanımını günceller.

**Remarks**

Bu yöntem bazı özel senaryolarda kullanılabilir. Örneğin, kullanıcı bazı özel işlevlerin bazı parametrelerinin dizi modunda hesaplanmasını istiyorsa, bu işlevler için uygulanmış [CustomFunctionDefinition.getArrayModeParameters(String)](../../com.aspose.cells/customfunctiondefinition\#getArrayModeParameters-String-) içeren kendi tanımını sağlayabilir. Formüllerin verileri güncellendikten sonra, belirtilen parametreler ilgili özel işlevler hesaplanırken dizi modunda otomatik olarak hesaplanacaktır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| definition | [CustomFunctionDefinition](../../com.aspose.cells/customfunctiondefinition) | Kullanıcının özel gereksinimi için özel işlevlerin özel tanımı. |

### updateLinkedDataSource(Workbook[] externalWorkbooks) {#updateLinkedDataSource-com.aspose.cells.Workbook---}
```
public void updateLinkedDataSource(Workbook[] externalWorkbooks)
```


Bu çalışma kitabı başka veri kaynaklarına dış bağlantılar içeriyorsa, Aspose.Cells verilen kaynaklardan en son verileri almaya çalışacaktır.

**Remarks**

Eğer bir çalışma kitabı için ilgili dış bağlantı bulunamazsa, bu çalışma kitabı yok sayılacaktır. Bu nedenle, daha sonra yeni bir dış bağlantı ekleyerek yok sayılan çalışma kitabının ona bağlanmasını istediğinizde, bu bağlantı, bu yöntemi o çalışma kitaplarıyla tekrar çağırana kadar gerçekleştirilemez.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| externalWorkbooks | [Workbook\[\]](../../com.aspose.cells/workbook) | Bu çalışma kitabı tarafından başvurulan dış bağlantıların verilerini güncellemek için kullanılacak çalışma kitapları. Bu çalışma kitapları ile dış bağlantıların eşleşmesi, [getFileName()](../../com.aspose.cells/workbook\#getFileName--) ve [ExternalLink.getDataSource()](../../com.aspose.cells/externallink\#getDataSource--) tarafından belirlenir. Bu nedenle, her bir çalışma kitabı için [getFileName()](../../com.aspose.cells/workbook\#getFileName--) doğru değerle belirtilmiş olduğundan emin olun, böylece ilgili dış bağlantıya bağlanabilirler. |

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

