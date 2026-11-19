---
title: "VbaProjectReferenceCollection"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل جميع مراجع مشروع VBA."
type: docs
url: /ar/java/com.aspose.cells/vbaprojectreferencecollection/
---

**Inheritance:**
java.lang.Object، [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class VbaProjectReferenceCollection extends CollectionBase
```

يمثل جميع مراجع مشروع VBA.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
          // Init VBA project.
         VbaProject vbaProject = workbook.getVbaProject();
         // Add vba project reference
         vbaProject.getReferences().addRegisteredReference("stdole", "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");
         //Saving the Excel file
         workbook.save("book1.xlsm");
```
## الطرق

| طريقة | الوصف |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | يضيف عنصرًا إلى مثيل CollectionBase. |
| [addControlReferernce(String name, String libid, String twiddledlibid, String extendedLibid)](#addControlReferernce-java.lang.String-java.lang.String-java.lang.String-java.lang.String-) | أضف مرجعًا إلى مكتبة نوع مُعدَّلة ومكتبة النوع الموسعة الخاصة بها. |
| [addControlRefrernce(String name, String libid, String twiddledlibid, String extendedLibid)](#addControlRefrernce-java.lang.String-java.lang.String-java.lang.String-java.lang.String-) | أضف مرجعًا إلى مكتبة نوع مُعدَّلة ومكتبة النوع الموسعة الخاصة بها. |
| [addProjectReferernce(String name, String absoluteLibid, String relativeLibid)](#addProjectReferernce-java.lang.String-java.lang.String-java.lang.String-) | يضيف مرجعًا إلى مشروع VBA خارجي. |
| [addProjectRefrernce(String name, String absoluteLibid, String relativeLibid)](#addProjectRefrernce-java.lang.String-java.lang.String-java.lang.String-) | يضيف مرجعًا إلى مشروع VBA خارجي. |
| [addRegisteredReference(String name, String libid)](#addRegisteredReference-java.lang.String-java.lang.String-) | أضف مرجعًا إلى مكتبة نوع Automation. |
| [clear()](#clear--) | يزيل جميع الكائنات من مثيل CollectionBase. |
| [contains(Object o)](#contains-java.lang.Object-) | إرجاع ما إذا كان المثيل يحتوي على هذا الكائن |
| [copy(VbaProjectReferenceCollection source)](#copy-com.aspose.cells.VbaProjectReferenceCollection-) | ينسخ المراجع من مشروع VBA آخر. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int i)](#get-int-) | احصل على المرجع في القائمة حسب الفهرس. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | يحصل على عدد العناصر الموجودة في مثيل CollectionBase. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | يحدد فهرس عنصر محدد في مثيل CollectionBase. |
| [iterator()](#iterator--) | يرجع كائن تعداد يتنقل عبر مثيل CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | يزيل العنصر في الفهرس المحدد. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


يضيف عنصرًا إلى مثيل CollectionBase.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| o | java.lang.Object | الكائن لإضافته إلى مثيل CollectionBase. |

**Returns:**
int - الموضع الذي تم إدراج العنصر الجديد فيه.
### addControlReferernce(String name, String libid, String twiddledlibid, String extendedLibid) {#addControlReferernce-java.lang.String-java.lang.String-java.lang.String-java.lang.String-}
```
public int addControlReferernce(String name, String libid, String twiddledlibid, String extendedLibid)
```


أضف مرجعًا إلى مكتبة نوع مُعدَّلة ومكتبة النوع الموسعة الخاصة بها.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| name | java.lang.String | اسم المرجع. |
| libid | java.lang.String | معرّف مكتبة نوع Automation. |
| twiddledlibid | java.lang.String | معرّف مكتبة النوع المُعدَّلة |
| extendedLibid | java.lang.String | معرّف مكتبة النوع الموسعة |

**Returns:**
int -
### addControlRefrernce(String name, String libid, String twiddledlibid, String extendedLibid) {#addControlRefrernce-java.lang.String-java.lang.String-java.lang.String-java.lang.String-}
```
public int addControlRefrernce(String name, String libid, String twiddledlibid, String extendedLibid)
```


أضف مرجعًا إلى مكتبة نوع مُعدَّلة ومكتبة النوع الموسعة الخاصة بها.

**Remarks**

ملاحظة: هذه الطريقة الآن غير صالحة. بدلاً من ذلك، يرجى استخدام طريقة VbaProjectReferenceCollection.AddControlReferernce(). سيتم إزالة هذه الطريقة بعد 12 شهرًا اعتبارًا من يوليو 2026. تعتذر Aspise عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| name | java.lang.String | اسم المرجع. |
| libid | java.lang.String | معرّف مكتبة نوع Automation. |
| twiddledlibid | java.lang.String | معرّف مكتبة النوع المُعدَّلة |
| extendedLibid | java.lang.String | معرّف مكتبة النوع الموسعة |

**Returns:**
int -
### addProjectReferernce(String name, String absoluteLibid, String relativeLibid) {#addProjectReferernce-java.lang.String-java.lang.String-java.lang.String-}
```
public int addProjectReferernce(String name, String absoluteLibid, String relativeLibid)
```


يضيف مرجعًا إلى مشروع VBA خارجي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| name | java.lang.String | اسم المرجع. |
| absoluteLibid | java.lang.String | معرّف مشروع VBA المشار إليه بمسار مطلق. |
| relativeLibid | java.lang.String | معرّف مشروع VBA المشار إليه بمسار نسبي. |

**Returns:**
int -
### addProjectRefrernce(String name, String absoluteLibid, String relativeLibid) {#addProjectRefrernce-java.lang.String-java.lang.String-java.lang.String-}
```
public int addProjectRefrernce(String name, String absoluteLibid, String relativeLibid)
```


يضيف مرجعًا إلى مشروع VBA خارجي.

**Remarks**

ملاحظة: هذه الطريقة الآن غير صالحة. بدلاً من ذلك، يرجى استخدام طريقة VbaProjectReferenceCollection.AddProjectReferernce(). سيتم إزالة هذه الطريقة بعد 12 شهرًا اعتبارًا من يوليو 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| name | java.lang.String | اسم المرجع. |
| absoluteLibid | java.lang.String | معرّف مشروع VBA المشار إليه بمسار مطلق. |
| relativeLibid | java.lang.String | معرّف مشروع VBA المشار إليه بمسار نسبي. |

**Returns:**
int -
### addRegisteredReference(String name, String libid) {#addRegisteredReference-java.lang.String-java.lang.String-}
```
public int addRegisteredReference(String name, String libid)
```


أضف مرجعًا إلى مكتبة نوع Automation.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| name | java.lang.String | اسم المرجع. |
| libid | java.lang.String | معرّف مكتبة نوع Automation. |

**Returns:**
int -
### clear() {#clear--}
```
public void clear()
```


يزيل جميع الكائنات من مثيل CollectionBase.

### contains(Object o) {#contains-java.lang.Object-}
```
public boolean contains(Object o)
```


إرجاع ما إذا كان المثيل يحتوي على هذا الكائن

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| o | java.lang.Object | كائن اختبار |

**Returns:**
boolean - ما إذا كان المثيل يحتوي على هذا الكائن
### copy(VbaProjectReferenceCollection source) {#copy-com.aspose.cells.VbaProjectReferenceCollection-}
```
public void copy(VbaProjectReferenceCollection source)
```


ينسخ المراجع من مشروع VBA آخر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| source | [VbaProjectReferenceCollection](../../com.aspose.cells/vbaprojectreferencecollection) | المراجع المصدر. |

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
### get(int i) {#get-int-}
```
public VbaProjectReference get(int i)
```


احصل على المرجع في القائمة حسب الفهرس.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| i | int | الفهرس. |

**Returns:**
[VbaProjectReference](../../com.aspose.cells/vbaprojectreference) - 
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCount() {#getCount--}
```
public int getCount()
```


يحصل على عدد العناصر الموجودة في مثيل CollectionBase.

**Returns:**
int - عدد العناصر الموجودة في مثيل CollectionBase.
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public int indexOf(Object o)
```


يحدد فهرس عنصر محدد في مثيل CollectionBase.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| o | java.lang.Object | يحدد فهرس عنصر محدد في مثيل CollectionBase. |

**Returns:**
int - فهرس القيمة إذا وجد في القائمة؛ وإلا -1.
### iterator() {#iterator--}
```
public Iterator iterator()
```


يرجع كائن تعداد يتنقل عبر مثيل CollectionBase.

**Returns:**
java.util.Iterator - كائن تكرار لمثيل CollectionBase.
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


يزيل العنصر في الفهرس المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | الفهرس الصفري للعنصر المراد إزالته. |

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

