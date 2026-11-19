---
title: "ErrorCheckOption"
second_title: "Aspose.Cells for Java API Reference"
description: "إعداد فحص الأخطاء المطبق على نطاقات معينة."
type: docs
url: /ar/java/com.aspose.cells/errorcheckoption/
---

**Inheritance:**
java.lang.Object
```
public class ErrorCheckOption
```

إعداد فحص الأخطاء المطبق على نطاقات معينة.

**Example**

```
           Workbook workbook = new Workbook();
           ErrorCheckOptionCollection opts = workbook.getWorksheets().get(0).getErrorCheckOptions();
           int optionIdx = opts.add();
           ErrorCheckOption opt = opts.get(optionIdx);
           opt.setErrorCheck(com.aspose.cells.ErrorCheckType.INCONSIST_FORMULA, false);
           opt.setErrorCheck(com.aspose.cells.ErrorCheckType.INCONSIST_RANGE, false);
           opt.setErrorCheck(com.aspose.cells.ErrorCheckType.TEXT_DATE, false);
           opt.setErrorCheck(com.aspose.cells.ErrorCheckType.TEXT_NUMBER, false);
           opt.setErrorCheck(com.aspose.cells.ErrorCheckType.VALIDATION, false);
           opt.addRange(CellArea.createCellArea("A1", "B10"));
           workbook.save("Book1.xlsx");
```
## الطرق

| طريقة | الوصف |
| --- | --- |
| [addRange(CellArea ca)](#addRange-com.aspose.cells.CellArea-) | يضيف نطاقًا متأثرًا واحدًا بواسطة هذا الإعداد. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getCountOfRange()](#getCountOfRange--) | يحصل على عدد النطاقات التي تأثرت بهذا الإعداد. |
| [getRange(int index)](#getRange-int-) | يحصل على النطاق المتأثر لهذا الإعداد حسب الفهرس المعطى. |
| [hashCode()](#hashCode--) |  |
| [isErrorCheck(int errorCheckType)](#isErrorCheck-int-) | يتحقق مما إذا كان نوع الخطأ المعطى سيُفحص. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeRange(int index)](#removeRange-int-) | يزيل نطاقًا واحدًا حسب الفهرس المعطى. |
| [setErrorCheck(int errorCheckType, boolean isCheck)](#setErrorCheck-int-boolean-) | يضبط ما إذا كان نوع الخطأ المعطى سيُفحص. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addRange(CellArea ca) {#addRange-com.aspose.cells.CellArea-}
```
public int addRange(CellArea ca)
```


يضيف نطاقًا متأثرًا واحدًا بواسطة هذا الإعداد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | النطاق المراد إضافته. |

**Returns:**
int - الفهرس للنطاق المضاف في قائمة النطاقات لهذا الإعداد.
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| معامل | نوع | الوصف |
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
### getCountOfRange() {#getCountOfRange--}
```
public int getCountOfRange()
```


يحصل على عدد النطاقات التي تأثرت بهذا الإعداد.

**Returns:**
int - عدد النطاقات التي تأثرت بهذا الإعداد.
### getRange(int index) {#getRange-int-}
```
public CellArea getRange(int index)
```


يحصل على النطاق المتأثر لهذا الإعداد حسب الفهرس المعطى.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | فهرس النطاق |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - return influenced range at given index.
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isErrorCheck(int errorCheckType) {#isErrorCheck-int-}
```
public boolean isErrorCheck(int errorCheckType)
```


يتحقق مما إذا كان نوع الخطأ المعطى سيُفحص.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| errorCheckType | int | [ErrorCheckType](../../com.aspose.cells/errorchecktype). يمكن فحص نوع الخطأ |

**Returns:**
boolean - إرجاع true إذا تم فحص نوع الخطأ المعطى (سيظهر مثلث أخضر للخلية إذا فشل الفحص).
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### removeRange(int index) {#removeRange-int-}
```
public void removeRange(int index)
```


يزيل نطاقًا واحدًا حسب الفهرس المعطى.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | فهرس النطاق الذي سيتم إزالته. |

### setErrorCheck(int errorCheckType, boolean isCheck) {#setErrorCheck-int-boolean-}
```
public void setErrorCheck(int errorCheckType, boolean isCheck)
```


يضبط ما إذا كان نوع الخطأ المعطى سيُفحص.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| errorCheckType | int | [ErrorCheckType](../../com.aspose.cells/errorchecktype). يمكن فحص نوع الخطأ. |
| isCheck | boolean | true إذا كان نوع الخطأ المعطى يحتاج إلى الفحص (سيظهر مثلث أخضر للخلية إذا فشل الفحص). |

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

