---
title: "PdfSecurityOptions"
second_title: "Aspose.Cells for Java API Reference"
description: "خيارات التشفير وأذونات الوصول لمستند PDF."
type: docs
url: /ar/java/com.aspose.cells/pdfsecurityoptions/
---

**Inheritance:**
java.lang.Object
```
public class PdfSecurityOptions
```

خيارات تشفير وإعدادات أذونات الوصول لمستند PDF. لا يسمح PDF/A بإعدادات الأمان.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [PdfSecurityOptions()](#PdfSecurityOptions--) | المُنشئ الخاص بـ PdfSecurityOptions |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAccessibilityExtractContent()](#getAccessibilityExtractContent--) | يُشير إلى ما إذا كان يُسمح باستخراج النص والرسومات (دعمًا لإمكانية الوصول للمستخدمين ذوي الإعاقة أو لأغراض أخرى). |
| [getAnnotationsPermission()](#getAnnotationsPermission--) | يُشير إلى ما إذا كان يُسمح بإضافة أو تعديل تعليقات النص، وملء حقول النماذج التفاعلية. |
| [getAssembleDocumentPermission()](#getAssembleDocumentPermission--) | يُشير إلى ما إذا كان يُسمح بتجميع المستند (إدراج، تدوير، أو حذف الصفحات وإنشاء إشارات مرجعية أو صور مصغرة)، حتى إذا كان [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\\#getModifyDocumentPermission--) واضحًا. |
| [getClass()](#getClass--) |  |
| [getExtractContentPermission()](#getExtractContentPermission--) | يُشير إلى ما إذا كان يُسمح بنسخ أو استخراج النص والرسومات من المستند بطرق أخرى غير تلك التي يتحكم فيها [getAccessibilityExtractContent()](../../com.aspose.cells/pdfsecurityoptions\\#getAccessibilityExtractContent--). |
| [getExtractContentPermissionObsolete()](#getExtractContentPermissionObsolete--) | إذن النسخ أو استخراج المحتوى تم إهماله وفقًا لمرجع PDF. |
| [getFillFormsPermission()](#getFillFormsPermission--) | يُشير إلى ما إذا كان يُسمح بملء حقول النماذج التفاعلية الموجودة (بما في ذلك حقول التوقيع)، حتى إذا كان [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\\#getModifyDocumentPermission--) واضحًا. |
| [getFullQualityPrintPermission()](#getFullQualityPrintPermission--) | يُشير إلى ما إذا كان يُسمح بطباعة المستند إلى تمثيل يمكن من خلاله إنشاء نسخة رقمية دقيقة من محتوى PDF. |
| [getModifyDocumentPermission()](#getModifyDocumentPermission--) | يُشير إلى ما إذا كان يُسمح بتعديل محتويات المستند بعمليات غير تلك التي يتحكم فيها [getAnnotationsPermission()](../../com.aspose.cells/pdfsecurityoptions\\#getAnnotationsPermission--)، [getFillFormsPermission()](../../com.aspose.cells/pdfsecurityoptions\\#getFillFormsPermission--) و [getAssembleDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\\#getAssembleDocumentPermission--). |
| [getOwnerPassword()](#getOwnerPassword--) | يحصل على كلمة مرور المالك لمستند PDF المشفر. |
| [getPrintPermission()](#getPrintPermission--) | يُشير إلى ما إذا كان يُسمح بطباعة المستند. |
| [getUserPassword()](#getUserPassword--) | يحصل على كلمة مرور المستخدم المطلوبة لفتح مستند PDF المشفر. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAccessibilityExtractContent(boolean value)](#setAccessibilityExtractContent-boolean-) | يُشير إلى ما إذا كان يُسمح باستخراج النص والرسومات (دعمًا لإمكانية الوصول للمستخدمين ذوي الإعاقة أو لأغراض أخرى). |
| [setAnnotationsPermission(boolean value)](#setAnnotationsPermission-boolean-) | يُشير إلى ما إذا كان يُسمح بإضافة أو تعديل تعليقات النص، وملء حقول النماذج التفاعلية. |
| [setAssembleDocumentPermission(boolean value)](#setAssembleDocumentPermission-boolean-) | يُشير إلى ما إذا كان يُسمح بتجميع المستند (إدراج، تدوير، أو حذف الصفحات وإنشاء إشارات مرجعية أو صور مصغرة)، حتى إذا كان [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\\#getModifyDocumentPermission--) واضحًا. |
| [setExtractContentPermission(boolean value)](#setExtractContentPermission-boolean-) | يُشير إلى ما إذا كان يُسمح بنسخ أو استخراج النص والرسومات من المستند بطرق أخرى غير تلك التي يتحكم فيها [getAccessibilityExtractContent()](../../com.aspose.cells/pdfsecurityoptions\\#getAccessibilityExtractContent--). |
| [setExtractContentPermissionObsolete(boolean value)](#setExtractContentPermissionObsolete-boolean-) | إذن النسخ أو استخراج المحتوى تم إهماله وفقًا لمرجع PDF. |
| [setFillFormsPermission(boolean value)](#setFillFormsPermission-boolean-) | يُشير إلى ما إذا كان يُسمح بملء حقول النماذج التفاعلية الموجودة (بما في ذلك حقول التوقيع)، حتى إذا كان [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\\#getModifyDocumentPermission--) واضحًا. |
| [setFullQualityPrintPermission(boolean value)](#setFullQualityPrintPermission-boolean-) | يُشير إلى ما إذا كان يُسمح بطباعة المستند إلى تمثيل يمكن من خلاله إنشاء نسخة رقمية دقيقة من محتوى PDF. |
| [setModifyDocumentPermission(boolean value)](#setModifyDocumentPermission-boolean-) | يُشير إلى ما إذا كان يُسمح بتعديل محتويات المستند بعمليات غير تلك التي يتحكم فيها [getAnnotationsPermission()](../../com.aspose.cells/pdfsecurityoptions\\#getAnnotationsPermission--)، [getFillFormsPermission()](../../com.aspose.cells/pdfsecurityoptions\\#getFillFormsPermission--) و [getAssembleDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\\#getAssembleDocumentPermission--). |
| [setOwnerPassword(String value)](#setOwnerPassword-java.lang.String-) | يضبط كلمة مرور المالك لمستند PDF المشفر. |
| [setPrintPermission(boolean value)](#setPrintPermission-boolean-) | يُشير إلى ما إذا كان يُسمح بطباعة المستند. |
| [setUserPassword(String value)](#setUserPassword-java.lang.String-) | يضبط كلمة مرور المستخدم المطلوبة لفتح مستند PDF المشفر. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PdfSecurityOptions() {#PdfSecurityOptions--}
```
public PdfSecurityOptions()
```


المُنشئ الخاص بـ PdfSecurityOptions

**Example**

الكود التالي يضبط إذن الطباعة بدقة عالية للمستند PDF الناتج.

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
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getAccessibilityExtractContent() {#getAccessibilityExtractContent--}
```
public boolean getAccessibilityExtractContent()
```


يُشير إلى ما إذا كان يُسمح باستخراج النص والرسومات (دعمًا لإمكانية الوصول للمستخدمين ذوي الإعاقة أو لأغراض أخرى).

**Returns:**
boolean
### getAnnotationsPermission() {#getAnnotationsPermission--}
```
public boolean getAnnotationsPermission()
```


يُشير إلى ما إذا كان يُسمح بإضافة أو تعديل تعليقات النص، وملء حقول النماذج التفاعلية.

**Remarks**

إذا كان [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\\#getModifyDocumentPermission--) مُحددًا أيضًا، يتم إنشاء أو تعديل حقول النماذج التفاعلية (بما في ذلك حقول التوقيع).

**Returns:**
boolean
### getAssembleDocumentPermission() {#getAssembleDocumentPermission--}
```
public boolean getAssembleDocumentPermission()
```


يُشير إلى ما إذا كان يُسمح بتجميع المستند (إدراج، تدوير، أو حذف الصفحات وإنشاء إشارات مرجعية أو صور مصغرة)، حتى إذا كان [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\\#getModifyDocumentPermission--) واضحًا.

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


يُشير إلى ما إذا كان يُسمح بنسخ أو استخراج النص والرسومات من المستند بطرق أخرى غير تلك التي يتحكم فيها [getAccessibilityExtractContent()](../../com.aspose.cells/pdfsecurityoptions\\#getAccessibilityExtractContent--).

**Returns:**
boolean
### getExtractContentPermissionObsolete() {#getExtractContentPermissionObsolete--}
```
public boolean getExtractContentPermissionObsolete()
```


إذن النسخ أو استخراج المحتوى تم إهماله وفقًا لمرجع PDF.

**Remarks**

ملاحظة: هذا العضو أصبح الآن مهملًا. بدلاً من ذلك، يرجى استخدام خاصية ExtractContentPermission. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ سبتمبر 2023. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
boolean
### getFillFormsPermission() {#getFillFormsPermission--}
```
public boolean getFillFormsPermission()
```


يُشير إلى ما إذا كان يُسمح بملء حقول النماذج التفاعلية الموجودة (بما في ذلك حقول التوقيع)، حتى إذا كان [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\\#getModifyDocumentPermission--) واضحًا.

**Returns:**
boolean
### getFullQualityPrintPermission() {#getFullQualityPrintPermission--}
```
public boolean getFullQualityPrintPermission()
```


يُشير إلى ما إذا كان يُسمح بطباعة المستند إلى تمثيل يمكن من خلاله إنشاء نسخة رقمية دقيقة من محتوى PDF.

**Remarks**

عندما يكون واضحًا (و[getPrintPermission()](../../com.aspose.cells/pdfsecurityoptions\\#getPrintPermission--) مُحددًا)، يقتصر الطباعة على تمثيل منخفض المستوى للمظهر، وربما بجودة منخفضة.

**Returns:**
boolean
### getModifyDocumentPermission() {#getModifyDocumentPermission--}
```
public boolean getModifyDocumentPermission()
```


يُشير إلى ما إذا كان يُسمح بتعديل محتويات المستند بعمليات غير تلك التي يتحكم فيها [getAnnotationsPermission()](../../com.aspose.cells/pdfsecurityoptions\\#getAnnotationsPermission--)، [getFillFormsPermission()](../../com.aspose.cells/pdfsecurityoptions\\#getFillFormsPermission--) و [getAssembleDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\\#getAssembleDocumentPermission--).

**Returns:**
boolean
### getOwnerPassword() {#getOwnerPassword--}
```
public String getOwnerPassword()
```


يحصل على كلمة مرور المالك لمستند PDF المشفر.

**Remarks**

كلمة مرور المالك تسمح للمستخدم بفتح مستند PDF مشفر دون أي قيود وصول محددة.

**Returns:**
java.lang.String
### getPrintPermission() {#getPrintPermission--}
```
public boolean getPrintPermission()
```


يُشير إلى ما إذا كان يُسمح بطباعة المستند.

**Remarks**

ربما ليس بأعلى مستوى جودة، اعتمادًا على ما إذا كان [getFullQualityPrintPermission()](../../com.aspose.cells/pdfsecurityoptions\#getFullQualityPrintPermission--) محددًا أيضًا.

**Returns:**
boolean
### getUserPassword() {#getUserPassword--}
```
public String getUserPassword()
```


يحصل على كلمة مرور المستخدم المطلوبة لفتح مستند PDF المشفر.

**Remarks**

سيتطلب كلمة مرور المالك أو كلمة مرور المستخدم لفتح مستند PDF مشفر للعرض.

يمكن أن تكون كلمة مرور المستخدم فارغة أو سلسلة فارغة، في هذه الحالة لن تكون كلمة مرور مطلوبة من المستخدم عند فتح مستند PDF.

فتح المستند باستخدام كلمة مرور المالك الصحيحة يتيح الوصول الكامل إلى المستند.

فتح المستند باستخدام كلمة مرور المستخدم الصحيحة (أو فتح مستند لا يحتوي على كلمة مرور مستخدم) يتيح وصولًا محدودًا وفقًا للأذونات المحددة.

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


يُشير إلى ما إذا كان يُسمح باستخراج النص والرسومات (دعمًا لإمكانية الوصول للمستخدمين ذوي الإعاقة أو لأغراض أخرى).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setAnnotationsPermission(boolean value) {#setAnnotationsPermission-boolean-}
```
public void setAnnotationsPermission(boolean value)
```


يُشير إلى ما إذا كان يُسمح بإضافة أو تعديل تعليقات النص، وملء حقول النماذج التفاعلية.

**Remarks**

إذا كان [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\\#getModifyDocumentPermission--) مُحددًا أيضًا، يتم إنشاء أو تعديل حقول النماذج التفاعلية (بما في ذلك حقول التوقيع).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setAssembleDocumentPermission(boolean value) {#setAssembleDocumentPermission-boolean-}
```
public void setAssembleDocumentPermission(boolean value)
```


يُشير إلى ما إذا كان يُسمح بتجميع المستند (إدراج، تدوير، أو حذف الصفحات وإنشاء إشارات مرجعية أو صور مصغرة)، حتى إذا كان [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\\#getModifyDocumentPermission--) واضحًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setExtractContentPermission(boolean value) {#setExtractContentPermission-boolean-}
```
public void setExtractContentPermission(boolean value)
```


يُشير إلى ما إذا كان يُسمح بنسخ أو استخراج النص والرسومات من المستند بطرق أخرى غير تلك التي يتحكم فيها [getAccessibilityExtractContent()](../../com.aspose.cells/pdfsecurityoptions\\#getAccessibilityExtractContent--).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setExtractContentPermissionObsolete(boolean value) {#setExtractContentPermissionObsolete-boolean-}
```
public void setExtractContentPermissionObsolete(boolean value)
```


إذن النسخ أو استخراج المحتوى تم إهماله وفقًا لمرجع PDF.

**Remarks**

ملاحظة: هذا العضو أصبح الآن مهملًا. بدلاً من ذلك، يرجى استخدام خاصية ExtractContentPermission. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ سبتمبر 2023. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setFillFormsPermission(boolean value) {#setFillFormsPermission-boolean-}
```
public void setFillFormsPermission(boolean value)
```


يُشير إلى ما إذا كان يُسمح بملء حقول النماذج التفاعلية الموجودة (بما في ذلك حقول التوقيع)، حتى إذا كان [getModifyDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\\#getModifyDocumentPermission--) واضحًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setFullQualityPrintPermission(boolean value) {#setFullQualityPrintPermission-boolean-}
```
public void setFullQualityPrintPermission(boolean value)
```


يُشير إلى ما إذا كان يُسمح بطباعة المستند إلى تمثيل يمكن من خلاله إنشاء نسخة رقمية دقيقة من محتوى PDF.

**Remarks**

عندما يكون واضحًا (و[getPrintPermission()](../../com.aspose.cells/pdfsecurityoptions\\#getPrintPermission--) مُحددًا)، يقتصر الطباعة على تمثيل منخفض المستوى للمظهر، وربما بجودة منخفضة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setModifyDocumentPermission(boolean value) {#setModifyDocumentPermission-boolean-}
```
public void setModifyDocumentPermission(boolean value)
```


يُشير إلى ما إذا كان يُسمح بتعديل محتويات المستند بعمليات غير تلك التي يتحكم فيها [getAnnotationsPermission()](../../com.aspose.cells/pdfsecurityoptions\\#getAnnotationsPermission--)، [getFillFormsPermission()](../../com.aspose.cells/pdfsecurityoptions\\#getFillFormsPermission--) و [getAssembleDocumentPermission()](../../com.aspose.cells/pdfsecurityoptions\\#getAssembleDocumentPermission--).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setOwnerPassword(String value) {#setOwnerPassword-java.lang.String-}
```
public void setOwnerPassword(String value)
```


يضبط كلمة مرور المالك لمستند PDF المشفر.

**Remarks**

كلمة مرور المالك تسمح للمستخدم بفتح مستند PDF مشفر دون أي قيود وصول محددة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setPrintPermission(boolean value) {#setPrintPermission-boolean-}
```
public void setPrintPermission(boolean value)
```


يُشير إلى ما إذا كان يُسمح بطباعة المستند.

**Remarks**

ربما ليس بأعلى مستوى جودة، اعتمادًا على ما إذا كان [getFullQualityPrintPermission()](../../com.aspose.cells/pdfsecurityoptions\#getFullQualityPrintPermission--) محددًا أيضًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setUserPassword(String value) {#setUserPassword-java.lang.String-}
```
public void setUserPassword(String value)
```


يضبط كلمة مرور المستخدم المطلوبة لفتح مستند PDF المشفر.

**Remarks**

سيتطلب كلمة مرور المالك أو كلمة مرور المستخدم لفتح مستند PDF مشفر للعرض.

يمكن أن تكون كلمة مرور المستخدم فارغة أو سلسلة فارغة، في هذه الحالة لن تكون كلمة مرور مطلوبة من المستخدم عند فتح مستند PDF.

فتح المستند باستخدام كلمة مرور المالك الصحيحة يتيح الوصول الكامل إلى المستند.

فتح المستند باستخدام كلمة مرور المستخدم الصحيحة (أو فتح مستند لا يحتوي على كلمة مرور مستخدم) يتيح وصولًا محدودًا وفقًا للأذونات المحددة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

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

