---
title: "GridCustomServerValidation"
second_title: "Aspose.Cells for Java API Reference"
description: "الواجهة التي تحتاج إلى تنفيذها عند استخدام التحقق من الجانب الخادم."
type: docs
url: /ar/java/com.aspose.gridweb/gridcustomservervalidation/
---
```
public interface GridCustomServerValidation
```

الواجهة التي تحتاج إلى تنفيذها عند استخدام التحقق من الجانب الخادم. CustomServerFunction.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [validate(GridWorksheet sheet, int row, int col, String value)](#validate-com.aspose.gridweb.GridWorksheet-int-int-java.lang.String-) | **ملاحظات** |
### validate(GridWorksheet sheet, int row, int col, String value) {#validate-com.aspose.gridweb.GridWorksheet-int-int-java.lang.String-}
```
public abstract String validate(GridWorksheet sheet, int row, int col, String value)
```


**Remarks**

إذا أُرجِع string.empty فإن التحقق ينجح، وإلا يمكنك إرجاع أي رسالة ذات صلة يمكن التعامل معها في دالة ClientCallback.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sheet | [GridWorksheet](../../com.aspose.gridweb/gridworksheet) | الـ GridWorksheet |
| صف | int | فهرس الصف للخلية |
| col | int | فهرس العمود للخلية |
| القيمة | java.lang.String | القيمة لإجراء التحقق |

**Returns:**
java.lang.String - قيمة النتيجة المستندة إلى سلسلة
