---
title: "الفئة ComboBox"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.GridDesktop.ComboBox. تمثل عنصر تحكم خلية من نوع combobox"
type: docs
url: /ar/net/aspose.cells.griddesktop/combobox/
---
## ComboBox class

يمثل عنصر تحكم مربع اختيار الخلية.

```csharp
public class ComboBox : CellControl
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Height](../../aspose.cells.griddesktop/combobox/height/) { get; set; } | يحصل أو يعيّن ارتفاع عنصر التحكم في القائمة. |
| [IsInputable](../../aspose.cells.griddesktop/combobox/isinputable/) { get; set; } | يشير إلى ما إذا كان المستخدم يمكنه إدخال نص إلى الـ combobox. سيتم حفظ النص المدخل كقيمة الخلية. القيمة الافتراضية هي "false". |
| [Items](../../aspose.cells.griddesktop/combobox/items/) { get; } | يحصل على كائن يمثل مجموعة العناصر الموجودة في هذا الـ ComboBox. |
| [SelectedIndex](../../aspose.cells.griddesktop/combobox/selectedindex/) { get; set; } | يحصل أو يعيّن الفهرس الذي يحدد العنصر المحدد حاليًا. تعيين الفهرس سيستدعي طريقة GridDesktop.RunAllFormulas تلقائيًا إذا كانت خاصية GridDesktop.RecalculateFormulas صحيحة. |
| [Text](../../aspose.cells.griddesktop/cellcontrol/text/) { get; set; } | يحصل أو يعيّن النص المرتبط بهذا العنصر.(موروث من [`CellControl`](../cellcontrol/).) |
| [Values](../../aspose.cells.griddesktop/combobox/values/) { get; } | يحصل على كائن يمثل مجموعة القيم الموجودة في هذا الـ ComboBox. |
| [Width](../../aspose.cells.griddesktop/combobox/width/) { get; set; } | يحصل أو يعيّن عرض عنصر التحكم في القائمة. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [SetSelectedIndex](../../aspose.cells.griddesktop/combobox/setselectedindex/)(int) | يعيّن الفهرس المحدد للـ ComboBox. هذا لن يحسب الصيغة. لحساب الصيغة، تحتاج إلى استدعاء GridDesktop.RunAllFormulas يدويًا. لن يتم حساب الصيغ تلقائيًا في أي حالة حتى إذا كانت GridDesktop.RecalculateFormulas صحيحة. |

### انظر أيضًا

* class [CellControl](../cellcontrol/)
* namespace [Aspose.Cells.GridDesktop](../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../)


