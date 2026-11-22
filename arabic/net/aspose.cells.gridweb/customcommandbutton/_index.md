---
title: "الفئة CustomCommandButton"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.GridWeb.CustomCommandButton. تمثل زر أمر مخصص في شريط علامات التبويب لعنصر التحكم GridWeb."
type: docs
url: /ar/net/aspose.cells.gridweb/customcommandbutton/
---
## CustomCommandButton class

يمثل زر أمر مخصص في شريط علامات التبويب للتحكم GridWeb.

```csharp
public class CustomCommandButton : Control, ISerializable
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [CustomCommandButton](customcommandbutton/)() | المنشئ الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [ClientClickEvent](../../aspose.cells.gridweb/customcommandbutton/clientclickevent/) { get; set; } | يحصل أو يحدد معالج حدث النقر على جانب العميل. |
| [Command](../../aspose.cells.gridweb/customcommandbutton/command/) { get; set; } | يحصل أو يحدد اسم الأمر. |
| [CommandType](../../aspose.cells.gridweb/customcommandbutton/commandtype/) { get; set; } | يحصل أو يحدد نوع العرض للأمر. يمكن أن يكون النوع زر أمر أو عنصر قائمة سياقية. |
| [DiscardInput](../../aspose.cells.gridweb/customcommandbutton/discardinput/) { get; set; } | يشير إلى ما إذا كان يجب تجاهل إدخال المستخدم في متصفح العميل عندما ينقر المستخدم هذا الزر. يمكن استخدامه كإجراء \"تراجع\". |
| [ImageUrl](../../aspose.cells.gridweb/customcommandbutton/imageurl/) { get; set; } | يحصل أو يحدد عنوان URL لصورة زر الأمر. إذا تم تعيينه إلى null أو سلسلة فارغة، سيعرض الزر النص فقط. |
| [Text](../../aspose.cells.gridweb/customcommandbutton/text/) { get; set; } | يحصل أو يحدد النص البديل لزر الأمر. |
| [ToolTip](../../aspose.cells.gridweb/customcommandbutton/tooltip/) { get; set; } | يحصل أو يحدد تلميح الأدوات لزر الأمر. |
| [Width](../../aspose.cells.gridweb/customcommandbutton/width/) { get; set; } | عرض الزر. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [GetObjectData](../../aspose.cells.gridweb/customcommandbutton/getobjectdata/)(SerializationInfo, StreamingContext) | مستخدم داخليًا فقط. |

### أمثلة

```csharp
[C#]
GridWebBean GridWeb1=ExtPage.getInstance().getBean();
CustomCommandButton button = new CustomCommandButton();
button.Command = "MyCommand";
button.ImageUrl = "images/button1.gif";
GridWeb1.CustomCommandButtons.Add(button);
[VB]
Dim button As CustomCommandButton =  New CustomCommandButton()
button.Command = "MyCommand"
button.ImageUrl = "images/button1.gif"
GridWeb1.CustomCommandButtons.Add(button)
```

### انظر أيضًا

* namespace [Aspose.Cells.GridWeb](../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../)


