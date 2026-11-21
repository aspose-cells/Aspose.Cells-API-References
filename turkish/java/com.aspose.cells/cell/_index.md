---
title: "Hücre"
second_title: "Aspose.Cells for Java API Referansı"
description: "Tek bir Çalışma Kitabı hücresini temsil eden nesneyi kapsar."
type: docs
url: /tr/java/com.aspose.cells/cell/
---

**Inheritance:**
java.lang.Object
```
public class Cell
```

Tek bir Çalışma Kitabı hücresini temsil eden nesneyi kapsar.

**Example**

```
         Workbook excel = new Workbook();
         Cells cells = excel.getWorksheets().get(0).getCells();
 
         //Put a string into a cell
         Cell cell = cells.get(0, 0);
         cell.putValue("Hello");
 
         String first = cell.getStringValue();
 
         //Put an integer into a cell
         cell = cells.get("B1");
         cell.putValue(12);
 
         int second = cell.getIntValue();
 
         //Put a double into a cell
         cell = cells.get(0, 2);
         cell.putValue(-1.234);
 
         double third = cell.getDoubleValue();
 
         //Put a formula into a cell
         cell = cells.get("D1");
         cell.setFormula("=B1 + C1");
 
         //Put a combined formula: "sum(average(b1,c1), b1)" to cell at b2
         cell = cells.get("b2");
         cell.setFormula("=sum(average(b1,c1), b1)");
 
         //Set style of a cell
         Style style = cell.getStyle();
         //Set background color
         style.setBackgroundColor(Color.getYellow());
         //Set format of a cell
         style.getFont().setName("Courier New");
         style.setVerticalAlignment(TextAlignmentType.TOP);
          cell.setStyle(style);
```
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [calculate(CalculationOptions options)](#calculate-com.aspose.cells.CalculationOptions-) | Hücrenin formülünü hesaplar. |
| [characters(int startIndex, int length)](#characters-int-int-) | Hücre metni içindeki bir karakter aralığını temsil eden bir Characters nesnesi döndürür. |
| [containsExternalLink()](#containsExternalLink--) | Bu hücrenin harici bir bağlantı içerip içermediğini gösterir. |
| [copy(Cell cell)](#copy-com.aspose.cells.Cell-) | Kaynak hücreden verileri kopyalar. |
| [equals(Cell cell)](#equals-com.aspose.cells.Cell-) | Bu nesnenin başka bir hücre nesnesiyle aynı hücreye referans verip vermediğini kontrol eder. |
| [equals(Object obj)](#equals-java.lang.Object-) | Bu nesnenin başka bir nesneyle aynı hücreye referans verip vermediğini kontrol eder. |
| [getArrayRange()](#getArrayRange--) | Hücrenin formülü bir dizi formülü ise dizi aralığını alır. |
| [getBoolValue()](#getBoolValue--) | Hücrede bulunan boolean değeri alır. |
| [getCharacters()](#getCharacters--) | Hücre metni içindeki bir karakter aralığını temsil eden tüm Characters nesnelerini döndürür. |
| [getCharacters(boolean flag)](#getCharacters-boolean-) | Hücre metni içindeki bir karakter aralığını temsil eden tüm Characters nesnelerini döndürür. |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | Hücrenin sütun numarasını (sıfır tabanlı) alır. |
| [getComment()](#getComment--) | Bu hücrenin yorumunu alır. |
| [getConditionalFormattingResult()](#getConditionalFormattingResult--) | Koşullu biçimlendirme sonucunu al. |
| [getDateTimeValue()](#getDateTimeValue--) | Hücrede bulunan DateTime değerini alır. |
| [getDependents(boolean isAll)](#getDependents-boolean-) | Formülü doğrudan bu hücreye referans veren tüm hücreleri al. |
| [getDependentsInCalculation(boolean recursive)](#getDependentsInCalculation-boolean-) | Hesaplanan sonucu bu hücreye bağlı olan tüm hücreleri alır. |
| [getDisplayStringValue()](#getDisplayStringValue--) | Hücrenin görüntüleme stiliyle biçimlendirilmiş dize değerini alır. |
| [getDisplayStyle()](#getDisplayStyle--) | Bu hücrenin görüntüleme stilini al. |
| [getDisplayStyle(boolean includeMergedBorders)](#getDisplayStyle-boolean-) | Bu hücrenin görüntüleme stilini al. |
| [getDisplayStyle(int adjacentBorders)](#getDisplayStyle-int-) | Bu hücrenin görüntüleme stilini al. |
| [getDoubleValue()](#getDoubleValue--) | Hücrede bulunan double değerini al. |
| [getEmbeddedImage()](#getEmbeddedImage--) | Hücrede gömülü resmi al. |
| [getFloatValue()](#getFloatValue--) | Hücrede bulunan float değerini al. |
| [getFormatConditions()](#getFormatConditions--) | Bu hücreye uygulanan biçim koşullarını al. |
| [getFormula()](#getFormula--) | Bir [Cell](../../com.aspose.cells/cell) formülü al. |
| [getFormula(boolean isR1C1, boolean isLocal)](#getFormula-boolean-boolean-) | Bu hücrenin formülünü al. |
| [getFormulaLocal()](#getFormulaLocal--) | Hücrenin yerel biçimlendirilmiş formülünü al. |
| [getHeightOfValue()](#getHeightOfValue--) | Değerin yüksekliğini piksel biriminde al. |
| [getHtmlString()](#getHtmlString--) | Bu hücredeki veri ve bazı biçimleri içeren html dizesini al. |
| [getHtmlString(boolean html5)](#getHtmlString-boolean-) | Bu hücredeki veri ve bazı biçimleri içeren html dizesini al. |
| [getIntValue()](#getIntValue--) | Hücrede bulunan tam sayı değerini al. |
| [getLeafs()](#getLeafs--) | Bu hücreye doğrudan başvuran ve hücre değiştirildiğinde güncellenmesi gereken tüm hücreleri al. |
| [getLeafs(boolean recursive)](#getLeafs-boolean-) | Bu hücre değiştirildiğinde güncellenecek tüm hücreleri al. |
| [getMergedRange()](#getMergedRange--) | Birleştirilmiş bir aralığı temsil eden bir [Range](../../com.aspose.cells/range) nesnesi döndürür. |
| [getName()](#getName--) | Hücrenin adını alır. |
| [getNumberCategoryType()](#getNumberCategoryType--) | Bu hücrenin sayı biçimlendirmesinin kategori türünü temsil eder. |
| [getPicture()](#getPicture--) | Bu hücrede gömülü görüntüyü temsil eden bir [Picture](../../com.aspose.cells/picture) örneğini alır; hücrede gömülü görüntü yoksa null döner. |
| [getPrecedents()](#getPrecedents--) | Bu hücrenin formülünde görünen tüm referansları al. |
| [getPrecedentsInCalculation()](#getPrecedentsInCalculation--) | Bu hücrenin formülü hesaplanırken kullandığı tüm öncülleri (geçerli çalışma kitabındaki hücre referansları) al. |
| [getR1C1Formula()](#getR1C1Formula--) | [Cell](../../com.aspose.cells/cell) nesnesinin bir R1C1 formülünü al. |
| [getRichValue()](#getRichValue--) | Hücrenin zengin değerini al. |
| [getRow()](#getRow--) | Hücrenin satır numarasını (sıfır tabanlı) al. |
| [getSharedStyleIndex()](#getSharedStyleIndex--) | Hücrenin stil havuzundaki paylaşılan stil indeksini al. |
| [getStringValue()](#getStringValue--) | Hücrede bulunan dize değerini al. |
| [getStringValue(int formatStrategy)](#getStringValue-int-) | Belirli biçimlendirme stratejisine göre dize değerini al. |
| [getStringValueWithoutFormat()](#getStringValueWithoutFormat--) | Hücrenin değerini herhangi bir biçim olmadan dize olarak al. |
| [getStyle()](#getStyle--) | Hücre stilini al. |
| [getStyle(boolean checkBorders)](#getStyle-boolean-) | checkBorders true ise, diğer hücrelerin kenarlıklarının bu hücrenin stilini etkileyip etkilemeyeceğini kontrol et. |
| [getTable()](#getTable--) | Bu hücreyi içeren tabloyu al. |
| [getType()](#getType--) | Hücre değer tipini temsil eder. |
| [getValidation()](#getValidation--) | Bu hücreye uygulanan doğrulamayı al. |
| [getValidationValue()](#getValidationValue--) | Bu hücreye uygulanan doğrulamanın değerini al. |
| [getValue()](#getValue--) | Bu hücrede bulunan değeri al. |
| [getWidthOfValue()](#getWidthOfValue--) | Değerin genişliğini piksel biriminde alır. |
| [getWorksheet()](#getWorksheet--) | Üst çalışma sayfasını alır. |
| [hasCustomFunction()](#hasCustomFunction--) | Bu hücrenin formülünde özel işlevin (desteklenmeyen işlev) olup olmadığını denetler. |
| [hasCustomStyle()](#hasCustomStyle--) | Bu hücrenin özel stil ayarlarına (ilgili satır, sütun veya çalışma kitabından devralınan varsayılanın farklısı) sahip olup olmadığını gösterir. |
| [hashCode()](#hashCode--) | Belirli bir tür için bir karma işlevi olarak hizmet verir. |
| [insertText(int index, String text)](#insertText-int-java.lang.String-) | Hücreye bazı karakterler ekler. |
| [isArrayFormula()](#isArrayFormula--) | Hücre formülünün dizi formülü olup olmadığını gösterir. |
| [isArrayHeader()](#isArrayHeader--) | Hücre formülünün dizi formülü olduğunu ve dizinin ilk hücresi olduğunu gösterir. |
| [isCheckBoxStyle()](#isCheckBoxStyle--) | Bu hücrenin onay kutusu olarak ayarlanıp ayarlanmadığını gösterir. |
| [isDynamicArrayFormula()](#isDynamicArrayFormula--) | Hücre formülünün dinamik dizi formülü (doğru) mu yoksa eski dizi formülü (yanlış) mu olduğunu gösterir. |
| [isErrorValue()](#isErrorValue--) | Bu hücrenin değerinin bir hata olup olmadığını denetler. |
| [isFormula()](#isFormula--) | Belirtilen hücrenin formül içerip içermediğini temsil eder. |
| [isInArray()](#isInArray--) | Hücre formülünün dizi formülü olup olmadığını gösterir. |
| [isInTable()](#isInTable--) | Bu hücrenin tablo formülünün bir parçası olup olmadığını gösterir. |
| [isMerged()](#isMerged--) | Bir hücrenin birleştirilmiş bir aralığın parçası olup olmadığını denetler. |
| [isNumericValue()](#isNumericValue--) | Bu hücrenin değerinin sayısal (int, double ve datetime) olup olmadığını gösterir. |
| [isRichText()](#isRichText--) | Bu hücrenin dize değerinin zengin biçimlendirilmiş metin olup olmadığını gösterir. |
| [isSharedFormula()](#isSharedFormula--) | Hücre formülünün paylaşılan formülün bir parçası olup olmadığını gösterir. |
| [isStyleSet()](#isStyleSet--) | Hücrenin stilinin ayarlanıp ayarlanmadığını gösterir. |
| [isTableFormula()](#isTableFormula--) | Bu hücrenin tablo formülünün bir parçası olup olmadığını gösterir. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [putValue(boolean boolValue)](#putValue-boolean-) | Hücreye bir boolean değer koyar. |
| [putValue(DateTime dateTime)](#putValue-com.aspose.cells.DateTime-) | Hücreye bir DateTime değeri koyar. |
| [putValue(double doubleValue)](#putValue-double-) | Hücreye bir double değeri koyar. |
| [putValue(int intValue)](#putValue-int-) | Hücreye bir integer değeri koyar. |
| [putValue(Object objectValue)](#putValue-java.lang.Object-) | Hücreye bir nesne değeri koyar. |
| [putValue(String stringValue)](#putValue-java.lang.String-) | Hücreye bir dize değeri koyar. |
| [putValue(String stringValue, boolean isConverted)](#putValue-java.lang.String-boolean-) | Hücreye bir dize değeri koyar ve uygun olduğunda değeri başka bir veri tipine dönüştürür. |
| [putValue(String stringValue, boolean isConverted, boolean setStyle)](#putValue-java.lang.String-boolean-boolean-) | Hücreye bir değer koyar, uygun olduğunda değer başka bir veri tipine dönüştürülür ve hücrenin sayı biçimi sıfırlanır. |
| [removeArrayFormula(boolean leaveNormalFormula)](#removeArrayFormula-boolean-) | Dizi formülünü kaldır. |
| [replace(String placeHolder, String newValue, ReplaceOptions options)](#replace-java.lang.String-java.lang.String-com.aspose.cells.ReplaceOptions-) | Hücrenin metnini seçeneklerle değiştir. |
| [setArrayFormula(String arrayFormula, int rowNumber, int columnNumber)](#setArrayFormula-java.lang.String-int-int-) | Bir hücre aralığına dizi formülü (MS Excel'de CTRL+SHIFT+ENTER ile girilen eski dizi formülü) ayarlar. |
| [setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, boolean isR1C1, boolean isLocal)](#setArrayFormula-java.lang.String-int-int-boolean-boolean-) | Bir hücre aralığına dizi formülü ayarlar. |
| [setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, FormulaParseOptions options)](#setArrayFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-) | Bir hücre aralığına dizi formülü ayarlar. |
| [setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, FormulaParseOptions options, Object[][] values)](#setArrayFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-java.lang.Object-----) | Bir hücre aralığına dizi formülü ayarlar. |
| [setCharacters(FontSetting[] characters)](#setCharacters-com.aspose.cells.FontSetting---) | Hücrenin zengin metin biçimini ayarlar. |
| [setCheckBoxStyle(boolean value)](#setCheckBoxStyle-boolean-) | Bu hücrenin onay kutusu olarak ayarlanıp ayarlanmadığını gösterir. |
| [setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, boolean calculateValue)](#setDynamicArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-boolean-) | Dinamik dizi formülünü ayarlar ve mümkünse formülün komşu hücrelere yayılmasını sağlar. |
| [setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, Object[][] values, boolean calculateRange, boolean calculateValue)](#setDynamicArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-java.lang.Object-----boolean-boolean-) | Dinamik dizi formülünü ayarlar ve mümkünse formülün komşu hücrelere yayılmasını sağlar. |
| [setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, Object[][] values, boolean calculateRange, boolean calculateValue, CalculationOptions copts)](#setDynamicArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-java.lang.Object-----boolean-boolean-com.aspose.cells.CalculationOptions-) | Dinamik dizi formülünü ayarlar ve mümkünse formülün komşu hücrelere yayılmasını sağlar. |
| [setEmbeddedImage(byte[] value)](#setEmbeddedImage-byte---) | Hücrede gömülü resmi ayarlar. |
| [setFormula(String value)](#setFormula-java.lang.String-) | [Cell](../../com.aspose.cells/cell) nesnesinin formülünü ayarlar. |
| [setFormula(String formula, boolean isR1C1, boolean isLocal, Object value)](#setFormula-java.lang.String-boolean-boolean-java.lang.Object-) | Formülü ve formülün değerini ayarla. |
| [setFormula(String formula, FormulaParseOptions options)](#setFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-) | Formülü ve değerini (hesaplanan sonuç) ayarla. |
| [setFormula(String formula, FormulaParseOptions options, Object value)](#setFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-java.lang.Object-) | Formülü ve değerini (hesaplanan sonuç) ayarla. |
| [setFormula(String formula, Object value)](#setFormula-java.lang.String-java.lang.Object-) | Formülü ve değerini (hesaplanan sonuç) ayarla. |
| [setFormulaLocal(String value)](#setFormulaLocal-java.lang.String-) | Hücrenin yerel biçimlendirilmiş formülünü al. |
| [setHtmlString(String value)](#setHtmlString-java.lang.String-) | Bu hücrede veri ve bazı biçimleri içeren html dizesini ayarlar. |
| [setR1C1Formula(String value)](#setR1C1Formula-java.lang.String-) | [Cell](../../com.aspose.cells/cell) nesnesinin R1C1 formülünü ayarlar. |
| [setSharedFormula(String sharedFormula, int rowNumber, int columnNumber)](#setSharedFormula-java.lang.String-int-int-) | Bir hücre aralığına paylaşılan formülleri ayarlar. |
| [setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, boolean isR1C1, boolean isLocal)](#setSharedFormula-java.lang.String-int-int-boolean-boolean-) | Bir hücre aralığına formül ayarlar. |
| [setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, FormulaParseOptions options)](#setSharedFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-) | Bir hücre aralığına paylaşılan formülleri ayarlar. |
| [setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, FormulaParseOptions options, Object[][] values)](#setSharedFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-java.lang.Object-----) | Bir hücre aralığına paylaşılan formülleri ayarlar. |
| [setStyle(Style style)](#setStyle-com.aspose.cells.Style-) | Hücre stilini ayarlar. |
| [setStyle(Style style, boolean explicitFlag)](#setStyle-com.aspose.cells.Style-boolean-) | Stilin değiştirilen özelliğini hücreye uygula. |
| [setStyle(Style style, StyleFlag flag)](#setStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | Bayraklara göre hücre stilini uygula. |
| [setTableFormula(int rowNumber, int columnNumber, int rowIndexOfInputCell, int columnIndexOfInputCell, boolean isRowInput, Object[][] values)](#setTableFormula-int-int-int-int-boolean-java.lang.Object-----) | Bu hücreden başlayan verilen aralık için tek değişkenli veri tablosu oluştur. |
| [setTableFormula(int rowNumber, int columnNumber, int rowIndexOfRowInputCell, int columnIndexOfRowInputCell, int rowIndexOfColumnInputCell, int columnIndexOfColumnInputCell, Object[][] values)](#setTableFormula-int-int-int-int-int-int-java.lang.Object-----) | Bu hücreden başlayan verilen aralık için iki değişkenli veri tablosu oluştur. |
| [setTableFormula(int rowNumber, int columnNumber, String inputCell, boolean isRowInput, Object[][] values)](#setTableFormula-int-int-java.lang.String-boolean-java.lang.Object-----) | Bu hücreden başlayan verilen aralık için tek değişkenli veri tablosu oluştur. |
| [setTableFormula(int rowNumber, int columnNumber, String rowInputCell, String columnInputCell, Object[][] values)](#setTableFormula-int-int-java.lang.String-java.lang.String-java.lang.Object-----) | Bu hücreden başlayan verilen aralık için iki değişkenli veri tablosu oluştur. |
| [setValue(Object value)](#setValue-java.lang.Object-) | Bu hücrede bulunan değeri ayarlar. |
| [toJson()](#toJson--) | [Cell](../../com.aspose.cells/cell) nesnesini JSON yapı verisine dönüştür. |
| [toString()](#toString--) | Geçerli Cell nesnesini temsil eden bir dize döndürür. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### calculate(CalculationOptions options) {#calculate-com.aspose.cells.CalculationOptions-}
```
public void calculate(CalculationOptions options)
```


Hücrenin formülünü hesaplar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| options | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Hesaplama seçenekleri |

### characters(int startIndex, int length) {#characters-int-int-}
```
public FontSetting characters(int startIndex, int length)
```


Hücre metni içindeki bir karakter aralığını temsil eden bir Characters nesnesi döndürür.

**Remarks**

Bu yöntem yalnızca dize değeri olan hücrelerde çalışır.

**Example**

```
         Workbook excel = new Workbook();
         	Cells cells = excel.getWorksheets().get(0).getCells();
         cells.get("A1").putValue("Helloworld");
         cells.get("A1").characters(5, 5).getFont().setBold(true);
         cells.get("A1").characters(5, 5).getFont().setColor(Color.getBlue());
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startIndex | int | Karakterin başlangıç indeksi. |
| length | int | Karakter sayısı. |

**Returns:**
[FontSetting](../../com.aspose.cells/fontsetting) - Characters object.
### containsExternalLink() {#containsExternalLink--}
```
public boolean containsExternalLink()
```


Bu hücrenin harici bir bağlantı içerip içermediğini gösterir. Yalnızca hücre bir formül hücresi olduğunda geçerlidir.

**Returns:**
boolean
### copy(Cell cell) {#copy-com.aspose.cells.Cell-}
```
public void copy(Cell cell)
```


Kaynak hücreden verileri kopyalar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cell | [Cell](../../com.aspose.cells/cell) | Kaynak [Cell](../../com.aspose.cells/cell) nesnesi. |

### equals(Cell cell) {#equals-com.aspose.cells.Cell-}
```
public boolean equals(Cell cell)
```


Bu nesnenin başka bir hücre nesnesiyle aynı hücreye referans verip vermediğini kontrol eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cell | [Cell](../../com.aspose.cells/cell) | başka bir hücre nesnesi |

**Returns:**
boolean - iki hücre nesnesi aynı hücreye işaret ediyorsa true.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Bu nesnenin başka bir nesneyle aynı hücreye referans verip vermediğini kontrol eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| obj | java.lang.Object | başka bir nesne |

**Returns:**
boolean - iki nesne aynı hücreye işaret ediyorsa true.
### getArrayRange() {#getArrayRange--}
```
public CellArea getArrayRange()
```


Hücrenin formülü bir dizi formülü ise dizi aralığını alır.

**Remarks**

Yalnızca hücrenin formülü bir dizi formülü olduğunda uygulanır.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - The array range.
### getBoolValue() {#getBoolValue--}
```
public boolean getBoolValue()
```


Hücrede bulunan boolean değeri alır.

**Returns:**
boolean
### getCharacters() {#getCharacters--}
```
public FontSetting[] getCharacters()
```


Hücre metni içindeki bir karakter aralığını temsil eden tüm Characters nesnelerini döndürür.

**Returns:**
com.aspose.cells.FontSetting[] - Tüm Karakter nesneleri
### getCharacters(boolean flag) {#getCharacters-boolean-}
```
public FontSetting[] getCharacters(boolean flag)
```


Hücre metni içindeki bir karakter aralığını temsil eden tüm Characters nesnelerini döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| bayrak | boolean | Hücre bir tabloda ise tablo stilinin hücreye uygulanıp uygulanmayacağını gösterir. |

**Returns:**
com.aspose.cells.FontSetting[] - Tüm Karakter nesneleri
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumn() {#getColumn--}
```
public int getColumn()
```


Hücrenin sütun numarasını (sıfır tabanlı) alır.

**Returns:**
int
### getComment() {#getComment--}
```
public Comment getComment()
```


Bu hücrenin yorumunu alır.

**Remarks**

Hücreye uygulanacak yorum yoksa, null döndürür.

**Returns:**
[Comment](../../com.aspose.cells/comment)
### getConditionalFormattingResult() {#getConditionalFormattingResult--}
```
public ConditionalFormattingResult getConditionalFormattingResult()
```


Koşullu biçimlendirme sonucunu al.

**Remarks**

Bu hücreye koşullu biçimlendirme uygulanmadıysa null döndürür,

**Returns:**
[ConditionalFormattingResult](../../com.aspose.cells/conditionalformattingresult)
### getDateTimeValue() {#getDateTimeValue--}
```
public DateTime getDateTimeValue()
```


Hücrede bulunan DateTime değerini alır.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getDependents(boolean isAll) {#getDependents-boolean-}
```
public Cell[] getDependents(boolean isAll)
```


Formülü doğrudan bu hücreye referans veren tüm hücreleri al.

**Remarks**

 *  If one reference containing this cell appears in one cell's formula, that cell will be taken as the dependent of this cell, no matter the reference or this cell is used or not while calculating. For example, although cell A2 in formula "=IF(TRUE,A1,A2)" is not used while calculating, this formula is still be taken as A2's dependent.
 *  To get those formulas whose calculated results depend on this cell, please use .
 *  When tracing dependents for one cell, all formulas in the workbook or worksheet will be analized and checked. So it is a time consumed process. If user need to trace dependents for lots of cells, using this method will cause poor performance. For performance consideration, user should use  instead. Or, user may gather precedents map of all cells by  firstly, and then build the dependents map according to the precedents map.

**Example**

```
         Workbook workbook = new Workbook();
         Cells cells = workbook.getWorksheets().get(0).getCells();
         cells.get("A1").setFormula("=B1+SUM(B1:B10)+[Book1.xls]Sheet1!B2");
         cells.get("A2").setFormula("=IF(TRUE,B2,B1)");
         Cell[] dependents = cells.get("B1").getDependents(true);
         for (int i = 0; i <dependents.length; i++)
         {
              System.out.println(dependents[i].getName());
         }
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| isAll | boolean | Diğer çalışma sayfalarındaki formüllerin kontrol edilip edilmeyeceğini gösterir. |

**Returns:**
com.aspose.cells.Cell[]
### getDependentsInCalculation(boolean recursive) {#getDependentsInCalculation-boolean-}
```
public Iterator getDependentsInCalculation(boolean recursive)
```


Hesaplanan sonucu bu hücreye bağlı olan tüm hücreleri alır.

**Remarks**

Bu yöntemi kullanmak için, çalışma kitabının [FormulaSettings.getEnableCalculationChain()](../../com.aspose.cells/formulasettings\#getEnableCalculationChain--) için true değerine ayarlandığından ve bu ayarla tamamen hesaplandığından emin olun. Bu hücreye referans veren bir formül yoksa, null döndürülecektir.

**Example**

```
         Workbook workbook = new Workbook();
         Cells cells = workbook.getWorksheets().get(0).getCells();
         cells.get("A1").setFormula("=B1+SUM(B1:B10)+[Book1.xls]Sheet1!B2");
         cells.get("A2").setFormula("=IF(TRUE,B2,B1)");
         workbook.getSettings().getFormulaSettings().setEnableCalculationChain(true);
         workbook.calculateFormula();
         Iterator en = cells.get("B1").getDependentsInCalculation(false);
         System.out.println("B1's calculation dependents:");
         while(en.hasNext())
         {
             Cell c = (Cell)en.next();
             System.out.println(c.getName());
         }
         en = cells.get("B2").getDependentsInCalculation(false);
         System.out.println("B2's calculation dependents:");
         while(en.hasNext())
         {
             Cell c = (Cell)en.next();
             System.out.println(c.getName());
         }
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| recursive | boolean | Bu hücreye doğrudan referans vermeyen, ancak bu hücrenin diğer yapraklarına referans veren bağımlıların döndürülüp döndürülmeyeceği. |

**Returns:**
java.util.Iterator - Tüm bağımlıları (Cell nesneleri) numaralandırmak için yineleyici
### getDisplayStringValue() {#getDisplayStringValue--}
```
public String getDisplayStringValue()
```


Hücrenin görüntüleme stiliyle biçimlendirilmiş dize değerini alır.

**Returns:**
java.lang.String
### getDisplayStyle() {#getDisplayStyle--}
```
public Style getDisplayStyle()
```


Bu hücrenin görüntüleme stilini al.

**Remarks**

Aynı şekilde, [BorderType.SIDE\_BORDERS](../../com.aspose.cells/bordertype\#SIDE-BORDERS) kullanarak [getDisplayStyle(int)](../../com.aspose.cells/cell\#getDisplayStyle-int-) uygulanır. Yani bu yöntem, komşu hücrelerin stiline ([getStyle()](../../com.aspose.cells/cell\#getStyle--)) göre bu hücrenin üst/alt/sol/sağ kenarlarını kontrol eder ve ayarlar, ancak birleştirilmiş hücreleri kontrol etmez ve komşu hücrelerin görüntü stilini kontrol etmez.

**Returns:**
[Style](../../com.aspose.cells/style) - display style of this cell
### getDisplayStyle(boolean includeMergedBorders) {#getDisplayStyle-boolean-}
```
public Style getDisplayStyle(boolean includeMergedBorders)
```


Bu hücrenin görüntüleme stilini al.

**Remarks**

Belirtilen bayrak false ise, [getDisplayStyle()](../../com.aspose.cells/cell\#getDisplayStyle--) ile aynı olur. Aksi takdirde, [BorderType.SIDE\_BORDERS](../../com.aspose.cells/bordertype\#SIDE-BORDERS)\|[BorderType.DYNAMIC\_STYLE\_BORDERS](../../com.aspose.cells/bordertype\#DYNAMIC-STYLE-BORDERS) kullanarak [getDisplayStyle(int)](../../com.aspose.cells/cell\#getDisplayStyle-int-) ile aynı olur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| includeMergedBorders | boolean | Birleştirilmiş hücrelerin kenarlarının kontrol edilip edilmeyeceğini gösterir. |

**Returns:**
[Style](../../com.aspose.cells/style) - display style of this cell
### getDisplayStyle(int adjacentBorders) {#getDisplayStyle-int-}
```
public Style getDisplayStyle(int adjacentBorders)
```


Bu hücrenin görüntüleme stilini al.

**Remarks**

Bu hücre, koşullu biçimlendirme, liste nesneleri vb. gibi diğer ayarlardan da etkileniyorsa, görüntü stili [getStyle()](../../com.aspose.cells/cell\#getStyle--) ile farklı olabilir.

Komşu hücrelere göre kenarları ayarlama bayrakları için, [BorderType.TOP\_BORDER](../../com.aspose.cells/bordertype\#TOP-BORDER)/[BorderType.BOTTOM\_BORDER](../../com.aspose.cells/bordertype\#BOTTOM-BORDER)/[BorderType.LEFT\_BORDER](../../com.aspose.cells/bordertype\#LEFT-BORDER)/[BorderType.RIGHT\_BORDER](../../com.aspose.cells/bordertype\#RIGHT-BORDER) bu hücrenin sol/sağ/üst/alt komşu hücrelerinin alt/üst/sağ/sol kenarlarının kontrol edilip birleştirilip birleştirilmeyeceğini belirtir.

Performans ve uyumluluk açısından, bazı özel işlemleri belirtmek için bazı enum'lar kullanılır:

[BorderType.HORIZONTAL](../../com.aspose.cells/bordertype\#HORIZONTAL)/[BorderType.VERTICAL](../../com.aspose.cells/bordertype\#VERTICAL) denote whether check and combine the bottom/right border of merged cells to this one.

[BorderType.DIAGONAL](../../com.aspose.cells/bordertype\#DIAGONAL)(that is, both [StyleModifyFlag.DIAGONAL\_UP\_BORDER](../../com.aspose.cells/stylemodifyflag\#DIAGONAL-UP-BORDER) and [StyleModifyFlag.DIAGONAL\_DOWN\_BORDER](../../com.aspose.cells/stylemodifyflag\#DIAGONAL-DOWN-BORDER) have been set) denotes check and combine borders from the display style of adjacent cells.

Lütfen unutmayın, komşu hücrelerin kenarlarını/stillerini, özellikle görüntü stillerini kontrol etmek zaman alan bir işlemdir. Döndürülen stil için kenarları almanıza gerek yoksa, komşu hücrelerin sürecini devre dışı bırakmak için [BorderType.NONE](../../com.aspose.cells/bordertype\#NONE) kullanmak daha iyi performans sağlar. Kenarları yalnızca o hücrelerde tanımlı stillerden ( [BorderType.DIAGONAL](../../com.aspose.cells/bordertype\#DIAGONAL) ayarlamadan) alırken, performans da daha iyi olabilir çünkü bir hücrenin görüntü stilini kontrol etmek de zaman alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| adjacentBorders | int | [BorderType](../../com.aspose.cells/bordertype). Komşu hücrelerin kenarlarına göre hangi kenarların kontrol edilip ayarlanması gerektiğini gösterir. |

**Returns:**
[Style](../../com.aspose.cells/style) - display style of this cell
### getDoubleValue() {#getDoubleValue--}
```
public double getDoubleValue()
```


Hücrede bulunan double değerini al.

**Returns:**
double
### getEmbeddedImage() {#getEmbeddedImage--}
```
public byte[] getEmbeddedImage()
```


Hücrede gömülü resmi al.

**Returns:**
byte[]
### getFloatValue() {#getFloatValue--}
```
public float getFloatValue()
```


Hücrede bulunan float değerini al.

**Returns:**
float
### getFormatConditions() {#getFormatConditions--}
```
public FormatConditionCollection[] getFormatConditions()
```


Bu hücreye uygulanan biçim koşullarını al.

**Returns:**
com.aspose.cells.FormatConditionCollection[] - [FormatConditionCollection](../../com.aspose.cells/formatconditioncollection) nesnesini döndürür
### getFormula() {#getFormula--}
```
public String getFormula()
```


Bir [Cell](../../com.aspose.cells/cell) formülü al.

**Remarks**

Bir formül dizesi her zaman eşittir işareti (=) ile başlar. Ve lütfen parametre ayırıcı olarak her zaman virgül (,) kullanın, örneğin \"=SUM(A1, E1, H2)\".

**Example**

```
         Workbook excel = new Workbook();
         Cells cells = excel.getWorksheets().get(0).getCells();
         cells.get("B6").setFormula("=SUM(B2:B5, E1) + sheet1!A1");
```

**Returns:**
java.lang.String
### getFormula(boolean isR1C1, boolean isLocal) {#getFormula-boolean-boolean-}
```
public String getFormula(boolean isR1C1, boolean isLocal)
```


Bu hücrenin formülünü al.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| isR1C1 | boolean | Formülün R1C1 olarak biçimlendirilip biçimlendirilmesi gerekip gerekmediği. |
| isLocal | boolean | Formülün yerel ayara göre biçimlendirilip biçimlendirilmesi gerekip gerekmediği. |

**Returns:**
java.lang.String - bu hücrenin formülü.
### getFormulaLocal() {#getFormulaLocal--}
```
public String getFormulaLocal()
```


Hücrenin yerel biçimlendirilmiş formülünü al.

**Returns:**
java.lang.String
### getHeightOfValue() {#getHeightOfValue--}
```
public int getHeightOfValue()
```


Değerin yüksekliğini piksel biriminde al.

**Returns:**
int -
### getHtmlString() {#getHtmlString--}
```
public String getHtmlString()
```


Bu hücredeki veri ve bazı biçimleri içeren html dizesini al.

**Returns:**
java.lang.String
### getHtmlString(boolean html5) {#getHtmlString-boolean-}
```
public String getHtmlString(boolean html5)
```


Bu hücredeki veri ve bazı biçimleri içeren html dizesini al.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| html5 | boolean | Değerin html5 ile uyumlu olup olmadığını gösterir. |

**Returns:**
java.lang.String -
### getIntValue() {#getIntValue--}
```
public int getIntValue()
```


Hücrede bulunan tam sayı değerini al.

**Returns:**
int
### getLeafs() {#getLeafs--}
```
public Iterator getLeafs()
```


Bu hücreye doğrudan başvuran ve hücre değiştirildiğinde güncellenmesi gereken tüm hücreleri al.

**Remarks**

NOT: Bu sınıf artık kullanılmamaktadır. Bunun yerine, hesaplama zincirindeki tüm bağımlıları almak için lütfen Cell.GetDependentsInCalculation(bool) metodunu kullanın. Bu özellik Mayıs 2022'den itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
java.util.Iterator - Tüm bağımlıları (Cell) numaralandırmak için Enumerator.
### getLeafs(boolean recursive) {#getLeafs-boolean-}
```
public Iterator getLeafs(boolean recursive)
```


Bu hücre değiştirildiğinde güncellenecek tüm hücreleri al.

**Remarks**

NOT: Bu sınıf artık kullanılmamaktadır. Bunun yerine, hesaplama zincirindeki tüm bağımlıları almak için lütfen Cell.GetDependentsInCalculation(bool) metodunu kullanın. Bu özellik Mayıs 2022'den itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| recursive | boolean | Bu hücreye doğrudan referans vermeyen ancak bu hücrenin diğer yapraklarına referans veren yaprakları döndürür mü? |

**Returns:**
java.util.Iterator - Tüm bağımlıları (Cell) numaralandırmak için Enumerator.
### getMergedRange() {#getMergedRange--}
```
public Range getMergedRange()
```


Birleştirilmiş bir aralığı temsil eden bir [Range](../../com.aspose.cells/range) nesnesi döndürür.

**Returns:**
[Range](../../com.aspose.cells/range) - [Range](../../com.aspose.cells/range) object. Null if this cell is not merged.
### getName() {#getName--}
```
public String getName()
```


Hücrenin adını alır.

**Remarks**

Bir hücre adı, sütun harfi ve satır numarasını içerir. Örneğin, 0. satır ve 0. sütundaki bir hücrenin adı A1'dir.

**Returns:**
java.lang.String
### getNumberCategoryType() {#getNumberCategoryType--}
```
public int getNumberCategoryType()
```


Bu hücrenin sayı biçimlendirmesinin kategori türünü temsil eder.

Bakınız [NumberCategoryType](../../com.aspose.cells/numbercategorytype).

**Remarks**

Hücrenin biçimlendirme deseni koşullu biçimlendirme desenleriyle birleştirildiğinde, döndürülen tür, bu hücrenin mevcut değeri için kullanılan bölüme karşılık gelir. Örneğin, bu hücre için biçimlendirme deseni "\#,\#\#0;(\#,\#\#0);"-";@" ise, hücre değeri sayısal ve 0 değilse, döndürülen tür [NumberCategoryType.NUMBER](../../com.aspose.cells/numbercategorytype\#NUMBER) olur; Hücre değeri 0 veya sayısal değilse, döndürülen tür [NumberCategoryType.TEXT](../../com.aspose.cells/numbercategorytype\#TEXT) olur.

**Returns:**
int
### getPicture() {#getPicture--}
```
public Picture getPicture()
```


Bu hücrede gömülü görüntüyü temsil eden bir [Picture](../../com.aspose.cells/picture) örneğini alır; hücrede gömülü görüntü yoksa null döner.

**Returns:**
[Picture](../../com.aspose.cells/picture)
### getPrecedents() {#getPrecedents--}
```
public ReferredAreaCollection getPrecedents()
```


Bu hücrenin formülünde görünen tüm referansları al.

**Remarks**

 *  Returns null if this is not a formula cell.
 *  All references appearing in this cell's formula will be returned no matter they are referenced or not while calculating. For example, although cell A2 in formula "=IF(TRUE,A1,A2)" is not used while calculating, it is still taken as the formula's precedents.
 *  To get those references which influence the calculation only, please use .

**Example**

```
         Workbook workbook = new Workbook();
         Cells cells = workbook.getWorksheets().get(0).getCells();
         cells.get("A1").setFormula("=B1+SUM(B1:B10)+[Book1.xls]Sheet1!A1");
         ReferredAreaCollection areas = cells.get("A1").getPrecedents();
         for (int i = 0; i <areas.getCount(); i++)
         {
              ReferredArea area = areas.get(i);
              StringBuilder stringBuilder = new StringBuilder();
              if (area.isExternalLink())
              {
                  stringBuilder.append("[");
                  stringBuilder.append(area.getExternalFileName());
                  stringBuilder.append("]");
              }
              stringBuilder.append(area.getSheetName());
              stringBuilder.append("!");
              stringBuilder.append(CellsHelper.cellIndexToName(area.getStartRow(), area.getStartColumn()));
              if (area.isArea())
              {
                  stringBuilder.append(":");
                  stringBuilder.append(CellsHelper.cellIndexToName(area.getEndRow(), area.getEndColumn()));
              }
              System.out.println(stringBuilder.toString());
         }
```

**Returns:**
[ReferredAreaCollection](../../com.aspose.cells/referredareacollection) - Collection of all references appearing in this cell's formula.
### getPrecedentsInCalculation() {#getPrecedentsInCalculation--}
```
public Iterator getPrecedentsInCalculation()
```


Bu hücrenin formülü hesaplanırken kullandığı tüm öncülleri (geçerli çalışma kitabındaki hücre referansları) al.

**Remarks**

Bu yöntem yalnızca çalışma kitabı için [FormulaSettings.getEnableCalculationChain()](../../com.aspose.cells/formulasettings\#getEnableCalculationChain--) true olduğunda ve çalışma kitabı tamamen hesaplandığında çalışabilir. Bu hücre bir formül değilse veya başka hücrelere referans vermiyorsa, null döndürülür.

**Example**

```
         Workbook workbook = new Workbook();
         Cells cells = workbook.getWorksheets().get(0).getCells();
         cells.get("A2").setFormula("=IF(TRUE,B2,B1)");
         workbook.getSettings().getFormulaSettings().setEnableCalculationChain(true);
         workbook.calculateFormula();
         Iterator en = cells.get("A2").getPrecedentsInCalculation();
         System.out.println("A2's calculation precedents:");
         while(en.hasNext())
         {
             ReferredArea r = (ReferredArea)en.next();
             System.out.println(r);
         }
```

**Returns:**
java.util.Iterator - Tüm referansları (ReferredArea) numaralandırmak için Enumerator.
### getR1C1Formula() {#getR1C1Formula--}
```
public String getR1C1Formula()
```


[Cell](../../com.aspose.cells/cell) nesnesinin bir R1C1 formülünü al.

**Returns:**
java.lang.String
### getRichValue() {#getRichValue--}
```
public CellRichValue getRichValue()
```


Hücrenin zengin değerini al.

**Returns:**
[CellRichValue](../../com.aspose.cells/cellrichvalue)
### getRow() {#getRow--}
```
public int getRow()
```


Hücrenin satır numarasını (sıfır tabanlı) al.

**Returns:**
int
### getSharedStyleIndex() {#getSharedStyleIndex--}
```
public int getSharedStyleIndex()
```


Hücrenin stil havuzundaki paylaşılan stil indeksini al.

**Returns:**
int
### getStringValue() {#getStringValue--}
```
public String getStringValue()
```


Hücrede bulunan string değeri alır. Eğer bu hücrenin tipi string ise, string değerini kendisini döndürür. Diğer hücre tipleri için, biçimlendirilmiş string değer (bu hücrenin belirtilen stiliyle biçimlendirilmiş) döndürülür. Biçimlendirilmiş hücre değeri, bir hücreyi metin olarak (örneğin hücreyi metin düzenleyiciye kopyalama veya csv'ye dışa aktarma) kopyaladığınızda Excel'den alabileceğiniz değerle aynıdır.

**Returns:**
java.lang.String
### getStringValue(int formatStrategy) {#getStringValue-int-}
```
public String getStringValue(int formatStrategy)
```


Belirli biçimlendirme stratejisine göre dize değerini al.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| formatStrategy | int | [CellValueFormatStrategy](../../com.aspose.cells/cellvalueformatstrategy). Biçimlendirilmiş strateji. |

**Returns:**
java.lang.String -
### getStringValueWithoutFormat() {#getStringValueWithoutFormat--}
```
public String getStringValueWithoutFormat()
```


Hücrenin değerini herhangi bir biçim olmadan dize olarak al.

**Remarks**

NOT: Bu yöntem artık kullanılmamaktadır. Bunun yerine, kullanıcı değer nesnesini almalı ve değer tipine ve belirli gereksinime göre biçimlendirmelidir. Bu özellik Aralık 2020'den itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
java.lang.String
### getStyle() {#getStyle--}
```
public Style getStyle()
```


Hücre stilini al.

**Remarks**

Hücrenin stilini değiştirmek için, döndürülen stil nesnesini değiştirdikten sonra lütfen Cell.SetStyle() metodunu çağırın. Bu yöntem, parametre için true değeriyle [getStyle(boolean)](../../com.aspose.cells/cell\#getStyle-boolean-) ile aynıdır.

**Returns:**
[Style](../../com.aspose.cells/style) - Style object.
### getStyle(boolean checkBorders) {#getStyle-boolean-}
```
public Style getStyle(boolean checkBorders)
```


checkBorders true ise, diğer hücrelerin kenarlıklarının bu hücrenin stilini etkileyip etkilemeyeceğini kontrol et.

**Remarks**

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| checkBorders | boolean | Diğer hücrelerin kenarlıklarını kontrol et |

**Returns:**
[Style](../../com.aspose.cells/style) - Style object.
### getTable() {#getTable--}
```
public ListObject getTable()
```


Bu hücreyi içeren tabloyu al.

**Returns:**
[ListObject](../../com.aspose.cells/listobject) - 
### getType() {#getType--}
```
public int getType()
```


Hücre değer tipini temsil eder.

Bakınız [CellValueType](../../com.aspose.cells/cellvaluetype).

**Returns:**
int
### getValidation() {#getValidation--}
```
public Validation getValidation()
```


Bu hücreye uygulanan doğrulamayı al.

**Returns:**
[Validation](../../com.aspose.cells/validation) - 
### getValidationValue() {#getValidationValue--}
```
public boolean getValidationValue()
```


Bu hücreye uygulanan doğrulamanın değerini al.

**Returns:**
boolean -
### getValue() {#getValue--}
```
public Object getValue()
```


Bu hücrede bulunan değeri al.

**Remarks**

Olası tip:

null,

Boolean,

DateTime,

Double,

Integer

String.

int değeri için, bir Integer nesnesi veya bir Double nesnesi olarak döndürülebilir. Ve döndürülen değerin her zaman aynı nesne türünde tutulacağına dair bir garanti yoktur.

**Returns:**
java.lang.Object
### getWidthOfValue() {#getWidthOfValue--}
```
public int getWidthOfValue()
```


Değerin genişliğini piksel biriminde alır.

**Returns:**
int -
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```


Üst çalışma sayfasını alır.

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
### hasCustomFunction() {#hasCustomFunction--}
```
public boolean hasCustomFunction()
```


Bu hücrenin formülünde özel işlevin (desteklenmeyen işlev) olup olmadığını denetler.

**Returns:**
boolean
### hasCustomStyle() {#hasCustomStyle--}
```
public boolean hasCustomStyle()
```


Bu hücrenin özel stil ayarlarına (ilgili satır, sütun veya çalışma kitabından devralınan varsayılanın farklısı) sahip olup olmadığını gösterir.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public int hashCode()
```


Belirli bir tür için bir karma işlevi olarak hizmet verir.

**Returns:**
int - Mevcut Cell nesnesi için bir karma kodu.
### insertText(int index, String text) {#insertText-int-java.lang.String-}
```
public void insertText(int index, String text)
```


Hücreye bazı karakterler ekleyin. Hücre zengin biçimlendirilmişse, bu yöntem orijinal biçimlendirmeyi koruyabilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | İndeks. |
| metin | java.lang.String | Eklenmiş metin. |

### isArrayFormula() {#isArrayFormula--}
```
public boolean isArrayFormula()
```


Hücre formülünün dizi formülü olup olmadığını gösterir.

**Returns:**
boolean
### isArrayHeader() {#isArrayHeader--}
```
public boolean isArrayHeader()
```


Hücre formülünün dizi formülü olduğunu ve dizinin ilk hücresi olduğunu gösterir.

**Returns:**
boolean
### isCheckBoxStyle() {#isCheckBoxStyle--}
```
public boolean isCheckBoxStyle()
```


Bu hücrenin onay kutusu olarak ayarlanıp ayarlanmadığını gösterir.

**Returns:**
boolean
### isDynamicArrayFormula() {#isDynamicArrayFormula--}
```
public boolean isDynamicArrayFormula()
```


Hücre formülünün dinamik dizi formülü (doğru) mu yoksa eski dizi formülü (yanlış) mu olduğunu gösterir.

**Returns:**
boolean
### isErrorValue() {#isErrorValue--}
```
public boolean isErrorValue()
```


Bu hücrenin değerinin bir hata olup olmadığını denetler.

**Remarks**

Ayrıca, hesaplanan sonucun bir hata olup olmadığını kontrol etmek için formül hücresine de uygulanır.

**Returns:**
boolean
### isFormula() {#isFormula--}
```
public boolean isFormula()
```


Belirtilen hücrenin formül içerip içermediğini temsil eder.

**Returns:**
boolean
### isInArray() {#isInArray--}
```
public boolean isInArray()
```


Hücre formülünün dizi formülü olup olmadığını gösterir.

**Remarks**

NOT: Bu sınıf artık kullanımdan kaldırılmıştır. Bunun yerine, hücre formülünün bir dizi formülü olup olmadığını kontrol etmek için lütfen Cell.IsArrayFormula kullanın. Bu özellik Mayıs 2018'den itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
boolean
### isInTable() {#isInTable--}
```
public boolean isInTable()
```


Bu hücrenin tablo formülünün bir parçası olup olmadığını gösterir.

**Remarks**

NOT: Bu sınıf artık kullanımdan kaldırılmıştır. Bunun yerine, hücre formülünün tablo formülünün bir parçası olup olmadığını kontrol etmek için lütfen Cell.IsTableFormula kullanın. Bu özellik Mayıs 2018'den itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
boolean
### isMerged() {#isMerged--}
```
public boolean isMerged()
```


Bir hücrenin birleştirilmiş bir aralığın parçası olup olmadığını denetler.

**Returns:**
boolean
### isNumericValue() {#isNumericValue--}
```
public boolean isNumericValue()
```


Bu hücrenin değerinin sayısal (int, double ve datetime) olup olmadığını gösterir.

**Remarks**

Ayrıca, hesaplanan sonucu kontrol etmek için formül hücresine de uygulanır.

**Returns:**
boolean
### isRichText() {#isRichText--}
```
public boolean isRichText()
```


Bu hücrenin dize değerinin zengin biçimlendirilmiş metin olup olmadığını gösterir.

**Returns:**
boolean
### isSharedFormula() {#isSharedFormula--}
```
public boolean isSharedFormula()
```


Hücre formülünün paylaşılan formülün bir parçası olup olmadığını gösterir.

**Returns:**
boolean
### isStyleSet() {#isStyleSet--}
```
public boolean isStyleSet()
```


Hücrenin stilinin ayarlanıp ayarlanmadığını gösterir. False dönerse, bu hücrenin varsayılan hücre biçimine sahip olduğu anlamına gelir.

**Returns:**
boolean
### isTableFormula() {#isTableFormula--}
```
public boolean isTableFormula()
```


Bu hücrenin tablo formülünün bir parçası olup olmadığını gösterir.

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




### putValue(boolean boolValue) {#putValue-boolean-}
```
public void putValue(boolean boolValue)
```


Hücreye bir boolean değer koyar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| boolValue | boolean |  |

### putValue(DateTime dateTime) {#putValue-com.aspose.cells.DateTime-}
```
public void putValue(DateTime dateTime)
```


Hücreye bir DateTime değeri koyar.

**Remarks**

Bir hücreye DateTime değeri ayarlamak, hücrenin otomatik olarak tarih saat olarak biçimlendirileceği anlamına gelmez. DateTime değeri, hem MS Excel hem de Aspose.Cells veri modelinde sayısal değer olarak tutulur. Sayısal değerin kendisi olarak mı yoksa tarih saat olarak mı yorumlanacağı, bu hücreye uygulanan sayı biçimine bağlıdır. Eğer bu hücre tarih saat olarak biçimlendirilmemişse, girdiğiniz DateTime olmasına rağmen sayısal bir değer olarak görüntülenecektir.

**Example**

Bu örnek, bir hücreye DateTime değerinin nasıl ayarlanacağını ve tarih saat olarak görüntülenmesini nasıl sağlayacağını gösterir.

```
         Workbook excel = new Workbook();
         Cells cells = excel.getWorksheets().get(0).getCells();
 
         //Put date time into a cell
         Cell cell = cells.get(0, 0);
         cell.putValue(new DateTime(2023, 5, 15));
         Style style = cell.getStyle(false);
         style.setNumber(14);
         cell.setStyle(style);
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dateTime | [DateTime](../../com.aspose.cells/datetime) | Girdi değeri |

### putValue(double doubleValue) {#putValue-double-}
```
public void putValue(double doubleValue)
```


Hücreye bir double değeri koyar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| doubleValue | double | Girdi değeri |

### putValue(int intValue) {#putValue-int-}
```
public void putValue(int intValue)
```


Hücreye bir integer değeri koyar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| intValue | int | Girdi değeri |

### putValue(Object objectValue) {#putValue-java.lang.Object-}
```
public void putValue(Object objectValue)
```


Hücreye bir nesne değeri koyar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| objectValue | java.lang.Object | girdi değeri |

### putValue(String stringValue) {#putValue-java.lang.String-}
```
public void putValue(String stringValue)
```


Hücreye bir dize değeri koyar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stringValue | java.lang.String | Girdi değeri |

### putValue(String stringValue, boolean isConverted) {#putValue-java.lang.String-boolean-}
```
public void putValue(String stringValue, boolean isConverted)
```


Hücreye bir dize değeri koyar ve uygun olduğunda değeri başka bir veri tipine dönüştürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stringValue | java.lang.String | Girdi değeri |
| isConverted | boolean | True: uygun olduğunda diğer veri tipine dönüştürülür. |

### putValue(String stringValue, boolean isConverted, boolean setStyle) {#putValue-java.lang.String-boolean-boolean-}
```
public void putValue(String stringValue, boolean isConverted, boolean setStyle)
```


Hücreye bir değer koyar, uygun olduğunda değer başka bir veri tipine dönüştürülür ve hücrenin sayı biçimi sıfırlanır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stringValue | java.lang.String | Girdi değeri |
| isConverted | boolean | True: uygun olduğunda diğer veri tipine dönüştürülür. |
| setStyle | boolean | True: diğer veri tipine dönüştürürken sayı biçimini hücrenin stiline ayarlar |

### removeArrayFormula(boolean leaveNormalFormula) {#removeArrayFormula-boolean-}
```
public void removeArrayFormula(boolean leaveNormalFormula)
```


Dizi formülünü kaldır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| leaveNormalFormula | boolean | True, dizi formülünün normal formüle dönüştürülmesini temsil eder. |

### replace(String placeHolder, String newValue, ReplaceOptions options) {#replace-java.lang.String-java.lang.String-com.aspose.cells.ReplaceOptions-}
```
public void replace(String placeHolder, String newValue, ReplaceOptions options)
```


Hücrenin metnini seçeneklerle değiştir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| placeHolder | java.lang.String | Hücre yer tutucu |
| newValue | java.lang.String | Değiştirilecek metin değeri |
| options | [ReplaceOptions](../../com.aspose.cells/replaceoptions) | Değiştirme seçenekleri |

### setArrayFormula(String arrayFormula, int rowNumber, int columnNumber) {#setArrayFormula-java.lang.String-int-int-}
```
public void setArrayFormula(String arrayFormula, int rowNumber, int columnNumber)
```


Bir hücre aralığına dizi formülü (MS Excel'de CTRL+SHIFT+ENTER ile girilen eski dizi formülü) ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arrayFormula | java.lang.String | Dizi formülü. |
| rowNumber | int | Dizi formülünün sonucunu doldurmak için gereken satır sayısı. |
| columnNumber | int | Dizi formülünün sonucunu doldurmak için gereken sütun sayısı. |

### setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, boolean isR1C1, boolean isLocal) {#setArrayFormula-java.lang.String-int-int-boolean-boolean-}
```
public void setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, boolean isR1C1, boolean isLocal)
```


Bir hücre aralığına dizi formülü ayarlar.

**Remarks**

NOT: Bu sınıf artık kullanımdan kaldırılmıştır. Bunun yerine lütfen Cell.SetArrayFormula(string,int,int,FormulaParseOptions) metodunu kullanın. Bu özellik, Aralık 2019'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arrayFormula | java.lang.String | Dizi formülü. |
| rowNumber | int | Dizi formülünün sonucunu doldurmak için gereken satır sayısı. |
| columnNumber | int | Dizi formülünün sonucunu doldurmak için gereken sütun sayısı. |
| isR1C1 | boolean | formülün R1C1 formülü olup olmadığı |
| isLocal | boolean | formülün yerel ayarlara göre biçimlendirilip biçimlendirilmediği |

### setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, FormulaParseOptions options) {#setArrayFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-}
```
public void setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, FormulaParseOptions options)
```


Bir hücre aralığına dizi formülü ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arrayFormula | java.lang.String | Dizi formülü. |
| rowNumber | int | Dizi formülünün sonucunu doldurmak için gereken satır sayısı. |
| columnNumber | int | Dizi formülünün sonucunu doldurmak için gereken sütun sayısı. |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | Formülün ayrıştırılması için seçenekler. |

### setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, FormulaParseOptions options, Object[][] values) {#setArrayFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-java.lang.Object-----}
```
public void setArrayFormula(String arrayFormula, int rowNumber, int columnNumber, FormulaParseOptions options, Object[][] values)
```


Bir hücre aralığına dizi formülü ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arrayFormula | java.lang.String | Dizi formülü. |
| rowNumber | int | Dizi formülünün sonucunu doldurmak için gereken satır sayısı. |
| columnNumber | int | Dizi formülünün sonucunu doldurmak için gereken sütun sayısı. |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | Formülün ayrıştırılması için seçenekler. |
| değerler | java.lang.Object[][] | verilen dizi formülüne sahip hücreler için değerler |

### setCharacters(FontSetting[] characters) {#setCharacters-com.aspose.cells.FontSetting---}
```
public void setCharacters(FontSetting[] characters)
```


Hücrenin zengin metin biçimini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| characters | [FontSetting\[\]](../../com.aspose.cells/fontsetting) | Tüm Characters nesneleri. |

### setCheckBoxStyle(boolean value) {#setCheckBoxStyle-boolean-}
```
public void setCheckBoxStyle(boolean value)
```


Bu hücrenin onay kutusu olarak ayarlanıp ayarlanmadığını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, boolean calculateValue) {#setDynamicArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-boolean-}
```
public CellArea setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, boolean calculateValue)
```


Dinamik dizi formülünü ayarlar ve mümkünse formülün komşu hücrelere yayılmasını sağlar.

**Remarks**

dönen aralık, bu dinamik dizi formülünün döküldüğü gerçek aralıkla aynı olmayabilir. Eğer aralıkta boş olmayan hücreler varsa, formül yalnızca geçerli hücreye ayarlanacak ve \"\\#SPILL!\" olarak işaretlenecektir. Ancak bu tür durumlarda formülün dökülmesi gereken tüm aralığı yine de döndürürüz.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arrayFormula | java.lang.String | formül ifadesi |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | formülü ayrıştırmak için seçenekler. \"Parse\" seçeneği yoksayılacak ve formül her zaman hemen ayrıştırılacaktır |
| calculateValue | boolean | dökülen aralıktaki hücreler için bu dinamik dizi formülünün hesaplanıp hesaplanmayacağı. |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - the range that the formula should spill into.
### setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, Object[][] values, boolean calculateRange, boolean calculateValue) {#setDynamicArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-java.lang.Object-----boolean-boolean-}
```
public CellArea setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, Object[][] values, boolean calculateRange, boolean calculateValue)
```


Dinamik dizi formülünü ayarlar ve mümkünse formülün komşu hücrelere yayılmasını sağlar.

**Remarks**

dönen aralık, bu dinamik dizi formülünün döküldüğü gerçek aralıkla aynı olmayabilir. Eğer aralıkta boş olmayan hücreler varsa, formül yalnızca geçerli hücreye ayarlanacak ve \"\\#SPILL!\" olarak işaretlenecektir. Ancak bu tür durumlarda formülün dökülmesi gereken tüm aralığı yine de döndürürüz.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arrayFormula | java.lang.String | formül ifadesi |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | formülü ayrıştırmak için seçenekler. \"Parse\" seçeneği yoksayılacak ve formül her zaman hemen ayrıştırılacaktır |
| değerler | java.lang.Object[][] | verilen dinamik dizi formülüne sahip hücreler için değerler (hesaplanmış sonuçlar) |
| calculateRange | boolean | Bu dinamik dizi formülü için dökülen aralığın hesaplanıp hesaplanmayacağı. \"values\" parametresi null değil ve bu bayrak false ise, dökülen aralığın yüksekliği values.Length ve genişliği values[0].Length olacaktır. |
| calculateValue | boolean | \"values\" null olduğunda veya bir hücre için \"values\" içindeki ilgili öğe null olduğunda, dökülen aralıktaki hücreler için bu dinamik dizi formülünün hesaplanıp hesaplanmayacağı. |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - the range that the formula should spill into.
### setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, Object[][] values, boolean calculateRange, boolean calculateValue, CalculationOptions copts) {#setDynamicArrayFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-java.lang.Object-----boolean-boolean-com.aspose.cells.CalculationOptions-}
```
public CellArea setDynamicArrayFormula(String arrayFormula, FormulaParseOptions options, Object[][] values, boolean calculateRange, boolean calculateValue, CalculationOptions copts)
```


Dinamik dizi formülünü ayarlar ve mümkünse formülün komşu hücrelere yayılmasını sağlar.

**Remarks**

dönen aralık, bu dinamik dizi formülünün döküldüğü gerçek aralıkla aynı olmayabilir. Eğer aralıkta boş olmayan hücreler varsa, formül yalnızca geçerli hücreye ayarlanacak ve \"\\#SPILL!\" olarak işaretlenecektir. Ancak bu tür durumlarda formülün dökülmesi gereken tüm aralığı yine de döndürürüz.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arrayFormula | java.lang.String | formül ifadesi |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | formülü ayrıştırmak için seçenekler. \"Parse\" seçeneği yoksayılacak ve formül her zaman hemen ayrıştırılacaktır |
| değerler | java.lang.Object[][] | verilen dinamik dizi formülüne sahip hücreler için değerler (hesaplanmış sonuçlar) |
| calculateRange | boolean | Bu dinamik dizi formülü için dökülen aralığın hesaplanıp hesaplanmayacağı. \"values\" parametresi null değil ve bu bayrak false ise, dökülen aralığın yüksekliği values.Length ve genişliği values[0].Length olacaktır. |
| calculateValue | boolean | \"values\" null olduğunda veya bir hücre için \"values\" içindeki ilgili öğe null olduğunda, dökülen aralıktaki hücreler için bu dinamik dizi formülünün hesaplanıp hesaplanmayacağı. |
| copts | [CalculationOptions](../../com.aspose.cells/calculationoptions) | Formülün hesaplanması için seçenekler. Genellikle, performans açısından, [CalculationOptions.getRecursive()](../../com.aspose.cells/calculationoptions\\#getRecursive--) özelliği false olmalıdır. |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - the range that the formula should spill into.
### setEmbeddedImage(byte[] value) {#setEmbeddedImage-byte---}
```
public void setEmbeddedImage(byte[] value)
```


Hücrede gömülü resmi ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | byte[] |  |

### setFormula(String value) {#setFormula-java.lang.String-}
```
public void setFormula(String value)
```


[Cell](../../com.aspose.cells/cell) nesnesinin formülünü ayarlar.

**Remarks**

Bir formül dizesi her zaman eşittir işareti (=) ile başlar. Ve lütfen parametre ayırıcı olarak her zaman virgül (,) kullanın, örneğin \"=SUM(A1, E1, H2)\".

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setFormula(String formula, boolean isR1C1, boolean isLocal, Object value) {#setFormula-java.lang.String-boolean-boolean-java.lang.Object-}
```
public void setFormula(String formula, boolean isR1C1, boolean isLocal, Object value)
```


Formülü ve formülün değerini ayarla.

**Remarks**

NOT: Bu sınıf artık kullanımdan kaldırılmıştır. Bunun yerine lütfen Cell.SetFormula(string,FormulaParseOptions,object) metodunu kullanın. Bu özellik, Aralık 2019'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| formula | java.lang.String | Formül. |
| isR1C1 | boolean | Formülün R1C1 formülü olup olmadığı. |
| isLocal | boolean | Formülün yerel ayara göre biçimlendirilip biçimlendirilmediği. |
| değer | java.lang.Object | Formülün değeri. |

### setFormula(String formula, FormulaParseOptions options) {#setFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-}
```
public void setFormula(String formula, FormulaParseOptions options)
```


Formülü ve değerini (hesaplanan sonuç) ayarla.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| formula | java.lang.String | Formül. |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | Formülün ayrıştırılması için seçenekler. |

### setFormula(String formula, FormulaParseOptions options, Object value) {#setFormula-java.lang.String-com.aspose.cells.FormulaParseOptions-java.lang.Object-}
```
public void setFormula(String formula, FormulaParseOptions options, Object value)
```


Formülü ve değerini (hesaplanan sonuç) ayarla.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| formula | java.lang.String | Formül. |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | Formülün ayrıştırılması için seçenekler. |
| değer | java.lang.Object | Formülün değeri (hesaplanmış sonuç). |

### setFormula(String formula, Object value) {#setFormula-java.lang.String-java.lang.Object-}
```
public void setFormula(String formula, Object value)
```


Formülü ve değerini (hesaplanan sonuç) ayarla.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| formula | java.lang.String | Formül. |
| değer | java.lang.Object | Formülün değeri (hesaplanmış sonuç). |

### setFormulaLocal(String value) {#setFormulaLocal-java.lang.String-}
```
public void setFormulaLocal(String value)
```


Hücrenin yerel biçimlendirilmiş formülünü al.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setHtmlString(String value) {#setHtmlString-java.lang.String-}
```
public void setHtmlString(String value)
```


Bu hücrede veri ve bazı biçimleri içeren html dizesini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setR1C1Formula(String value) {#setR1C1Formula-java.lang.String-}
```
public void setR1C1Formula(String value)
```


[Cell](../../com.aspose.cells/cell) nesnesinin R1C1 formülünü ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setSharedFormula(String sharedFormula, int rowNumber, int columnNumber) {#setSharedFormula-java.lang.String-int-int-}
```
public void setSharedFormula(String sharedFormula, int rowNumber, int columnNumber)
```


Bir hücre aralığına paylaşılan formülleri ayarlar.

**Remarks**

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sharedFormula | java.lang.String | Paylaşılan formül. |
| rowNumber | int | Formülü doldurmak için satır sayısı. |
| columnNumber | int | Formülü doldurmak için sütun sayısı. |

### setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, boolean isR1C1, boolean isLocal) {#setSharedFormula-java.lang.String-int-int-boolean-boolean-}
```
public void setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, boolean isR1C1, boolean isLocal)
```


Bir hücre aralığına formül ayarlar.

**Remarks**

NOT: Bu sınıf artık kullanımdan kaldırılmıştır. Bunun yerine lütfen Cell.SetSharedFormula(string,int,int,FormulaParseOptions) yöntemini kullanın. Bu özellik Aralık 2019'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sharedFormula | java.lang.String | Paylaşılan formül. |
| rowNumber | int | Formülü doldurmak için satır sayısı. |
| columnNumber | int | Formülü doldurmak için sütun sayısı. |
| isR1C1 | boolean | formülün R1C1 formülü olup olmadığı |
| isLocal | boolean | formülün yerel ayarlara göre biçimlendirilip biçimlendirilmediği |

### setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, FormulaParseOptions options) {#setSharedFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-}
```
public void setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, FormulaParseOptions options)
```


Bir hücre aralığına paylaşılan formülleri ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sharedFormula | java.lang.String | Paylaşılan formül. |
| rowNumber | int | Formülü doldurmak için satır sayısı. |
| columnNumber | int | Formülü doldurmak için sütun sayısı. |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | Formülün ayrıştırılması için seçenekler. |

### setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, FormulaParseOptions options, Object[][] values) {#setSharedFormula-java.lang.String-int-int-com.aspose.cells.FormulaParseOptions-java.lang.Object-----}
```
public void setSharedFormula(String sharedFormula, int rowNumber, int columnNumber, FormulaParseOptions options, Object[][] values)
```


Bir hücre aralığına paylaşılan formülleri ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sharedFormula | java.lang.String | Paylaşılan formül. |
| rowNumber | int | Formülü doldurmak için satır sayısı. |
| columnNumber | int | Formülü doldurmak için sütun sayısı. |
| options | [FormulaParseOptions](../../com.aspose.cells/formulaparseoptions) | Formülün ayrıştırılması için seçenekler. |
| değerler | java.lang.Object[][] | verilen ortak formülle olan hücreler için değerler |

### setStyle(Style style) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style style)
```


Hücre stilini ayarlar.

**Remarks**

Kenarlık ayarları değiştirildiğinde, ayarlanan hücrelerin kenarlığı da güncellenecektir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | Hücre stili. |

### setStyle(Style style, boolean explicitFlag) {#setStyle-com.aspose.cells.Style-boolean-}
```
public void setStyle(Style style, boolean explicitFlag)
```


Stilin değiştirilen özelliğini hücreye uygula.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | Hücre stili. |
| explicitFlag | boolean | True, yalnızca açıkça ayarlanmış biçimlendirmeyi üzerine yazar. |

### setStyle(Style style, StyleFlag flag) {#setStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void setStyle(Style style, StyleFlag flag)
```


Bayraklara göre hücre stilini uygula.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | Hücre stili. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | Stil bayrağı. |

### setTableFormula(int rowNumber, int columnNumber, int rowIndexOfInputCell, int columnIndexOfInputCell, boolean isRowInput, Object[][] values) {#setTableFormula-int-int-int-int-boolean-java.lang.Object-----}
```
public void setTableFormula(int rowNumber, int columnNumber, int rowIndexOfInputCell, int columnIndexOfInputCell, boolean isRowInput, Object[][] values)
```


Bu hücreden başlayan verilen aralık için tek değişkenli veri tablosu oluştur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowNumber | int | Formülü doldurmak için satır sayısı. |
| columnNumber | int | Formülü doldurmak için sütun sayısı. |
| rowIndexOfInputCell | int | giriş hücresinin satır indeksi |
| columnIndexOfInputCell | int | giriş hücresinin sütun indeksi |
| isRowInput | boolean | Giriş hücresinin satır giriş hücresi (true) mı yoksa sütun giriş hücresi (false) mı olduğunu gösterir. |
| değerler | java.lang.Object[][] | tablo formül aralığındaki hücreler için değerler |

### setTableFormula(int rowNumber, int columnNumber, int rowIndexOfRowInputCell, int columnIndexOfRowInputCell, int rowIndexOfColumnInputCell, int columnIndexOfColumnInputCell, Object[][] values) {#setTableFormula-int-int-int-int-int-int-java.lang.Object-----}
```
public void setTableFormula(int rowNumber, int columnNumber, int rowIndexOfRowInputCell, int columnIndexOfRowInputCell, int rowIndexOfColumnInputCell, int columnIndexOfColumnInputCell, Object[][] values)
```


Bu hücreden başlayan verilen aralık için iki değişkenli veri tablosu oluştur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowNumber | int | Formülü doldurmak için satır sayısı. |
| columnNumber | int | Formülü doldurmak için sütun sayısı. |
| rowIndexOfRowInputCell | int | satır giriş hücresinin satır indeksi |
| columnIndexOfRowInputCell | int | satır giriş hücresinin sütun indeksi |
| rowIndexOfColumnInputCell | int | sütun giriş hücresinin satır indeksi |
| columnIndexOfColumnInputCell | int | sütun giriş hücresinin sütun indeksi |
| değerler | java.lang.Object[][] | tablo formül aralığındaki hücreler için değerler |

### setTableFormula(int rowNumber, int columnNumber, String inputCell, boolean isRowInput, Object[][] values) {#setTableFormula-int-int-java.lang.String-boolean-java.lang.Object-----}
```
public void setTableFormula(int rowNumber, int columnNumber, String inputCell, boolean isRowInput, Object[][] values)
```


Bu hücreden başlayan verilen aralık için tek değişkenli veri tablosu oluştur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowNumber | int | Formülü doldurmak için satır sayısı. |
| columnNumber | int | Formülü doldurmak için sütun sayısı. |
| inputCell | java.lang.String | giriş hücresi |
| isRowInput | boolean | Giriş hücresinin satır giriş hücresi (true) mı yoksa sütun giriş hücresi (false) mı olduğunu gösterir. |
| değerler | java.lang.Object[][] | tablo formül aralığındaki hücreler için değerler |

### setTableFormula(int rowNumber, int columnNumber, String rowInputCell, String columnInputCell, Object[][] values) {#setTableFormula-int-int-java.lang.String-java.lang.String-java.lang.Object-----}
```
public void setTableFormula(int rowNumber, int columnNumber, String rowInputCell, String columnInputCell, Object[][] values)
```


Bu hücreden başlayan verilen aralık için iki değişkenli veri tablosu oluştur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowNumber | int | Formülü doldurmak için satır sayısı. |
| columnNumber | int | Formülü doldurmak için sütun sayısı. |
| rowInputCell | java.lang.String | satır giriş hücresi |
| columnInputCell | java.lang.String | sütun giriş hücresi |
| değerler | java.lang.Object[][] | tablo formül aralığındaki hücreler için değerler |

### setValue(Object value) {#setValue-java.lang.Object-}
```
public void setValue(Object value)
```


Bu hücrede bulunan değeri ayarlar.

**Remarks**

Olası tip:

null,

Boolean,

DateTime,

Double,

Integer

String.

int değeri için, bir Integer nesnesi veya bir Double nesnesi olarak döndürülebilir. Ve döndürülen değerin her zaman aynı nesne türünde tutulacağına dair bir garanti yoktur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.Object |  |

### toJson() {#toJson--}
```
public String toJson()
```


[Cell](../../com.aspose.cells/cell) nesnesini JSON yapı verisine dönüştür.

**Returns:**
java.lang.String -
### toString() {#toString--}
```
public String toString()
```


Geçerli Cell nesnesini temsil eden bir dize döndürür.

**Returns:**
java.lang.String -
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

