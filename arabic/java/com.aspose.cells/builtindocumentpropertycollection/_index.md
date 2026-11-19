---
title: "BuiltInDocumentPropertyCollection"
second_title: "Aspose.Cells for Java API Reference"
description: "مجموعة من خصائص المستند المدمجة."
type: docs
url: /ar/java/com.aspose.cells/builtindocumentpropertycollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase), [com.aspose.cells.DocumentPropertyCollection](../../com.aspose.cells/documentpropertycollection)
```
public class BuiltInDocumentPropertyCollection extends DocumentPropertyCollection
```

مجموعة من خصائص المستند المدمجة.

**Remarks**

يوفر الوصول إلى الكائنات بأسمائها (باستخدام الفهرس) ومن خلال مجموعة من الخصائص المكتوبة التي تُعيد قيم الأنواع المناسبة.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | يضيف عنصرًا إلى مثيل CollectionBase. |
| [clear()](#clear--) | يزيل جميع الكائنات من مثيل CollectionBase. |
| [contains(Object o)](#contains-java.lang.Object-) | إرجاع ما إذا كان المثيل يحتوي على هذا الكائن |
| [contains(String name)](#contains-java.lang.String-) | يرجع true إذا كان هناك خاصية بالاسم المحدد موجودة في المجموعة. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | يرجع كائن [DocumentProperty](../../com.aspose.cells/documentproperty) حسب الفهرس. |
| [get(String name)](#get-java.lang.String-) | يرجع كائن [DocumentProperty](../../com.aspose.cells/documentproperty) حسب اسم الخاصية. |
| [getAuthor()](#getAuthor--) | يحصل على اسم مؤلف المستند. |
| [getBytes()](#getBytes--) | يمثل تقديرًا لعدد البايتات في المستند. |
| [getCategory()](#getCategory--) | يحصل على فئة المستند. |
| [getCharacters()](#getCharacters--) | يمثل تقديرًا لعدد الأحرف في المستند. |
| [getCharactersWithSpaces()](#getCharactersWithSpaces--) | يمثل تقديرًا لعدد الأحرف (بما في ذلك المسافات) في المستند. |
| [getClass()](#getClass--) |  |
| [getComments()](#getComments--) | يحصل على تعليقات المستند. |
| [getCompany()](#getCompany--) | يحصل على خاصية الشركة. |
| [getContentStatus()](#getContentStatus--) | يحصل على حالة محتوى المستند. |
| [getContentType()](#getContentType--) | يحصل على نوع محتوى المستند. |
| [getCount()](#getCount--) | يحصل على عدد العناصر الموجودة في مثيل CollectionBase. |
| [getCreatedTime()](#getCreatedTime--) | يحصل على تاريخ إنشاء المستند بالتوقيت المحلي. |
| [getCreatedUniversalTime()](#getCreatedUniversalTime--) | يحصل على الوقت العالمي لإنشاء المستند. |
| [getDocumentVersion()](#getDocumentVersion--) | يمثل نسخة الملف. |
| [getHyperlinkBase()](#getHyperlinkBase--) | يحصل على خاصية قاعدة الارتباط التشعبي. |
| [getKeywords()](#getKeywords--) | يحصل على كلمات مفتاحية للمستند. |
| [getLanguage()](#getLanguage--) | يحصل على لغة المستند. |
| [getLastPrinted()](#getLastPrinted--) | يحصل على تاريخ آخر طباعة للمستند بالتوقيت المحلي. |
| [getLastPrintedUniversalTime()](#getLastPrintedUniversalTime--) | يحصل على الوقت العالمي عندما تم طباعة المستند آخر مرة. |
| [getLastSavedBy()](#getLastSavedBy--) | يحصل على اسم المؤلف الأخير. |
| [getLastSavedTime()](#getLastSavedTime--) | يحصل على وقت آخر حفظ بالتوقيت المحلي. |
| [getLastSavedUniversalTime()](#getLastSavedUniversalTime--) | يحصل على الوقت العالمي لآخر حفظ. |
| [getLines()](#getLines--) | يمثل تقديراً لعدد الأسطر في المستند. |
| [getLinksUpToDate()](#getLinksUpToDate--) | يشير إلى ما إذا كانت الروابط التشعبية في المستند محدثة. |
| [getManager()](#getManager--) | يحصل على خاصية المدير. |
| [getNameOfApplication()](#getNameOfApplication--) | يحصل على اسم التطبيق. |
| [getPages()](#getPages--) | يمثل تقديراً لعدد الصفحات في المستند. |
| [getParagraphs()](#getParagraphs--) | يمثل تقديراً لعدد الفقرات في المستند. |
| [getRevisionNumber()](#getRevisionNumber--) | يحصل على رقم مراجعة المستند. |
| [getScaleCrop()](#getScaleCrop--) | يشير إلى وضع عرض صورة المصغرة للمستند. |
| [getSubject()](#getSubject--) | يحصل على موضوع المستند. |
| [getTemplate()](#getTemplate--) | يحصل على الاسم المعلوماتي لقالب المستند. |
| [getTitle()](#getTitle--) | يحصل على عنوان المستند. |
| [getTotalEditingTime()](#getTotalEditingTime--) | يحصل على إجمالي وقت التحرير بالدقائق. |
| [getVersion()](#getVersion--) | يمثل رقم نسخة التطبيق الذي أنشأ المستند. |
| [getWords()](#getWords--) | يمثل تقديراً لعدد الكلمات في المستند. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | يحدد فهرس عنصر محدد في مثيل CollectionBase. |
| [indexOf(String name)](#indexOf-java.lang.String-) | يحصل على فهرس الخاصية حسب الاسم. |
| [iterator()](#iterator--) | يرجع كائن تعداد يتنقل عبر مثيل CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(String name)](#remove-java.lang.String-) | يزيل خاصية بالاسم المحدد من المجموعة. |
| [removeAt(int index)](#removeAt-int-) | يزيل خاصية عند الفهرس المحدد. |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | يضبط اسم مؤلف المستند. |
| [setBytes(int value)](#setBytes-int-) | يمثل تقديرًا لعدد البايتات في المستند. |
| [setCategory(String value)](#setCategory-java.lang.String-) | يضبط فئة المستند. |
| [setCharacters(int value)](#setCharacters-int-) | يمثل تقديرًا لعدد الأحرف في المستند. |
| [setCharactersWithSpaces(int value)](#setCharactersWithSpaces-int-) | يمثل تقديرًا لعدد الأحرف (بما في ذلك المسافات) في المستند. |
| [setComments(String value)](#setComments-java.lang.String-) | يضبط تعليقات المستند. |
| [setCompany(String value)](#setCompany-java.lang.String-) | يضبط خاصية الشركة. |
| [setContentStatus(String value)](#setContentStatus-java.lang.String-) | يضبط حالة محتوى المستند. |
| [setContentType(String value)](#setContentType-java.lang.String-) | يضبط نوع محتوى المستند. |
| [setCreatedTime(DateTime value)](#setCreatedTime-com.aspose.cells.DateTime-) | يضبط تاريخ إنشاء المستند بالتوقيت المحلي. |
| [setCreatedUniversalTime(DateTime value)](#setCreatedUniversalTime-com.aspose.cells.DateTime-) | يضبط الوقت العالمي لإنشاء المستند. |
| [setDocumentVersion(String value)](#setDocumentVersion-java.lang.String-) | يمثل نسخة الملف. |
| [setHyperlinkBase(String value)](#setHyperlinkBase-java.lang.String-) | يضبط خاصية قاعدة الروابط التشعبية. |
| [setKeywords(String value)](#setKeywords-java.lang.String-) | يضبط كلمات مفتاح المستند. |
| [setLanguage(String value)](#setLanguage-java.lang.String-) | يضبط لغة المستند. |
| [setLastPrinted(DateTime value)](#setLastPrinted-com.aspose.cells.DateTime-) | يضبط التاريخ عندما تم طباعة المستند آخر مرة في المنطقة الزمنية المحلية. |
| [setLastPrintedUniversalTime(DateTime value)](#setLastPrintedUniversalTime-com.aspose.cells.DateTime-) | يضبط الوقت العالمي عندما تم طباعة المستند آخر مرة. |
| [setLastSavedBy(String value)](#setLastSavedBy-java.lang.String-) | يضبط اسم المؤلف الأخير. |
| [setLastSavedTime(DateTime value)](#setLastSavedTime-com.aspose.cells.DateTime-) | يضبط وقت الحفظ الأخير في المنطقة الزمنية المحلية. |
| [setLastSavedUniversalTime(DateTime value)](#setLastSavedUniversalTime-com.aspose.cells.DateTime-) | يضبط الوقت العالمي للحفظ الأخير. |
| [setLines(int value)](#setLines-int-) | يمثل تقديراً لعدد الأسطر في المستند. |
| [setLinksUpToDate(boolean value)](#setLinksUpToDate-boolean-) | يشير إلى ما إذا كانت الروابط التشعبية في المستند محدثة. |
| [setManager(String value)](#setManager-java.lang.String-) | يضبط خاصية المدير. |
| [setNameOfApplication(String value)](#setNameOfApplication-java.lang.String-) | يضبط اسم التطبيق. |
| [setPages(int value)](#setPages-int-) | يمثل تقديراً لعدد الصفحات في المستند. |
| [setParagraphs(int value)](#setParagraphs-int-) | يمثل تقديراً لعدد الفقرات في المستند. |
| [setRevisionNumber(String value)](#setRevisionNumber-java.lang.String-) | يضبط رقم مراجعة المستند. |
| [setScaleCrop(boolean value)](#setScaleCrop-boolean-) | يشير إلى وضع عرض صورة المصغرة للمستند. |
| [setSubject(String value)](#setSubject-java.lang.String-) | يضبط موضوع المستند. |
| [setTemplate(String value)](#setTemplate-java.lang.String-) | يضبط الاسم المعلوماتي لقالب المستند. |
| [setTitle(String value)](#setTitle-java.lang.String-) | يضبط عنوان المستند. |
| [setTotalEditingTime(double value)](#setTotalEditingTime-double-) | يضبط إجمالي وقت التحرير بالدقائق. |
| [setVersion(String value)](#setVersion-java.lang.String-) | يمثل رقم نسخة التطبيق الذي أنشأ المستند. |
| [setWords(int value)](#setWords-int-) | يمثل تقديراً لعدد الكلمات في المستند. |
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
### contains(String name) {#contains-java.lang.String-}
```
public boolean contains(String name)
```


يرجع true إذا كان هناك خاصية بالاسم المحدد موجودة في المجموعة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| name | java.lang.String | اسم الخاصية غير حساس لحالة الأحرف. |

**Returns:**
boolean - True إذا كانت الخاصية موجودة في المجموعة؛ false خلاف ذلك.
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
### get(int index) {#get-int-}
```
public DocumentProperty get(int index)
```


يرجع كائن [DocumentProperty](../../com.aspose.cells/documentproperty) حسب الفهرس.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| index | int | الفهرس الصفري لـ [DocumentProperty](../../com.aspose.cells/documentproperty) المراد استرجاعه. |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty)
### get(String name) {#get-java.lang.String-}
```
public DocumentProperty get(String name)
```


يرجع كائن [DocumentProperty](../../com.aspose.cells/documentproperty) حسب اسم الخاصية.

**Remarks**

أسماء السلاسل للخصائص تتطابق مع أسماء الخصائص المكتوبة المتاحة من .

إذا طلبت خاصية غير موجودة في المستند، ولكن اسم الخاصية تم التعرف عليه كاسم مدمج صالح، يتم إنشاء  جديد، يضاف إلى المجموعة ويُرجع. الخاصية التي تم إنشاؤها حديثًا تُعطى قيمة افتراضية (سلسلة فارغة، صفر، خطأ أو DateTime.MinValue حسب نوع الخاصية المدمجة).

إذا طلبت خاصية غير موجودة في المستند ولم يتم التعرف على الاسم كاسم مدمج، يتم إرجاع null.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| name | java.lang.String | اسم الخاصية غير حساس لحالة الأحرف المراد استرجاعه. |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty)
### getAuthor() {#getAuthor--}
```
public String getAuthor()
```


يحصل على اسم مؤلف المستند.

**Returns:**
java.lang.String
### getBytes() {#getBytes--}
```
public int getBytes()
```


يمثل تقديرًا لعدد البايتات في المستند.

**Returns:**
int
### getCategory() {#getCategory--}
```
public String getCategory()
```


يحصل على فئة المستند.

**Returns:**
java.lang.String
### getCharacters() {#getCharacters--}
```
public int getCharacters()
```


يمثل تقديرًا لعدد الأحرف في المستند.

**Returns:**
int
### getCharactersWithSpaces() {#getCharactersWithSpaces--}
```
public int getCharactersWithSpaces()
```


يمثل تقديرًا لعدد الأحرف (بما في ذلك المسافات) في المستند.

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getComments() {#getComments--}
```
public String getComments()
```


يحصل على تعليقات المستند.

**Returns:**
java.lang.String
### getCompany() {#getCompany--}
```
public String getCompany()
```


يحصل على خاصية الشركة.

**Returns:**
java.lang.String
### getContentStatus() {#getContentStatus--}
```
public String getContentStatus()
```


يحصل على حالة محتوى المستند.

**Returns:**
java.lang.String
### getContentType() {#getContentType--}
```
public String getContentType()
```


يحصل على نوع محتوى المستند.

**Returns:**
java.lang.String
### getCount() {#getCount--}
```
public int getCount()
```


يحصل على عدد العناصر الموجودة في مثيل CollectionBase.

**Returns:**
int - عدد العناصر الموجودة في مثيل CollectionBase.
### getCreatedTime() {#getCreatedTime--}
```
public DateTime getCreatedTime()
```


يحصل على تاريخ إنشاء المستند بالتوقيت المحلي.

**Remarks**

Aspose.Cells لا يقوم بتحديث هذه الخاصية عند تعديل المستند.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getCreatedUniversalTime() {#getCreatedUniversalTime--}
```
public DateTime getCreatedUniversalTime()
```


يحصل على الوقت العالمي لإنشاء المستند.

**Remarks**

Aspose.Cells لا يقوم بتحديث هذه الخاصية عند تعديل المستند.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getDocumentVersion() {#getDocumentVersion--}
```
public String getDocumentVersion()
```


يمثل نسخة الملف.

**Returns:**
java.lang.String
### getHyperlinkBase() {#getHyperlinkBase--}
```
public String getHyperlinkBase()
```


يحصل على خاصية قاعدة الارتباط التشعبي.

**Returns:**
java.lang.String
### getKeywords() {#getKeywords--}
```
public String getKeywords()
```


يحصل على كلمات مفتاحية للمستند.

**Returns:**
java.lang.String
### getLanguage() {#getLanguage--}
```
public String getLanguage()
```


يحصل على لغة المستند.

**Returns:**
java.lang.String
### getLastPrinted() {#getLastPrinted--}
```
public DateTime getLastPrinted()
```


يحصل على تاريخ آخر طباعة للمستند بالتوقيت المحلي.

**Remarks**

إذا لم يتم طباعة المستند مطلقًا، ستُرجع هذه الخاصية DateTime.MinValue.

Aspose.Cells لا يقوم بتحديث هذه الخاصية عند تعديل المستند.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getLastPrintedUniversalTime() {#getLastPrintedUniversalTime--}
```
public DateTime getLastPrintedUniversalTime()
```


يحصل على الوقت العالمي عندما تم طباعة المستند آخر مرة.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getLastSavedBy() {#getLastSavedBy--}
```
public String getLastSavedBy()
```


يحصل على اسم المؤلف الأخير.

**Remarks**

Aspose.Cells لا يقوم بتحديث هذه الخاصية عند تعديل المستند.

**Returns:**
java.lang.String
### getLastSavedTime() {#getLastSavedTime--}
```
public DateTime getLastSavedTime()
```


يحصل على وقت آخر حفظ بالتوقيت المحلي.

**Remarks**

Aspose.Cells لا يقوم بتحديث هذه الخاصية عند تعديل المستند.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getLastSavedUniversalTime() {#getLastSavedUniversalTime--}
```
public DateTime getLastSavedUniversalTime()
```


يحصل على الوقت العالمي لآخر حفظ.

**Remarks**

Aspose.Cells لا يقوم بتحديث هذه الخاصية عند تعديل المستند.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getLines() {#getLines--}
```
public int getLines()
```


يمثل تقديراً لعدد الأسطر في المستند.

**Remarks**

Aspose.Cells لا يقوم بتحديث هذه الخاصية عند تعديل المستند.

**Returns:**
int
### getLinksUpToDate() {#getLinksUpToDate--}
```
public boolean getLinksUpToDate()
```


يشير إلى ما إذا كانت الروابط التشعبية في المستند محدثة.

**Returns:**
boolean
### getManager() {#getManager--}
```
public String getManager()
```


يحصل على خاصية المدير.

**Returns:**
java.lang.String
### getNameOfApplication() {#getNameOfApplication--}
```
public String getNameOfApplication()
```


يحصل على اسم التطبيق.

**Returns:**
java.lang.String
### getPages() {#getPages--}
```
public int getPages()
```


يمثل تقديراً لعدد الصفحات في المستند.

**Returns:**
int
### getParagraphs() {#getParagraphs--}
```
public int getParagraphs()
```


يمثل تقديراً لعدد الفقرات في المستند.

**Returns:**
int
### getRevisionNumber() {#getRevisionNumber--}
```
public String getRevisionNumber()
```


يحصل على رقم مراجعة المستند.

**Remarks**

Aspose.Cells لا يقوم بتحديث هذه الخاصية عند تعديل المستند.

**Returns:**
java.lang.String
### getScaleCrop() {#getScaleCrop--}
```
public boolean getScaleCrop()
```


يشير إلى وضع عرض صورة المصغرة للمستند.

**Returns:**
boolean
### getSubject() {#getSubject--}
```
public String getSubject()
```


يحصل على موضوع المستند.

**Returns:**
java.lang.String
### getTemplate() {#getTemplate--}
```
public String getTemplate()
```


يحصل على الاسم المعلوماتي لقالب المستند.

**Returns:**
java.lang.String
### getTitle() {#getTitle--}
```
public String getTitle()
```


يحصل على عنوان المستند.

**Returns:**
java.lang.String
### getTotalEditingTime() {#getTotalEditingTime--}
```
public double getTotalEditingTime()
```


يحصل على إجمالي وقت التحرير بالدقائق.

**Returns:**
double
### getVersion() {#getVersion--}
```
public String getVersion()
```


يمثل رقم نسخة التطبيق الذي أنشأ المستند.

**Remarks**

تنسيقها هو "00.0000"، على سبيل المثال: 12.0000

**Returns:**
java.lang.String
### getWords() {#getWords--}
```
public int getWords()
```


يمثل تقديراً لعدد الكلمات في المستند.

**Returns:**
int
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
### indexOf(String name) {#indexOf-java.lang.String-}
```
public int indexOf(String name)
```


يحصل على فهرس الخاصية حسب الاسم.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| name | java.lang.String | اسم الخاصية غير حساس لحالة الأحرف. |

**Returns:**
int - الفهرس القائم على الصفر. قيمة سالبة إذا لم يتم العثور عليه.
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




### remove(String name) {#remove-java.lang.String-}
```
public void remove(String name)
```


يزيل خاصية بالاسم المحدد من المجموعة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| name | java.lang.String | اسم الخاصية غير حساس لحالة الأحرف. |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


يزيل خاصية عند الفهرس المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | الفهرس القائم على الصفر. |

### setAuthor(String value) {#setAuthor-java.lang.String-}
```
public void setAuthor(String value)
```


يضبط اسم مؤلف المستند.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setBytes(int value) {#setBytes-int-}
```
public void setBytes(int value)
```


يمثل تقديرًا لعدد البايتات في المستند.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setCategory(String value) {#setCategory-java.lang.String-}
```
public void setCategory(String value)
```


يضبط فئة المستند.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setCharacters(int value) {#setCharacters-int-}
```
public void setCharacters(int value)
```


يمثل تقديرًا لعدد الأحرف في المستند.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setCharactersWithSpaces(int value) {#setCharactersWithSpaces-int-}
```
public void setCharactersWithSpaces(int value)
```


يمثل تقديرًا لعدد الأحرف (بما في ذلك المسافات) في المستند.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setComments(String value) {#setComments-java.lang.String-}
```
public void setComments(String value)
```


يضبط تعليقات المستند.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setCompany(String value) {#setCompany-java.lang.String-}
```
public void setCompany(String value)
```


يضبط خاصية الشركة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setContentStatus(String value) {#setContentStatus-java.lang.String-}
```
public void setContentStatus(String value)
```


يضبط حالة محتوى المستند.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setContentType(String value) {#setContentType-java.lang.String-}
```
public void setContentType(String value)
```


يضبط نوع محتوى المستند.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setCreatedTime(DateTime value) {#setCreatedTime-com.aspose.cells.DateTime-}
```
public void setCreatedTime(DateTime value)
```


يضبط تاريخ إنشاء المستند بالتوقيت المحلي.

**Remarks**

Aspose.Cells لا يقوم بتحديث هذه الخاصية عند تعديل المستند.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setCreatedUniversalTime(DateTime value) {#setCreatedUniversalTime-com.aspose.cells.DateTime-}
```
public void setCreatedUniversalTime(DateTime value)
```


يضبط الوقت العالمي لإنشاء المستند.

**Remarks**

Aspose.Cells لا يقوم بتحديث هذه الخاصية عند تعديل المستند.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setDocumentVersion(String value) {#setDocumentVersion-java.lang.String-}
```
public void setDocumentVersion(String value)
```


يمثل نسخة الملف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setHyperlinkBase(String value) {#setHyperlinkBase-java.lang.String-}
```
public void setHyperlinkBase(String value)
```


يضبط خاصية قاعدة الروابط التشعبية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setKeywords(String value) {#setKeywords-java.lang.String-}
```
public void setKeywords(String value)
```


يضبط كلمات مفتاح المستند.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setLanguage(String value) {#setLanguage-java.lang.String-}
```
public void setLanguage(String value)
```


يضبط لغة المستند.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setLastPrinted(DateTime value) {#setLastPrinted-com.aspose.cells.DateTime-}
```
public void setLastPrinted(DateTime value)
```


يضبط التاريخ عندما تم طباعة المستند آخر مرة في المنطقة الزمنية المحلية.

**Remarks**

إذا لم يتم طباعة المستند مطلقًا، ستُرجع هذه الخاصية DateTime.MinValue.

Aspose.Cells لا يقوم بتحديث هذه الخاصية عند تعديل المستند.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setLastPrintedUniversalTime(DateTime value) {#setLastPrintedUniversalTime-com.aspose.cells.DateTime-}
```
public void setLastPrintedUniversalTime(DateTime value)
```


يضبط الوقت العالمي عندما تم طباعة المستند آخر مرة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setLastSavedBy(String value) {#setLastSavedBy-java.lang.String-}
```
public void setLastSavedBy(String value)
```


يضبط اسم المؤلف الأخير.

**Remarks**

Aspose.Cells لا يقوم بتحديث هذه الخاصية عند تعديل المستند.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setLastSavedTime(DateTime value) {#setLastSavedTime-com.aspose.cells.DateTime-}
```
public void setLastSavedTime(DateTime value)
```


يضبط وقت الحفظ الأخير في المنطقة الزمنية المحلية.

**Remarks**

Aspose.Cells لا يقوم بتحديث هذه الخاصية عند تعديل المستند.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setLastSavedUniversalTime(DateTime value) {#setLastSavedUniversalTime-com.aspose.cells.DateTime-}
```
public void setLastSavedUniversalTime(DateTime value)
```


يضبط الوقت العالمي للحفظ الأخير.

**Remarks**

Aspose.Cells لا يقوم بتحديث هذه الخاصية عند تعديل المستند.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setLines(int value) {#setLines-int-}
```
public void setLines(int value)
```


يمثل تقديراً لعدد الأسطر في المستند.

**Remarks**

Aspose.Cells لا يقوم بتحديث هذه الخاصية عند تعديل المستند.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setLinksUpToDate(boolean value) {#setLinksUpToDate-boolean-}
```
public void setLinksUpToDate(boolean value)
```


يشير إلى ما إذا كانت الروابط التشعبية في المستند محدثة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setManager(String value) {#setManager-java.lang.String-}
```
public void setManager(String value)
```


يضبط خاصية المدير.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setNameOfApplication(String value) {#setNameOfApplication-java.lang.String-}
```
public void setNameOfApplication(String value)
```


يضبط اسم التطبيق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setPages(int value) {#setPages-int-}
```
public void setPages(int value)
```


يمثل تقديراً لعدد الصفحات في المستند.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setParagraphs(int value) {#setParagraphs-int-}
```
public void setParagraphs(int value)
```


يمثل تقديراً لعدد الفقرات في المستند.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setRevisionNumber(String value) {#setRevisionNumber-java.lang.String-}
```
public void setRevisionNumber(String value)
```


يضبط رقم مراجعة المستند.

**Remarks**

Aspose.Cells لا يقوم بتحديث هذه الخاصية عند تعديل المستند.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setScaleCrop(boolean value) {#setScaleCrop-boolean-}
```
public void setScaleCrop(boolean value)
```


يشير إلى وضع عرض صورة المصغرة للمستند.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setSubject(String value) {#setSubject-java.lang.String-}
```
public void setSubject(String value)
```


يضبط موضوع المستند.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setTemplate(String value) {#setTemplate-java.lang.String-}
```
public void setTemplate(String value)
```


يضبط الاسم المعلوماتي لقالب المستند.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setTitle(String value) {#setTitle-java.lang.String-}
```
public void setTitle(String value)
```


يضبط عنوان المستند.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setTotalEditingTime(double value) {#setTotalEditingTime-double-}
```
public void setTotalEditingTime(double value)
```


يضبط إجمالي وقت التحرير بالدقائق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setVersion(String value) {#setVersion-java.lang.String-}
```
public void setVersion(String value)
```


يمثل رقم نسخة التطبيق الذي أنشأ المستند.

**Remarks**

تنسيقها هو "00.0000"، على سبيل المثال: 12.0000

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setWords(int value) {#setWords-int-}
```
public void setWords(int value)
```


يمثل تقديراً لعدد الكلمات في المستند.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

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

