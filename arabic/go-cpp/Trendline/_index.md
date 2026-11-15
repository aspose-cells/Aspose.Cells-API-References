---
title: "Trendline فئة"
linktitle: "Trendline"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "Trendline فئة. تغلف الكائن الذي يمثل trendline في Go."
type: docs
weight: 200
url: /ar/go-cpp/trendline/
---

## Trendline class

يمثل خط الاتجاه في مخطط.

```go

type Trendline struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |
| [NewTrendline](./newtrendline/) | يُنشئ من كائن أب. |

## طرق

| طريقة | الوصف |
| --- | --- |
| [IsNull](./isnull/) | يتحقق مما إذا كان كائن التنفيذ هو nullptr. |
| [IsNameAuto](./isnameauto/) | يرجع ما إذا كان Microsoft Excel يحدد اسم خط الاتجاه تلقائيًا. |
| [SetIsNameAuto](./setisnameauto/) | يرجع ما إذا كان Microsoft Excel يحدد اسم خط الاتجاه تلقائيًا. |
| [GetType](./gettype/) | يرجع نوع خط الاتجاه. |
| [GetName](./getname/) | يرجع اسم خط الاتجاه. |
| [SetName](./setname/) | يرجع اسم خط الاتجاه. |
| [GetOrder](./getorder/) | يرجع أو يضبط ترتيب خط الاتجاه (عدد صحيح أكبر من 1) عندما يكون نوع خط الاتجاه Polynomial. يجب أن يكون الترتيب بين 2 و 6. |
| [SetOrder](./setorder/) | يرجع أو يضبط ترتيب خط الاتجاه (عدد صحيح أكبر من 1) عندما يكون نوع خط الاتجاه Polynomial. يجب أن يكون الترتيب بين 2 و 6. |
| [GetPeriod](./getperiod/) | يرجع أو يضبط الفترة لخط الاتجاه المتوسط المتحرك. |
| [SetPeriod](./setperiod/) | يرجع أو يضبط الفترة لخط الاتجاه المتوسط المتحرك. |
| [GetForward](./getforward/) | يرجع أو يضبط عدد الفترات (أو الوحدات على مخطط التشتت) التي يمتد إليها خط الاتجاه إلى الأمام. يجب أن يكون عدد الفترات أكبر من أو يساوي الصفر. |
| [SetForward](./setforward/) | يرجع أو يضبط عدد الفترات (أو الوحدات على مخطط التشتت) التي يمتد إليها خط الاتجاه إلى الأمام. يجب أن يكون عدد الفترات أكبر من أو يساوي الصفر. |
| [GetBackward](./getbackward/) | يرجع أو يضبط عدد الفترات (أو الوحدات على مخطط التشتت) التي يمتد إليها خط الاتجاه إلى الخلف. يجب أن يكون عدد الفترات أكبر من أو يساوي الصفر. إذا كان نوع المخطط عموديًا، يجب أن يكون عدد الفترات بين 0 و 0.5 |
| [SetBackward](./setbackward/) | يرجع أو يضبط عدد الفترات (أو الوحدات على مخطط التشتت) التي يمتد إليها خط الاتجاه إلى الخلف. يجب أن يكون عدد الفترات أكبر من أو يساوي الصفر. إذا كان نوع المخطط عموديًا، يجب أن يكون عدد الفترات بين 0 و 0.5 |
| [GetDisplayEquation](./getdisplayequation/) | يمثل ما إذا كانت معادلة خط الاتجاه معروضة على المخطط (في نفس تسمية البيانات كقيمة R-squared). ضبط هذه الخاصية إلى True يُفعّل تلقائيًا تسميات البيانات. |
| [SetDisplayEquation](./setdisplayequation/) | يمثل ما إذا كانت معادلة خط الاتجاه معروضة على المخطط (في نفس تسمية البيانات كقيمة R-squared). ضبط هذه الخاصية إلى True يُفعّل تلقائيًا تسميات البيانات. |
| [GetDisplayRSquared](./getdisplayrsquared/) | يمثل ما إذا كانت قيمة R-squared لخط الاتجاه معروضة على المخطط (في نفس تسمية البيانات كالمعادلة). ضبط هذه الخاصية إلى True يُفعّل تلقائيًا تسميات البيانات. |
| [SetDisplayRSquared](./setdisplayrsquared/) | يمثل ما إذا كانت قيمة R-squared لخط الاتجاه معروضة على المخطط (في نفس تسمية البيانات كالمعادلة). ضبط هذه الخاصية إلى True يُفعّل تلقائيًا تسميات البيانات. |
| [GetIntercept](./getintercept/) | يرجع أو يضبط النقطة التي يقطع فيها خط الاتجاه محور القيم. |
| [SetIntercept](./setintercept/) | يرجع أو يضبط النقطة التي يقطع فيها خط الاتجاه محور القيم. |
| [GetDataLabels](./getdatalabels/) | يمثل كائن DataLabels للسلسلة المحددة. |
| [GetLegendEntry](./getlegendentry/) | يحصل على مدخل الأسطورة وفقًا لهذا خط الاتجاه |
| [GetCompoundType](./getcompoundtype/) | يحدد نوع الخط المركب |
| [SetCompoundType](./setcompoundtype/) | يحدد نوع الخط المركب |
| [GetDashType](./getdashtype/) | يحدد نوع خط المتقطع |
| [SetDashType](./setdashtype/) | يحدد نوع خط المتقطع |
| [GetCapType](./getcaptype/) | يحدد نهايات القُبُعات. |
| [SetCapType](./setcaptype/) | يحدد نهايات القُبُعات. |
| [GetJoinType](./getjointype/) | يحدد القُبُعات المتصلة. |
| [SetJoinType](./setjointype/) | يحدد القُبُعات المتصلة. |
| [GetBeginType](./getbegintype/) | يحدد رأس السهم لبداية الخط. |
| [SetBeginType](./setbegintype/) | يحدد رأس السهم لبداية الخط. |
| [GetEndType](./getendtype/) | يحدد رأس السهم لنهاية الخط. |
| [SetEndType](./setendtype/) | يحدد رأس السهم لنهاية الخط. |
| [GetBeginArrowLength](./getbeginarrowlength/) | يحدد طول رأس السهم لبداية الخط. |
| [SetBeginArrowLength](./setbeginarrowlength/) | يحدد طول رأس السهم لبداية الخط. |
| [GetEndArrowLength](./getendarrowlength/) | يحدد طول رأس السهم لنهاية الخط. |
| [SetEndArrowLength](./setendarrowlength/) | يحدد طول رأس السهم لنهاية الخط. |
| [GetBeginArrowWidth](./getbeginarrowwidth/) | يحدد عرض رأس السهم لبداية الخط. |
| [SetBeginArrowWidth](./setbeginarrowwidth/) | يحدد عرض رأس السهم لبداية الخط. |
| [GetEndArrowWidth](./getendarrowwidth/) | يحدد عرض رأس السهم لنهاية الخط. |
| [SetEndArrowWidth](./setendarrowwidth/) | يحدد عرض رأس السهم لنهاية الخط. |
| [GetThemeColor](./getthemecolor/) | يحصل ويضبط لون السمة. |
| [SetThemeColor](./setthemecolor/) | يحصل ويضبط لون السمة. |
| [GetColor](./getcolor/) | يمثل لون الخط. |
| [SetColor](./setcolor/) | يمثل لون الخط. |
| [GetTransparency](./gettransparency/) | يعيد أو يضبط درجة شفافية الخط كقيمة من 0.0 (معتم) إلى 1.0 (شفاف). |
| [SetTransparency](./settransparency/) | يعيد أو يضبط درجة شفافية الخط كقيمة من 0.0 (معتم) إلى 1.0 (شفاف). |
| [GetStyle](./getstyle/) | يمثل نمط الخط. |
| [SetStyle](./setstyle/) | يمثل نمط الخط. |
| [GetWeight](./getweight/) | يحصل أو يضبط نوع الوزن للخط. |
| [SetWeight](./setweight/) | يحصل أو يضبط نوع الوزن للخط. |
| [GetWeightPt](./getweightpt/) | يحصل أو يضبط وزن الخط بوحدة النقاط. |
| [SetWeightPt](./setweightpt/) | يحصل أو يضبط وزن الخط بوحدة النقاط. |
| [GetWeightPx](./getweightpx/) | يحصل أو يضبط وزن الخط بوحدة البكسل. |
| [SetWeightPx](./setweightpx/) | يحصل أو يضبط وزن الخط بوحدة البكسل. |
| [GetFormattingType](./getformattingtype/) | يحصل أو يضبط نوع التنسيق. |
| [SetFormattingType](./setformattingtype/) | يحصل أو يضبط نوع التنسيق. |
| [IsAutomaticColor](./isautomaticcolor/) | يشير إلى ما إذا كان لون الخط معينًا تلقائيًا. |
| [IsVisible](./isvisible/) | يمثل ما إذا كان الخط مرئيًا. |
| [SetIsVisible](./setisvisible/) | يمثل ما إذا كان الخط مرئيًا. |
| [IsAuto](./isauto/) | يشير إلى ما إذا كان نمط الخط هذا معينًا تلقائيًا. |
| [SetIsAuto](./setisauto/) | يشير إلى ما إذا كان نمط الخط هذا معينًا تلقائيًا. |
| [GetGradientFill](./getgradientfill/) | يمثل تعبئة التدرج. |
