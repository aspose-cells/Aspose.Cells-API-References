---
title: "MainWeb.SessionMode"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية MainWeb. تحصل أو تعيين وضع الجلسة للشبكة"
type: docs
url: /ar/net/aspose.cells.gridweb/mainweb/sessionmode/
---
## MainWeb.SessionMode property

الحصول أو تعيين وضع الجلسة للشبكة.

```csharp
public SessionMode SessionMode { get; set; }
```

### ملاحظات

هناك 4 أنواع من وضع الجلسة: 1. Session (الافتراضي): استخدم جلسة النظام لتخزين بيانات الورقة. عادةً يستخدم asp.net حالة الجلسة InProc. تدعم الشبكة أيضًا حالة الجلسة "StateServer" خارج العملية وحالة الجلسة SQLServer. 2. ViewState: استخدم ViewState للصفحة لتخزين بيانات الورقة. 3. Custom: استخدم أحداث LoadCustomData و SheetDataUpdated لتخزين/استعادة بيانات الورقة. 4. File: خزن/استعد بيانات الورقة في SessionStorePath. هذه هي الطريقة المقترحة ويمكن الحفاظ على الملف دائمًا. عند استخدام SessionMode.ViewState، ستخزن الشبكة بعض البيانات في ViewState للصفحة. سيؤدي ذلك إلى تقليل استخدام الذاكرة على الخادم، لكن حجم الصفحة سيكون أكبر وسيؤثر على الأداء العام.

### أمثلة

```csharp
[C#]
	GridWeb1.SessionMode = SessionMode.ViewState;
	
[Visual Basic]
	GridWeb1.SessionMode = SessionMode.ViewState
```

### انظر أيضًا

* enum [SessionMode](../../sessionmode/)
* class [MainWeb](../)
* namespace [Aspose.Cells.GridWeb](../../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../../)


