---
title: "GridNameCollection.Add"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة GridNameCollection. تعريف اسم عالمي جديد"
type: docs
url: /ar/net/aspose.cells.gridweb.data/gridnamecollection/add/
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
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)

---

## Add(int, string, string) {#add}

يعرّف اسمًا جديدًا في الورقة المحددة.

```csharp
public int Add(int sheetIndex, string text, string refersTo)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| sheetIndex | Int32 | فهرس الورقة التي يُطبق فيها الاسم. |
| نص | String | نص الاسم. لا يمكن أن يحتوي على اسم ورقة. |
| refersTo | String | الصيغة التي يُعرّف الاسم للإشارة إليها. يجب أن يحتوي على اسم ورقة. مثال: 'sheet hello!'A1:B2. |

### قيمة الإرجاع

فهرس كائن الاسم.

### انظر أيضًا

* class [GridNameCollection](../)
* namespace [Aspose.Cells.GridWeb.Data](../../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../../)


