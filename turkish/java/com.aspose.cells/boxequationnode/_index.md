---
title: "BoxEquationNode"
second_title: "Aspose.Cells for Java API Referansı"
description: "Bu sınıf, bir denklemin bileşenlerini gruplamak için kullanılan kutu işlevini belirtir."
type: docs
url: /tr/java/com.aspose.cells/boxequationnode/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.FontSetting](../../com.aspose.cells/fontsetting), [com.aspose.cells.EquationNode](../../com.aspose.cells/equationnode)
```
public class BoxEquationNode extends EquationNode
```

Bu sınıf, bir denklemin bileşenlerini gruplamak için kullanılan kutu işlevini belirtir.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [addChild(EquationNode node)](#addChild-com.aspose.cells.EquationNode-) | Belirtilen düğümü, geçerli düğümün alt düğüm listesine son olarak ekler. |
| [addChild(int equationType)](#addChild-int-) | Geçerli düğümün alt düğüm listesine, belirtilen türde bir düğümü son olarak ekleyin. |
| [createNode(int equationType, Workbook workbook, EquationNode parent)](#createNode-int-com.aspose.cells.Workbook-com.aspose.cells.EquationNode-) | Belirtilen türde bir düğüm oluştur. |
| [equals(Object obj)](#equals-java.lang.Object-) | Geçerli denklem düğümünün belirtilen düğüme eşit olup olmadığını belirle. |
| [getChild(int index)](#getChild-int-) | Geçerli düğümün çocukları arasında belirtilen indeksteki düğümü döndürür. |
| [getClass()](#getClass--) |  |
| [getEquationType()](#getEquationType--) | Geçerli düğümün denklem türünü al. |
| [getFont()](#getFont--) | Bu nesnenin yazı tipini döndürür. |
| [getLength()](#getLength--) | Karakterlerin uzunluğunu alır. |
| [getParentNode()](#getParentNode--) | Geçerli düğümün üst düğümünü belirtir. |
| [getStartIndex()](#getStartIndex--) | Karakterlerin başlangıç indeksini alır. |
| [getTextOptions()](#getTextOptions--) | Metin seçeneklerini döndürür. |
| [getType()](#getType--) | Düğümün türünü temsil eder. |
| [hashCode()](#hashCode--) |  |
| [insertAfter(int equationType)](#insertAfter-int-) | Belirtilen düğümü geçerli düğümün sonrasına ekler. |
| [insertBefore(int equationType)](#insertBefore-int-) | Belirtilen düğümü geçerli düğümün önüne ekler. |
| [insertChild(int index, int equationType)](#insertChild-int-int-) | Belirtilen tipte bir düğümü, geçerli düğümün alt düğüm listesinde belirtilen indeks konumuna ekler. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove()](#remove--) | Kendisini üst düğümden kaldırır. |
| [removeAllChildren()](#removeAllChildren--) | Geçerli düğümün tüm alt düğümlerini kaldırır. |
| [removeChild(EquationNode node)](#removeChild-com.aspose.cells.EquationNode-) | Belirtilen düğümü, geçerli düğümün alt düğümlerinden kaldırır. |
| [removeChild(int index)](#removeChild-int-) | Belirtilen indeksteki düğümü, geçerli düğümün alt düğümlerinden kaldırır. |
| [setParentNode(EquationNode value)](#setParentNode-com.aspose.cells.EquationNode-) | Geçerli düğümün üst düğümünü belirtir. |
| [setWordArtStyle(int style)](#setWordArtStyle-int-) | Önceden ayarlanmış WordArt stilini ayarlar. |
| [toLaTeX()](#toLaTeX--) | Bu denklemi LaTeX ifadesine dönüştür. |
| [toMathML()](#toMathML--) | Bu denklemi MathML ifadesine dönüştür. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addChild(EquationNode node) {#addChild-com.aspose.cells.EquationNode-}
```
public void addChild(EquationNode node)
```


Belirtilen düğümü, geçerli düğümün alt düğüm listesine son olarak ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| node | [EquationNode](../../com.aspose.cells/equationnode) | Belirtilen düğüm |

### addChild(int equationType) {#addChild-int-}
```
public EquationNode addChild(int equationType)
```


Geçerli düğümün alt düğüm listesine, belirtilen türde bir düğümü son olarak ekleyin.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| equationType | int | [EquationNodeType](../../com.aspose.cells/equationnodetype). Denklem Düğümlerinin Türleri |

**Returns:**
[EquationNode](../../com.aspose.cells/equationnode) - If the specified type exists, the corresponding node is returned, and if the type does not exist, a node of unknown type is returned.
### createNode(int equationType, Workbook workbook, EquationNode parent) {#createNode-int-com.aspose.cells.Workbook-com.aspose.cells.EquationNode-}
```
public static EquationNode createNode(int equationType, Workbook workbook, EquationNode parent)
```


Belirtilen türde bir düğüm oluştur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| equationType | int | [EquationNodeType](../../com.aspose.cells/equationnodetype). Denklem Düğümlerinin Türleri |
| workbook | [Workbook](../../com.aspose.cells/workbook) | Denklemle ilişkili çalışma kitabı nesnesi |
| parent | [EquationNode](../../com.aspose.cells/equationnode) | Bu düğümün bulunduğu üst düğüm |

**Returns:**
[EquationNode](../../com.aspose.cells/equationnode) - If the specified type exists, the corresponding node is returned, and if the type does not exist, a node of unknown type is returned.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Geçerli denklem düğümünün belirtilen düğüme eşit olup olmadığını belirle.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| obj | java.lang.Object | Belirtilen düğüm |

**Returns:**
boolean -
### getChild(int index) {#getChild-int-}
```
public EquationNode getChild(int index)
```


Geçerli düğümün çocukları arasında belirtilen indeksteki düğümü döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | Düğümün indeksi |

**Returns:**
[EquationNode](../../com.aspose.cells/equationnode) - Returns the corresponding node if the specified node exists, otherwise returns null.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getEquationType() {#getEquationType--}
```
public int getEquationType()
```


Geçerli düğümün denklem türünü al.

Bkz. [EquationNodeType](../../com.aspose.cells/equationnodetype).

**Returns:**
int
### getFont() {#getFont--}
```
public Font getFont()
```


Bu nesnenin yazı tipini döndürür.

**Returns:**
[Font](../../com.aspose.cells/font)
### getLength() {#getLength--}
```
public int getLength()
```


Karakterlerin uzunluğunu alır.

**Returns:**
int
### getParentNode() {#getParentNode--}
```
public EquationNode getParentNode()
```


Geçerli düğümün üst düğümünü belirtir.

**Returns:**
[EquationNode](../../com.aspose.cells/equationnode)
### getStartIndex() {#getStartIndex--}
```
public int getStartIndex()
```


Karakterlerin başlangıç indeksini alır.

**Returns:**
int
### getTextOptions() {#getTextOptions--}
```
public TextOptions getTextOptions()
```


Metin seçeneklerini döndürür.

**Returns:**
[TextOptions](../../com.aspose.cells/textoptions)
### getType() {#getType--}
```
public int getType()
```


Düğümün türünü temsil eder.

Bkz. [TextNodeType](../../com.aspose.cells/textnodetype).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### insertAfter(int equationType) {#insertAfter-int-}
```
public EquationNode insertAfter(int equationType)
```


Belirtilen düğümü geçerli düğümün sonrasına ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| equationType | int | [EquationNodeType](../../com.aspose.cells/equationnodetype). Denklem Düğümlerinin Türleri |

**Returns:**
[EquationNode](../../com.aspose.cells/equationnode) - If the specified type exists, the corresponding node is returned, and if the type does not exist, a node of unknown type is returned.
### insertBefore(int equationType) {#insertBefore-int-}
```
public EquationNode insertBefore(int equationType)
```


Belirtilen düğümü geçerli düğümün önüne ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| equationType | int | [EquationNodeType](../../com.aspose.cells/equationnodetype). Denklem Düğümlerinin Türleri |

**Returns:**
[EquationNode](../../com.aspose.cells/equationnode) - If the specified type exists, the corresponding node is returned, and if the type does not exist, a node of unknown type is returned.
### insertChild(int index, int equationType) {#insertChild-int-int-}
```
public EquationNode insertChild(int index, int equationType)
```


Belirtilen tipte bir düğümü, geçerli düğümün alt düğüm listesinde belirtilen indeks konumuna ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | indeks değeri |
| equationType | int | [EquationNodeType](../../com.aspose.cells/equationnodetype). Denklem Düğümlerinin Türleri |

**Returns:**
[EquationNode](../../com.aspose.cells/equationnode) - If the specified type exists, the corresponding node is returned, and if the type does not exist, a node of unknown type is returned.
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### remove() {#remove--}
```
public void remove()
```


Kendisini üst düğümden kaldırır.

### removeAllChildren() {#removeAllChildren--}
```
public void removeAllChildren()
```


Geçerli düğümün tüm alt düğümlerini kaldırır.

### removeChild(EquationNode node) {#removeChild-com.aspose.cells.EquationNode-}
```
public void removeChild(EquationNode node)
```


Belirtilen düğümü, geçerli düğümün alt düğümlerinden kaldırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| node | [EquationNode](../../com.aspose.cells/equationnode) | Silinecek düğüm. |

### removeChild(int index) {#removeChild-int-}
```
public void removeChild(int index)
```


Belirtilen indeksteki düğümü, geçerli düğümün alt düğümlerinden kaldırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | Düğümün indeksi |

### setParentNode(EquationNode value) {#setParentNode-com.aspose.cells.EquationNode-}
```
public void setParentNode(EquationNode value)
```


Geçerli düğümün üst düğümünü belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [EquationNode](../../com.aspose.cells/equationnode) |  |

### setWordArtStyle(int style) {#setWordArtStyle-int-}
```
public void setWordArtStyle(int style)
```


Önceden ayarlanmış WordArt stilini ayarlar.

**Remarks**

Yalnızca şekil/grafik metni için.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| style | int | [PresetWordArtStyle](../../com.aspose.cells/presetwordartstyle). Önceden ayarlanmış WordArt stili. |

### toLaTeX() {#toLaTeX--}
```
public String toLaTeX()
```


Bu denklemi LaTeX ifadesine dönüştür.

**Returns:**
java.lang.String
### toMathML() {#toMathML--}
```
public String toMathML()
```


Bu denklemi MathML ifadesine dönüştür.

**Returns:**
java.lang.String -
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

