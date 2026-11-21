---
title: "Satır"
second_title: "Aspose.Cells for Java API Referansı"
description: "Bir çalışma sayfasındaki tek bir satırı temsil eder."
type: docs
url: /tr/java/com.aspose.cells/row/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class Row implements Iterable
```

Bir çalışma sayfasındaki tek bir satırı temsil eder.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //Obtaining the reference of the first worksheet
         Worksheet worksheet = workbook.getWorksheets().get(0);
         Style style = workbook.createStyle();
 
         //Setting the background color to Blue
         style.setBackgroundColor(Color.getBlue());
 
         //Setting the foreground color to Red
         style.setForegroundColor(Color.getRed());
 
         //setting Background Pattern
         style.setPattern(BackgroundType.DIAGONAL_STRIPE);
 
         //New Style Flag
         StyleFlag styleFlag = new StyleFlag();
 
         //Set All Styles
         styleFlag.setAll(true);
 
          //Get first row
         Row row = worksheet.getCells().getRows().get(0);
          //Apply Style to first row
         row.applyStyle(style, styleFlag);
 
         //Saving the Excel file
         workbook.save("book1.xls");
```
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [applyStyle(Style style, StyleFlag flag)](#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | Tüm bir satır için biçimleri uygular. |
| [copySettings(Row source, boolean checkStyle)](#copySettings-com.aspose.cells.Row-boolean-) | Satırın ayarlarını kopyala, örneğin stil, yükseklik, görünürlük, ... vb. |
| [equals(Row row)](#equals-com.aspose.cells.Row-) | Bu nesnenin başka bir satır nesnesiyle aynı satıra referans verip vermediğini kontrol eder. |
| [equals(Object obj)](#equals-java.lang.Object-) | Bu nesnenin başka bir nesneyle aynı satıra referans verip vermediğini kontrol eder. |
| [get(int column)](#get-int-) | Hücreyi alır. |
| [getCellByIndex(int index)](#getCellByIndex-int-) | Bu satırın hücre koleksiyonundaki belirli indeksle hücreyi al. |
| [getCellOrNull(int column)](#getCellOrNull-int-) | Belirli indeksteki hücreyi veya null değerini alır. |
| [getClass()](#getClass--) |  |
| [getFirstCell()](#getFirstCell--) | Satırdaki ilk hücre nesnesini alır. |
| [getFirstDataCell()](#getFirstDataCell--) | Satırdaki ilk boş olmayan hücreyi alır. |
| [getGroupLevel()](#getGroupLevel--) | Satırın grup seviyesini alır. |
| [getHeight()](#getHeight--) | Satır yüksekliğini Point biriminde alır. |
| [getIndex()](#getIndex--) | Bu satırın indeksini alır. |
| [getLastCell()](#getLastCell--) | Satırdaki son hücre nesnesini alır. |
| [getLastDataCell()](#getLastDataCell--) | Satırdaki son boş olmayan hücreyi alır. |
| [getStyle()](#getStyle--) | Bu satırın stilini alır. |
| [hasCustomStyle()](#hasCustomStyle--) | Bu satırın, çalışma kitabından devralınan varsayılan stilden farklı özel stil ayarlarına sahip olup olmadığını gösterir. |
| [hashCode()](#hashCode--) |  |
| [isBlank()](#isBlank--) | Satırın herhangi bir veri içerip içermediğini gösterir |
| [isCollapsed()](#isCollapsed--) | satırın daraltılmış olup olmadığı |
| [isHeightMatched()](#isHeightMatched--) | Satır yüksekliğinin çalışma kitabının mevcut varsayılan yazı tipi ayarına uygun olup olmadığını gösterir. |
| [isHidden()](#isHidden--) | Satırın gizli olup olmadığını gösterir. |
| [iterator()](#iterator--) | Hücre enumerator'ünü alır |
| [iterator(boolean reversed, boolean sync)](#iterator-boolean-boolean-) | Bu satırdaki hücreleri yineleyen bir enumerator alır. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCollapsed(boolean value)](#setCollapsed-boolean-) | satırın daraltılmış olup olmadığı |
| [setGroupLevel(byte value)](#setGroupLevel-byte-) | Satırın grup seviyesini alır. |
| [setHeight(double value)](#setHeight-double-) | Satır yüksekliğini Nokta biriminde ayarlar. |
| [setHeightMatched(boolean value)](#setHeightMatched-boolean-) | Satır yüksekliğinin çalışma kitabının mevcut varsayılan yazı tipi ayarına uygun olup olmadığını gösterir. |
| [setHidden(boolean value)](#setHidden-boolean-) | Satırın gizli olup olmadığını gösterir. |
| [setStyle(Style style)](#setStyle-com.aspose.cells.Style-) | Bu satırın stilini ayarlar. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### applyStyle(Style style, StyleFlag flag) {#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void applyStyle(Style style, StyleFlag flag)
```


Tüm bir satır için biçimleri uygular.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | Uygulanacak stil nesnesi. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | Uygulanan biçimlendirme özelliklerini gösteren bayraklar. |

### copySettings(Row source, boolean checkStyle) {#copySettings-com.aspose.cells.Row-boolean-}
```
public void copySettings(Row source, boolean checkStyle)
```


Satırın ayarlarını kopyala, örneğin stil, yükseklik, görünürlük, ... vb.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| source | [Row](../../com.aspose.cells/row) | Ayarları bu satıra kopyalanacak kaynak satır |
| checkStyle | boolean | stil kontrolü ve toplama. Yalnızca iki satır nesnesi farklı çalışma kitaplarına ait olduğunda ve iki çalışma kitabının stilleri farklı olduğunda etkili olur ve gerekir. |

### equals(Row row) {#equals-com.aspose.cells.Row-}
```
public boolean equals(Row row)
```


Bu nesnenin başka bir satır nesnesiyle aynı satıra referans verip vermediğini kontrol eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| row | [Row](../../com.aspose.cells/row) | başka bir satır nesnesi |

**Returns:**
boolean - iki satır nesnesi aynı satıra işaret ediyorsa true.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Bu nesnenin başka bir nesneyle aynı satıra referans verip vermediğini kontrol eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| obj | java.lang.Object | başka bir nesne |

**Returns:**
boolean - iki nesne aynı satıra işaret ediyorsa true.
### get(int column) {#get-int-}
```
public Cell get(int column)
```


Hücreyi alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sütun | int | Sütun indeksi |

**Returns:**
[Cell](../../com.aspose.cells/cell) - 
### getCellByIndex(int index) {#getCellByIndex-int-}
```
public Cell getCellByIndex(int index)
```


Bu satırın hücre koleksiyonundaki belirli indeksle hücreyi al.

**Remarks**

Tüm hücreleri değişiklik yapmadan sıralı olarak dolaşmak için, [iterator()](../../com.aspose.cells/row\\#iterator--) kullanmak, bu yöntemi tek tek hücre almaktan daha iyi performans sağlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | Bu satırın hücre koleksiyonundaki hücrenin indeks (konumu). |

**Returns:**
[Cell](../../com.aspose.cells/cell) - The Cell object at given position.
### getCellOrNull(int column) {#getCellOrNull-int-}
```
public Cell getCellOrNull(int column)
```


Belirli indeksteki hücreyi veya null değerini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sütun | int | Sütun indeksi |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Returns the cell object if the cell exists. Or returns null if the cell object does not exist.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFirstCell() {#getFirstCell--}
```
public Cell getFirstCell()
```


Satırdaki ilk hücre nesnesini alır.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getFirstDataCell() {#getFirstDataCell--}
```
public Cell getFirstDataCell()
```


Satırdaki ilk boş olmayan hücreyi alır.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getGroupLevel() {#getGroupLevel--}
```
public byte getGroupLevel()
```


Satırın grup seviyesini alır.

**Returns:**
byte
### getHeight() {#getHeight--}
```
public double getHeight()
```


Satır yüksekliğini Point biriminde alır.

**Returns:**
double
### getIndex() {#getIndex--}
```
public int getIndex()
```


Bu satırın indeksini alır.

**Returns:**
int
### getLastCell() {#getLastCell--}
```
public Cell getLastCell()
```


Satırdaki son hücre nesnesini alır.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getLastDataCell() {#getLastDataCell--}
```
public Cell getLastDataCell()
```


Satırdaki son boş olmayan hücreyi alır.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getStyle() {#getStyle--}
```
public Style getStyle()
```


Bu satırın stilini alır.

**Remarks**

Döndürülen stil nesnesi doğrudan değiştirilirse bu satır ya da bu satırdaki hücreler üzerinde etkisi olmaz. Değişikliği bu satıra uygulamak için [applyStyle(Style,StyleFlag)](../../com.aspose.cells/row\\#applyStyle-Style-StyleFlag-) veya [setStyle(Style)](../../com.aspose.cells/row\\#setStyle-Style-) metodunu çağırmanız gerekir.

Satırın stili, bu satırdaki hücreler tarafından (özelleştirilmiş stil ayarı olmayan hücreler, örneğin stil açıkça ayarlanmamış mevcut hücreler veya henüz oluşturulmamış hücreler) devralınacak stildir.

**Returns:**
[Style](../../com.aspose.cells/style)
### hasCustomStyle() {#hasCustomStyle--}
```
public boolean hasCustomStyle()
```


Bu satırın, çalışma kitabından devralınan varsayılan stilden farklı özel stil ayarlarına sahip olup olmadığını gösterir.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isBlank() {#isBlank--}
```
public boolean isBlank()
```


Satırın herhangi bir veri içerip içermediğini gösterir

**Returns:**
boolean
### isCollapsed() {#isCollapsed--}
```
public boolean isCollapsed()
```


satırın daraltılmış olup olmadığı

**Returns:**
boolean
### isHeightMatched() {#isHeightMatched--}
```
public boolean isHeightMatched()
```


Satır yüksekliğinin çalışma kitabının mevcut varsayılan yazı tipi ayarına uygun olup olmadığını gösterir. Bu özelliğin true olması aynı zamanda satır yüksekliğinin kullanıcı tarafından özel bir değer ayarlanmamış \"otomatik\" olduğunu gösterir.

**Remarks**

Bu özellik true olduğunda, bu satırdaki içerik değişirse, genellikle satır yüksekliği yeniden hesaplanmalıdır (örneğin [Worksheet.autoFitRows()](../../com.aspose.cells/worksheet\\#autoFitRows--) kullanılarak) böylece çalışma kitabını ms excel'de açtığınızda gösterilenle aynı sonuç elde edilir.

**Returns:**
boolean
### isHidden() {#isHidden--}
```
public boolean isHidden()
```


Satırın gizli olup olmadığını gösterir.

**Returns:**
boolean
### iterator() {#iterator--}
```
public Iterator iterator()
```


Hücre enumerator'ünü alır

**Example**

```
         Workbook workbook = new Workbook("template.xlsx");
         	Cells cells = workbook.getWorksheets().get(0).getCells();
 
         	Iterator en = cells.getRows().get(1).iterator();
         	while (en.hasNext())
         	{
         	    Cell cell = (Cell)en.next();
         	    System.out.println(cell.getName() + ": " + cell.getValue());
         	}
```

**Returns:**
java.util.Iterator - Bu satırdaki mevcut tüm hücreleri dolaşacak hücre enumerator'ü.
### iterator(boolean reversed, boolean sync) {#iterator-boolean-boolean-}
```
public Iterator iterator(boolean reversed, boolean sync)
```


Bu satırdaki hücreleri yineleyen bir enumerator alır.

**Remarks**

Satır, enumerator ile dolaşım sırasında (yeni Hücre oluşturulmasına veya mevcut Hücre'nin kaldırılmasına neden olabilecek işlemlerle) değiştirilecekse, normal enumerator yerine senkronize enumerator kullanılmalıdır; böylece dolaşım son MoveNext() tarafından dolaşılmış olanın hemen sonrasından devam edebilir. Ancak hiçbir öğenin atlanmaması veya tekrar dolaşılmaması avantajının yanı sıra, senkronize enumerator'ün dezavantajı, normal enumerator ile karşılaştırıldığında performansın biraz düşmesidir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ters | boolean | hücreleri ters sırada numaralandırıp numaralandırmayacağı |
| eşzamanlı | boolean | dönen yineleyicinin bu satırdaki hücrelerin değişikliklerini kontrol edip onunla senkronize kalıp kalmayacağı. |

**Returns:**
java.util.Iterator - Bu satırdaki mevcut tüm hücreleri dolaşacak hücre enumerator'ü.
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setCollapsed(boolean value) {#setCollapsed-boolean-}
```
public void setCollapsed(boolean value)
```


satırın daraltılmış olup olmadığı

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setGroupLevel(byte value) {#setGroupLevel-byte-}
```
public void setGroupLevel(byte value)
```


Satırın grup seviyesini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | byte |  |

### setHeight(double value) {#setHeight-double-}
```
public void setHeight(double value)
```


Satır yüksekliğini Nokta biriminde ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setHeightMatched(boolean value) {#setHeightMatched-boolean-}
```
public void setHeightMatched(boolean value)
```


Satır yüksekliğinin çalışma kitabının mevcut varsayılan yazı tipi ayarına uygun olup olmadığını gösterir. Bu özelliğin true olması aynı zamanda satır yüksekliğinin kullanıcı tarafından özel bir değer ayarlanmamış \"otomatik\" olduğunu gösterir.

**Remarks**

Bu özellik true olduğunda, bu satırdaki içerik değişirse, genellikle satır yüksekliği yeniden hesaplanmalıdır (örneğin [Worksheet.autoFitRows()](../../com.aspose.cells/worksheet\\#autoFitRows--) kullanılarak) böylece çalışma kitabını ms excel'de açtığınızda gösterilenle aynı sonuç elde edilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setHidden(boolean value) {#setHidden-boolean-}
```
public void setHidden(boolean value)
```


Satırın gizli olup olmadığını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setStyle(Style style) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style style)
```


Bu satırın stilini ayarlar.

**Remarks**

Bu yöntem yalnızca verilen stili bu satır için varsayılan stil olarak ayarlar, bu satırdaki mevcut hücrelerin stil ayarlarını değiştirmez. Mevcut hücrelerin stil ayarlarını aynı anda belirtilen stile güncellemek için lütfen [applyStyle(Style,StyleFlag)](../../com.aspose.cells/row\#applyStyle-Style-StyleFlag-) yöntemini kullanın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | bu satırdaki hücreler için varsayılan stil olarak kullanılacak stil. |

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

