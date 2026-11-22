---
title: "الفئة CustomCommandButtonCollection"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.GridWeb.CustomCommandButtonCollection. تمثل مجموعة CustomCommandButton"
type: docs
url: /ar/net/aspose.cells.gridweb/customcommandbuttoncollection/
---
## CustomCommandButtonCollection class

يمثل مجموعة CustomCommandButton.

```csharp
public class CustomCommandButtonCollection : CollectionBase
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Count](../../aspose.cells.gridweb/customcommandbuttoncollection/count/) { get; } | يحصل على عدد المجموعة. |
| [IsFixedSize](../../aspose.cells.gridweb/customcommandbuttoncollection/isfixedsize/) { get; } | مستخدم داخليًا فقط. |
| [IsReadOnly](../../aspose.cells.gridweb/customcommandbuttoncollection/isreadonly/) { get; } | مستخدم داخليًا فقط. |
| [IsSynchronized](../../aspose.cells.gridweb/customcommandbuttoncollection/issynchronized/) { get; } | مستخدم داخليًا فقط. |
| [Item](../../aspose.cells.gridweb/customcommandbuttoncollection/item/) { get; set; } | يحصل على كائن زر أمر مخصص عند الفهرس. |
| [SyncRoot](../../aspose.cells.gridweb/customcommandbuttoncollection/syncroot/) { get; } | مستخدم داخليًا فقط. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Add](../../aspose.cells.gridweb/customcommandbuttoncollection/add/)(object) | يضيف كائن زر أمر مخصص إلى المجموعة. |
| [Clear](../../aspose.cells.gridweb/customcommandbuttoncollection/clear/#clear)() | يمسح المجموعة. |
| [Contains](../../aspose.cells.gridweb/customcommandbuttoncollection/contains/)(object) | يشير إلى ما إذا كان كائن زر الأمر المخصص موجودًا في المجموعة. |
| [CopyTo](../../aspose.cells.gridweb/customcommandbuttoncollection/copyto/)(Array, int) | ينسخ المجموعة إلى مصفوفة. |
| [GetEnumerator](../../aspose.cells.gridweb/customcommandbuttoncollection/getenumerator/#getenumerator)() | يحصل على كائن IEnumerator من المجموعة. |
| [IndexOf](../../aspose.cells.gridweb/customcommandbuttoncollection/indexof/)(object) | يحصل على فهرس الزر. |
| [Insert](../../aspose.cells.gridweb/customcommandbuttoncollection/insert/)(int, object) | يدرج زرًا في الفهرس. |
| [Remove](../../aspose.cells.gridweb/customcommandbuttoncollection/remove/)(object) | يزيل كائن زر الأمر المخصص. |
| [RemoveAt](../../aspose.cells.gridweb/customcommandbuttoncollection/removeat/#removeat)(int) | يزيل عند الفهرس. |

### أمثلة

```csharp
[C#]
GridWeb GridWeb1 = new GridWeb();
CustomCommandButton button = new CustomCommandButton();
button.Command = "MyCommand";
button.ImageUrl = "images/button1.gif";
GridWeb1.CustomCommandButtons.Add(button);
[VB]
Dim GridWeb1 As GridWeb= New GridWeb();
Dim button As CustomCommandButton =  New CustomCommandButton()
button.Command = "MyCommand"
button.ImageUrl = "images/button1.gif"
GridWeb1.CustomCommandButtons.Add(button)
```

### انظر أيضًا

* namespace [Aspose.Cells.GridWeb](../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../)


