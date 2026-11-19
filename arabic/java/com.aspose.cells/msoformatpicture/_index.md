---
title: "MsoFormatPicture"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل تنسيق الصورة."
type: docs
url: /ar/java/com.aspose.cells/msoformatpicture/
---

**Inheritance:**
java.lang.Object
```
public class MsoFormatPicture
```

يمثل تنسيق الصورة.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) |  |
| [getBottomCrop()](#getBottomCrop--) | يمثل موقع الجزء السفلي من مستطيل القص، معبرًا عنه كنسبة من ارتفاع الصورة. |
| [getBottomCropInch()](#getBottomCropInch--) | يمثل موقع الجزء السفلي من مستطيل القص، بوحدة البوصة. |
| [getBrightness()](#getBrightness--) | يمثل تعديل السطوع للصورة بوحدة النسبة المئوية. |
| [getClass()](#getClass--) |  |
| [getContrast()](#getContrast--) | يمثل تعديل التباين للصورة بوحدة النسبة المئوية. |
| [getGamma()](#getGamma--) | يمثل قيمة غاما للصورة. |
| [getLeftCrop()](#getLeftCrop--) | يمثل موقع الجانب الأيسر من مستطيل القص، معبرًا عنه كنسبة من عرض الصورة. |
| [getLeftCropInch()](#getLeftCropInch--) | يمثل موقع الجانب الأيسر من مستطيل القص، بوحدة البوصة. |
| [getRightCrop()](#getRightCrop--) | يمثل موقع الجانب الأيمن من مستطيل القص، معبرًا عنه كنسبة من عرض الصورة. |
| [getRightCropInch()](#getRightCropInch--) | يمثل موقع الجانب الأيمن من مستطيل القص، بوحدة البوصة. |
| [getTopCrop()](#getTopCrop--) | يمثل موقع الجزء العلوي من مستطيل القص، معبرًا عنه كنسبة من ارتفاع الصورة. |
| [getTopCropInch()](#getTopCropInch--) | يمثل موقع الجزء العلوي من مستطيل القص، بوحدة البوصة. |
| [getTransparency()](#getTransparency--) | يرجع أو يضبط درجة شفافية المنطقة كقيمة من 0.0 (معتم) إلى 1.0 (شفاف). |
| [getTransparentColor()](#getTransparentColor--) | يحصل على اللون الشفاف للصورة. |
| [hashCode()](#hashCode--) | يحصل على رمز التجزئة. |
| [isBiLevel()](#isBiLevel--) | يشير إلى ما إذا كان يجب عرض هذه الصورة بالأبيض والأسود ثنائي اللون. |
| [isGray()](#isGray--) | يشير إلى ما إذا كان يجب عرض هذه الصورة بدرجات الرمادي. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBiLevel(boolean value)](#setBiLevel-boolean-) | يشير إلى ما إذا كان يجب عرض هذه الصورة بالأبيض والأسود ثنائي اللون. |
| [setBottomCrop(double value)](#setBottomCrop-double-) | يمثل موقع الجزء السفلي من مستطيل القص، معبرًا عنه كنسبة من ارتفاع الصورة. |
| [setBottomCropInch(double value)](#setBottomCropInch-double-) | يمثل موقع الجزء السفلي من مستطيل القص، بوحدة البوصة. |
| [setBrightness(double value)](#setBrightness-double-) | يمثل تعديل السطوع للصورة بوحدة النسبة المئوية. |
| [setContrast(double value)](#setContrast-double-) | يمثل تعديل التباين للصورة بوحدة النسبة المئوية. |
| [setGamma(double value)](#setGamma-double-) | يمثل قيمة غاما للصورة. |
| [setGray(boolean value)](#setGray-boolean-) | يشير إلى ما إذا كان يجب عرض هذه الصورة بدرجات الرمادي. |
| [setLeftCrop(double value)](#setLeftCrop-double-) | يمثل موقع الجانب الأيسر من مستطيل القص، معبرًا عنه كنسبة من عرض الصورة. |
| [setLeftCropInch(double value)](#setLeftCropInch-double-) | يمثل موقع الجانب الأيسر من مستطيل القص، بوحدة البوصة. |
| [setRightCrop(double value)](#setRightCrop-double-) | يمثل موقع الجانب الأيمن من مستطيل القص، معبرًا عنه كنسبة من عرض الصورة. |
| [setRightCropInch(double value)](#setRightCropInch-double-) | يمثل موقع الجانب الأيمن من مستطيل القص، بوحدة البوصة. |
| [setTopCrop(double value)](#setTopCrop-double-) | يمثل موقع الجزء العلوي من مستطيل القص، معبرًا عنه كنسبة من ارتفاع الصورة. |
| [setTopCropInch(double value)](#setTopCropInch-double-) | يمثل موقع الجزء العلوي من مستطيل القص، بوحدة البوصة. |
| [setTransparency(double value)](#setTransparency-double-) | يرجع أو يضبط درجة شفافية المنطقة كقيمة من 0.0 (معتم) إلى 1.0 (شفاف). |
| [setTransparentColor(CellsColor value)](#setTransparentColor-com.aspose.cells.CellsColor-) | يضبط اللون الشفاف للصورة. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| obj | java.lang.Object |  |

**Returns:**
boolean -
### getBottomCrop() {#getBottomCrop--}
```
public double getBottomCrop()
```


يمثل موقع الجزء السفلي من مستطيل القص، معبرًا عنه كنسبة من ارتفاع الصورة.

**Returns:**
double
### getBottomCropInch() {#getBottomCropInch--}
```
public double getBottomCropInch()
```


يمثل موقع الجزء السفلي من مستطيل القص، بوحدة البوصة.

**Returns:**
double
### getBrightness() {#getBrightness--}
```
public double getBrightness()
```


يمثل تعديل السطوع للصورة بوحدة النسبة المئوية.

**Remarks**

القيمة بين -100٪ و 100٪. تعمل بنفس طريقة Excel 2007 أو الإصدارات الأحدث.

**Returns:**
double
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getContrast() {#getContrast--}
```
public double getContrast()
```


يمثل تعديل التباين للصورة بوحدة النسبة المئوية.

**Remarks**

القيمة بين -100٪ و 100٪. تعمل بنفس طريقة Excel 2007 أو الإصدارات الأحدث.

**Returns:**
double
### getGamma() {#getGamma--}
```
public double getGamma()
```


يمثل قيمة غاما للصورة.

**Returns:**
double
### getLeftCrop() {#getLeftCrop--}
```
public double getLeftCrop()
```


يمثل موقع الجانب الأيسر من مستطيل القص، معبرًا عنه كنسبة من عرض الصورة.

**Returns:**
double
### getLeftCropInch() {#getLeftCropInch--}
```
public double getLeftCropInch()
```


يمثل موقع الجانب الأيسر من مستطيل القص، بوحدة البوصة.

**Returns:**
double
### getRightCrop() {#getRightCrop--}
```
public double getRightCrop()
```


يمثل موقع الجانب الأيمن من مستطيل القص، معبرًا عنه كنسبة من عرض الصورة.

**Returns:**
double
### getRightCropInch() {#getRightCropInch--}
```
public double getRightCropInch()
```


يمثل موقع الجانب الأيمن من مستطيل القص، بوحدة البوصة.

**Returns:**
double
### getTopCrop() {#getTopCrop--}
```
public double getTopCrop()
```


يمثل موقع الجزء العلوي من مستطيل القص، معبرًا عنه كنسبة من ارتفاع الصورة.

**Returns:**
double
### getTopCropInch() {#getTopCropInch--}
```
public double getTopCropInch()
```


يمثل موقع الجزء العلوي من مستطيل القص، بوحدة البوصة.

**Returns:**
double
### getTransparency() {#getTransparency--}
```
public double getTransparency()
```


يرجع أو يضبط درجة شفافية المنطقة كقيمة من 0.0 (معتم) إلى 1.0 (شفاف).

**Returns:**
double
### getTransparentColor() {#getTransparentColor--}
```
public CellsColor getTransparentColor()
```


يحصل على اللون الشفاف للصورة.

**Returns:**
[CellsColor](../../com.aspose.cells/cellscolor)
### hashCode() {#hashCode--}
```
public int hashCode()
```


يحصل على رمز التجزئة.

**Returns:**
int -
### isBiLevel() {#isBiLevel--}
```
public boolean isBiLevel()
```


يشير إلى ما إذا كان يجب عرض هذه الصورة بالأبيض والأسود ثنائي اللون.

**Returns:**
boolean
### isGray() {#isGray--}
```
public boolean isGray()
```


يشير إلى ما إذا كان يجب عرض هذه الصورة بدرجات الرمادي.

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




### setBiLevel(boolean value) {#setBiLevel-boolean-}
```
public void setBiLevel(boolean value)
```


يشير إلى ما إذا كان يجب عرض هذه الصورة بالأبيض والأسود ثنائي اللون.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setBottomCrop(double value) {#setBottomCrop-double-}
```
public void setBottomCrop(double value)
```


يمثل موقع الجزء السفلي من مستطيل القص، معبرًا عنه كنسبة من ارتفاع الصورة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setBottomCropInch(double value) {#setBottomCropInch-double-}
```
public void setBottomCropInch(double value)
```


يمثل موقع الجزء السفلي من مستطيل القص، بوحدة البوصة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setBrightness(double value) {#setBrightness-double-}
```
public void setBrightness(double value)
```


يمثل تعديل السطوع للصورة بوحدة النسبة المئوية.

**Remarks**

القيمة بين -100٪ و 100٪. تعمل بنفس طريقة Excel 2007 أو الإصدارات الأحدث.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setContrast(double value) {#setContrast-double-}
```
public void setContrast(double value)
```


يمثل تعديل التباين للصورة بوحدة النسبة المئوية.

**Remarks**

القيمة بين -100٪ و 100٪. تعمل بنفس طريقة Excel 2007 أو الإصدارات الأحدث.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setGamma(double value) {#setGamma-double-}
```
public void setGamma(double value)
```


يمثل قيمة غاما للصورة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setGray(boolean value) {#setGray-boolean-}
```
public void setGray(boolean value)
```


يشير إلى ما إذا كان يجب عرض هذه الصورة بدرجات الرمادي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setLeftCrop(double value) {#setLeftCrop-double-}
```
public void setLeftCrop(double value)
```


يمثل موقع الجانب الأيسر من مستطيل القص، معبرًا عنه كنسبة من عرض الصورة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setLeftCropInch(double value) {#setLeftCropInch-double-}
```
public void setLeftCropInch(double value)
```


يمثل موقع الجانب الأيسر من مستطيل القص، بوحدة البوصة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setRightCrop(double value) {#setRightCrop-double-}
```
public void setRightCrop(double value)
```


يمثل موقع الجانب الأيمن من مستطيل القص، معبرًا عنه كنسبة من عرض الصورة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setRightCropInch(double value) {#setRightCropInch-double-}
```
public void setRightCropInch(double value)
```


يمثل موقع الجانب الأيمن من مستطيل القص، بوحدة البوصة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setTopCrop(double value) {#setTopCrop-double-}
```
public void setTopCrop(double value)
```


يمثل موقع الجزء العلوي من مستطيل القص، معبرًا عنه كنسبة من ارتفاع الصورة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setTopCropInch(double value) {#setTopCropInch-double-}
```
public void setTopCropInch(double value)
```


يمثل موقع الجزء العلوي من مستطيل القص، بوحدة البوصة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setTransparency(double value) {#setTransparency-double-}
```
public void setTransparency(double value)
```


يرجع أو يضبط درجة شفافية المنطقة كقيمة من 0.0 (معتم) إلى 1.0 (شفاف).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setTransparentColor(CellsColor value) {#setTransparentColor-com.aspose.cells.CellsColor-}
```
public void setTransparentColor(CellsColor value)
```


يضبط اللون الشفاف للصورة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [CellsColor](../../com.aspose.cells/cellscolor) |  |

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
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

