---
title: "IGridJsService.AddImage"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة IGridJsService. تُطبق عملية إضافة صورة من ملف محلي باستخدام بايتات الصورة مباشرة"
type: docs
url: /ar/net/aspose.cells.gridjs/igridjsservice/addimage/
---
## AddImage(string, string, string, byte[]) {#addimage}

يطبق عملية إضافة صورة من ملف محلي، مع أخذ بايتات الصورة مباشرة.

```csharp
public string AddImage(string p, string uid, string iscontrol, byte[] fileBytes)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| p | String | معامل سلسلة JSON |
| uid | String | المعرّف الفريد لملف التخزين المؤقت. |
| iscontrol | String | حدد ما إذا كان تحكمًا. |
| fileBytes | Byte[] | البايتات الخام لملف الصورة |

### قيمة الإرجاع

نتيجة سلسلة JSON

### انظر أيضًا

* interface [IGridJsService](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)

---

## AddImage(string, string, string, IFormFileCollection) {#addimage_1}

يطبق عملية إضافة صورة من ملف محلي، مع أخذ ملفات النموذج المرفوعة.

```csharp
public string AddImage(string p, string uid, string iscontrol, IFormFileCollection files)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| p | String | معامل سلسلة JSON |
| uid | String | المعرّف الفريد لملف التخزين المؤقت. |
| iscontrol | String | حدد ما إذا كان تحكمًا. |
| ملفات | IFormFileCollection | ملف النموذج الخاص بالصورة |

### قيمة الإرجاع

نتيجة سلسلة JSON

### انظر أيضًا

* interface [IGridJsService](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)


