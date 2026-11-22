---
title: "GridDesktop.SetCustomResourceManager"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة GridDesktop. تعيين مدير موارد مخصص لتنفيذ التعريب المحدد من قبل المستخدم"
type: docs
url: /ar/net/aspose.cells.griddesktop/griddesktop/setcustomresourcemanager/
---
## GridDesktop.SetCustomResourceManager method

تعيين مدير موارد مخصص لتنفيذ التعريب المحدد من قبل المستخدم.

```csharp
public void SetCustomResourceManager(ResourceManager customResourceManager)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| customResourceManager | ResourceManager | مدير الموارد المخصص. |

### ملاحظات

لإنشاء ملف موارد مخصص، يرجى اتباع الصيغة الموجودة في GridDesktopResource.resx.

### أمثلة

```csharp
[C#]
ResourceManager rm = new ResourceManager("yourapp.customtlocale", Assembly.GetExecutingAssembly());
gridDesktop1.SetCustomResourceManager(rm);
```

### انظر أيضًا

* class [GridDesktop](../)
* namespace [Aspose.Cells.GridDesktop](../../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../../)


