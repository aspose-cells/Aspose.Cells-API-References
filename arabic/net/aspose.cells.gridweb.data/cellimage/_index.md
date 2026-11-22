---
title: "الفئة CellImage"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.GridWeb.Data.CellImage. تمثل ارتباطًا تشعبيًا مع مصدر صورة."
type: docs
url: /ar/net/aspose.cells.gridweb.data/cellimage/
---
## CellImage class

يمثل رابطًا تشعبيًا مع مصدر الصورة.

```csharp
public class CellImage : Hyperlink
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| virtual [ActionType](../../aspose.cells.gridweb.data/hyperlink/actiontype/) { get; set; } | يحصل أو يعيّن نوع إجراء الارتباط التشعبي. قد يكون ActionTpye.UrlLink أو ActionType.CellCommand. نوع UrlLink يعني أن الارتباط التشعبي هو رابط إلى صفحة ويب أو بريد إلكتروني. على سبيل المثال: "http://www.aspose.com" أو "mailto:admin@aspose.com". نوع CellCommand يعني أن الارتباط التشعبي سيطلق حدث CellCommand، ويمكنك معالجة هذا الحدث. (موروث من [`Hyperlink`](../hyperlink/).) |
| [Area](../../aspose.cells.gridweb.data/hyperlink/area/) { get; } | يحصل على نطاق الارتباط التشعبي. (موروث من [`Hyperlink`](../hyperlink/).) |
| [CellCommand](../../aspose.cells.gridweb.data/hyperlink/cellcommand/) { get; set; } | يحصل أو يعيّن اسم أمر الخلية. (موروث من [`Hyperlink`](../hyperlink/).) |
| virtual [DiscardInput](../../aspose.cells.gridweb.data/hyperlink/discardinput/) { get; set; } | يشير إلى ما إذا كان يجب تجاهل إدخال المستخدم في متصفح العميل عندما ينقر المستخدم على هذا الارتباط التشعبي CellCommand. يمكن استخدامه كإجراء "تراجع". (موروث من [`Hyperlink`](../hyperlink/).) |
| virtual [ImageUrl](../../aspose.cells.gridweb.data/hyperlink/imageurl/) { get; set; } | يحصل أو يعيّن عنوان URL لصورة الارتباط التشعبي. إذا تم تعيينه إلى null أو سلسلة فارغة، سيعرض الارتباط التشعبي نصه فقط. (موروث من [`Hyperlink`](../hyperlink/).) |
| [Target](../../aspose.cells.gridweb.data/hyperlink/target/) { get; set; } | (موروث من [`Hyperlink`](../hyperlink/).) |
| virtual [Text](../../aspose.cells.gridweb.data/hyperlink/text/) { get; set; } | يحصل أو يعيّن النص المعروض للارتباط التشعبي. (موروث من [`Hyperlink`](../hyperlink/).) |
| virtual [ToolTip](../../aspose.cells.gridweb.data/hyperlink/tooltip/) { get; set; } | يحصل أو يعيّن تلميح الأداة للارتباط التشعبي. (موروث من [`Hyperlink`](../hyperlink/).) |
| virtual [Url](../../aspose.cells.gridweb.data/hyperlink/url/) { get; set; } | يحصل أو يعيّن سلسلة URL. (موروث من [`Hyperlink`](../hyperlink/).) |

### انظر أيضًا

* class [Hyperlink](../hyperlink/)
* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


