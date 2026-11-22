---
title: "GridNameCollection.Add"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة GridNameCollection. تعريف اسم عالمي جديد"
type: docs
url: /ar/net/aspose.cells.griddesktop.data/gridnamecollection/add/
---
## Add(string, string) {#add_1}

يعرّف اسمًا عالميًا جديدًا.

```csharp
public int Add(string text, string refersTo)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| نص | String | نص الاسم. يمكن أن يحتوي على اسم ورقة. |
| refersTo | String | الصيغة التي يُعرّف الاسم للإشارة إليها. يجب أن يحتوي على اسم ورقة. مثال: 'sheet hello!'A1:B2. |

### قيمة الإرجاع

فهرس كائن الاسم.

### انظر أيضًا

* class [GridNameCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)

---

## Add(int, string, string) {#add}

يعرّف اسمًا جديدًا في الورقة المحددة.

```csharp
public int Add(int sheetIndex, string text, string refersTo)
```

| معامل | الوصف |
| --- | --- |
| sheetIndex | فهرس الورقة التي يُطبق فيها الاسم. |
| نص | نص الاسم. لا يمكن أن يحتوي على اسم ورقة. |
| refersTo | الصيغة التي يُعرّف الاسم للإشارة إليها. يجب أن يحتوي على اسم ورقة. مثال: 'sheet hello!'A1:B2. |
| sheetIndex | فهرس الورقة للاسم، الفهرس يبدأ من 1. |

### قيمة الإرجاع

فهرس كائن الاسم.

### انظر أيضًا

* class [GridNameCollection](../)
* namespace [Aspose.Cells.GridDesktop.Data](../../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../../)


