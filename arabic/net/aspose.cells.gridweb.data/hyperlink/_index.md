---
title: "الفئة Hyperlink"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.GridWeb.Data.Hyperlink."
type: docs
url: /ar/net/aspose.cells.gridweb.data/hyperlink/
---
## Hyperlink class

```csharp
[Obsolete("This class is obsolete; use GridHyperlink instead")]
public class Hyperlink
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| virtual [ActionType](../../aspose.cells.gridweb.data/hyperlink/actiontype/) { get; set; } | يحصل أو يعيّن نوع إجراء الارتباط التشعبي. قد يكون ActionTpye.UrlLink أو ActionType.CellCommand. نوع UrlLink يعني أن الارتباط التشعبي هو رابط إلى صفحة ويب أو إلى بريد إلكتروني. على سبيل المثال: "http://www.aspose.com" أو "mailto:admin@aspose.com". نوع CellCommand يعني أن الارتباط التشعبي سيطلق حدث CellCommand، ويمكنك معالجة هذا الحدث. |
| [Area](../../aspose.cells.gridweb.data/hyperlink/area/) { get; } | يحصل على نطاق الارتباط التشعبي. |
| [CellCommand](../../aspose.cells.gridweb.data/hyperlink/cellcommand/) { get; set; } | يحصل أو يعيّن اسم أمر الخلية. |
| virtual [DiscardInput](../../aspose.cells.gridweb.data/hyperlink/discardinput/) { get; set; } | يشير إلى ما إذا كان يجب تجاهل إدخال المستخدم في متصفح العميل عندما ينقر المستخدم على هذا الارتباط التشعبي CellCommand. يمكن استخدامه كإجراء "تراجع". |
| virtual [ImageUrl](../../aspose.cells.gridweb.data/hyperlink/imageurl/) { get; set; } | يحصل أو يعيّن عنوان URL لصورة الارتباط التشعبي. إذا تم تعيينه إلى null أو سلسلة فارغة، سيعرض الارتباط التشعبي نصه فقط. |
| [Target](../../aspose.cells.gridweb.data/hyperlink/target/) { get; set; } |  |
| virtual [Text](../../aspose.cells.gridweb.data/hyperlink/text/) { get; set; } | يحصل أو يعيّن النص المعروض للارتباط التشعبي. |
| virtual [ToolTip](../../aspose.cells.gridweb.data/hyperlink/tooltip/) { get; set; } | يحصل أو يعيّن تلميح الأدوات للارتباط التشعبي. |
| virtual [Url](../../aspose.cells.gridweb.data/hyperlink/url/) { get; set; } | يحصل أو يعيّن سلسلة URL. |

### انظر أيضًا

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


