---
title: "ICustomParser"
second_title: "Aspose.Cells for Java API Reference"
description: "يسمح للمستخدمين بإضافة محلل القيم المخصص الخاص بهم لتحويل القيم النصية إلى كائن قيمة خلية مناسب آخر."
type: docs
url: /ar/java/com.aspose.cells/icustomparser/
---
```
public interface ICustomParser
```

يسمح للمستخدمين بإضافة محلل القيم المخصص الخاص بهم لتحويل القيم النصية إلى كائن قيمة خلية مناسب آخر.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getFormat()](#getFormat--) | يحصل على نمط التنسيق المقابل للقيمة التي تم تحليلها بواسطة آخر استدعاء لـ [parseObject(String)](../../com.aspose.cells/icustomparser\#parseObject-String-). |
| [parseObject(String value)](#parseObject-java.lang.String-) | يقوم بتحليل السلسلة المعطاة إلى كائن قيمة مناسب. |
### getFormat() {#getFormat--}
```
public abstract String getFormat()
```


يحصل على نمط التنسيق المقابل للقيمة التي تم تحليلها بواسطة آخر استدعاء لـ [parseObject(String)](../../com.aspose.cells/icustomparser\#parseObject-String-).

**Remarks**

قد يُستخدم نمط التنسيق المرجع لتنسيق الخلية المقابلة (قم بتعيينه إلى Style.Custom للخلية).

**Returns:**
java.lang.String
### parseObject(String value) {#parseObject-java.lang.String-}
```
public abstract Object parseObject(String value)
```


يقوم بتحليل السلسلة المعطاة إلى كائن قيمة مناسب.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | قيمة السلسلة التي سيتم تحليلها |

**Returns:**
java.lang.Object - كائن قيمة تم تحليله من السلسلة المعطاة. إذا تعذر تحليل السلسلة المعطاة إلى كائن قيمة مناسب، يُرجع null.
