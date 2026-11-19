---
title: "IFilePathProvider"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل موفر مسار الملف المصدر."
type: docs
url: /ar/java/com.aspose.cells/ifilepathprovider/
---
```
public interface IFilePathProvider
```

يمثل موفر مسار الملف المصدر.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getFullName(String sheetName)](#getFullName-java.lang.String-) | يحصل على المسار الكامل للملف حسب اسم ورقة العمل عند تصدير ورقة العمل إلى HTML بشكل منفصل. |
### getFullName(String sheetName) {#getFullName-java.lang.String-}
```
public abstract String getFullName(String sheetName)
```


يحصل على المسار الكامل للملف حسب اسم ورقة العمل عند تصدير ورقة العمل إلى HTML بشكل منفصل. بحيث يمكن تصدير المراجع بين أوراق العمل بشكل صحيح.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sheetName | java.lang.String | اسم ورقة العمل |

**Returns:**
java.lang.String - المسار الكامل للملف
