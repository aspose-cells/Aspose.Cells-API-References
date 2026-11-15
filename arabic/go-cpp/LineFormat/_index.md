---
title: "فئة LineFormat"
linktitle: "LineFormat"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة LineFormat. تغلف الكائن الذي يمثل تنسيق الخط في Go."
type: docs
weight: 200
url: /ar/go-cpp/lineformat/
---

## LineFormat class

يمثل جميع إعدادات الخط.

```go

type LineFormat struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |
| [NewLineFormat](./newlineformat/) | يُنشئ من كائن أب. |

## طرق

| طريقة | الوصف |
| --- | --- |
| [IsNull](./isnull/) | يتحقق مما إذا كان كائن التنفيذ هو nullptr. |
| [GetHashCode](./gethashcode/) | يحصل على رمز التجزئة. |
| [Equals](./equals/) | يحدد ما إذا كانت هذه الحالة لها نفس القيمة مثل كائن LineFormat المحدد الآخر. |
| [GetCompoundType](./getcompoundtype/) | يحدد نوع مركب الخط. |
| [SetCompoundType](./setcompoundtype/) | يحدد نوع مركب الخط. |
| [GetDashStyle](./getdashstyle/) | يحدد نوع الخط المتقطع. |
| [SetDashStyle](./setdashstyle/) | يحدد نوع الخط المتقطع. |
| [GetCapType](./getcaptype/) | يحدد نهايات القُبُعات. |
| [SetCapType](./setcaptype/) | يحدد نهايات القُبُعات. |
| [GetJoinType](./getjointype/) | يحدد نوع وصل الخط. |
| [SetJoinType](./setjointype/) | يحدد نوع وصل الخط. |
| [GetBeginArrowheadStyle](./getbeginarrowheadstyle/) | يحصل ويضبط نوع السهم الابتدائي للخط. |
| [SetBeginArrowheadStyle](./setbeginarrowheadstyle/) | يحصل ويضبط نوع السهم الابتدائي للخط. |
| [GetBeginArrowheadWidth](./getbeginarrowheadwidth/) | يحصل ويضبط نوع عرض السهم الابتدائي للخط. |
| [SetBeginArrowheadWidth](./setbeginarrowheadwidth/) | يحصل ويضبط نوع عرض السهم الابتدائي للخط. |
| [GetBeginArrowheadLength](./getbeginarrowheadlength/) | يحصل ويضبط نوع طول السهم الابتدائي للخط. |
| [SetBeginArrowheadLength](./setbeginarrowheadlength/) | يحصل ويضبط نوع طول السهم الابتدائي للخط. |
| [GetEndArrowheadStyle](./getendarrowheadstyle/) | يحصل ويضبط نوع السهم النهائي للخط. |
| [SetEndArrowheadStyle](./setendarrowheadstyle/) | يحصل ويضبط نوع السهم النهائي للخط. |
| [GetEndArrowheadWidth](./getendarrowheadwidth/) | يحصل ويضبط نوع عرض السهم النهائي للخط. |
| [SetEndArrowheadWidth](./setendarrowheadwidth/) | يحصل ويضبط نوع عرض السهم النهائي للخط. |
| [GetEndArrowheadLength](./getendarrowheadlength/) | يحصل ويضبط نوع طول السهم النهائي للخط. |
| [SetEndArrowheadLength](./setendarrowheadlength/) | يحصل ويضبط نوع طول السهم النهائي للخط. |
| [GetWeight](./getweight/) | يحصل أو يضبط وزن الخط بوحدة النقاط. |
| [SetWeight](./setweight/) | يحصل أو يضبط وزن الخط بوحدة النقاط. |
| [GetFillType](./getfilltype/) | يحصل ويضبط نوع التعبئة |
| [SetFillType](./setfilltype/) | يحصل ويضبط نوع التعبئة |
| [GetTransparency](./gettransparency/) | يرجع أو يضبط درجة شفافية المنطقة كقيمة تتراوح من 0.0 (معتم) إلى 1.0 (شفاف). |
| [SetTransparency](./settransparency/) | يرجع أو يضبط درجة شفافية المنطقة كقيمة تتراوح من 0.0 (معتم) إلى 1.0 (شفاف). |
| [GetGradientFill](./getgradientfill/) | يحصل على كائن GradientFill. |
| [GetTextureFill](./gettexturefill/) | يحصل على كائن TextureFill. |
| [GetSolidFill](./getsolidfill/) | يحصل على كائن SolidFill. |
| [GetPatternFill](./getpatternfill/) | يحصل على كائن PatternFill. |
| [GetGradientColorType](./getgradientcolortype/) | يرجع نوع لون التدرج للتعبئة المحددة. |
| [GetGradientStyle](./getgradientstyle/) | يرجع نمط التدرج للتعبئة المحددة. |
| [GetGradientColor1](./getgradientcolor1/) | يرجع اللون الأول للتدرج للتعبئة المحددة. |
| [GetGradientColor2](./getgradientcolor2/) | يرجع اللون الثاني للتدرج للتعبئة المحددة. |
| [GetGradientDegree](./getgradientdegree/) | يرجع درجة التدرج للتعبئة المحددة.ينطبق فقط على Excel 2007. |
| [GetGradientVariant](./getgradientvariant/) | يرجع متغير التدرج للتعبئة المحددة.ينطبق فقط على Excel 2007. |
| [GetPresetColor](./getpresetcolor/) | يعيد لون التدرج المحدد مسبقًا للملء المحدد. |
| [SetOneColorGradient](./setonecolorgradient/) | يضبط التعبئة المحددة إلى تدرج لون واحد. ينطبق فقط على Excel 2007. |
| [SetTwoColorGradient_Color_Color_GradientStyleType_Int](./settwocolorgradient_color_color_gradientstyletype_int/) | يضبط التعبئة المحددة إلى تدرج لونين. ينطبق فقط على Excel 2007. |
| [SetPresetColorGradient](./setpresetcolorgradient/) | يضبط الملء المحدد إلى تدرج لون محدد مسبقًا. ينطبق فقط على Excel 2007. |
| [GetTexture](./gettexture/) | يمثل نوع النسيج للملء المحدد. |
| [SetTexture](./settexture/) | يمثل نوع النسيج للملء المحدد. |
| [GetPattern](./getpattern/) | يمثل نمط عرض المنطقة. |
| [SetPattern](./setpattern/) | يمثل نمط عرض المنطقة. |
| [GetPictureFormatType](./getpictureformattype/) | يحصل على ويضبط نوع تنسيق الصورة. |
| [SetPictureFormatType](./setpictureformattype/) | يحصل على ويضبط نوع تنسيق الصورة. |
| [GetScale](./getscale/) | يحصل على ويضبط مقياس تنسيق الصورة. |
| [SetScale](./setscale/) | يحصل على ويضبط مقياس تنسيق الصورة. |
| [GetImageData](./getimagedata/) | يحصل على بيانات الصورة ويضبطها. |
| [SetImageData](./setimagedata/) | يحصل على بيانات الصورة ويضبطها. |
