---
title: "فئة CheckBox"
linktitle: "مربع اختيار"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة CheckBox. تغلف الكائن الذي يمثل مربع الاختيار في Go."
type: docs
weight: 200
url: /ar/go-cpp/checkbox/
---

## CheckBox class

يمثل كائن مربع اختيار في ورقة العمل.

```go

type CheckBox struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |
| [NewCheckBox](./newcheckbox/) | يُنشئ من كائن أب. |

## طرق

| طريقة | الوصف |
| --- | --- |
| [IsNull](./isnull/) | يتحقق مما إذا كان كائن التنفيذ هو nullptr. |
| [GetValue](./getvalue/) | يشير إلى ما إذا كان مربع الاختيار محددًا أم لا. |
| [SetValue](./setvalue/) | يشير إلى ما إذا كان مربع الاختيار محددًا أم لا. |
| [GetCheckedValue](./getcheckedvalue/) | يحصل أو يضبط قيمة مربع الاختيار. |
| [SetCheckedValue](./setcheckedvalue/) | يحصل أو يضبط قيمة مربع الاختيار. |
| [GetShadow](./getshadow/) | يشير إلى ما إذا كان صندوق القائمة يحتوي على تظليل ثلاثي الأبعاد. |
| [SetShadow](./setshadow/) | يشير إلى ما إذا كان صندوق القائمة يحتوي على تظليل ثلاثي الأبعاد. |
| [GetMacroName](./getmacroname/) | يحصل ويعيّن اسم الماكرو. |
| [SetMacroName](./setmacroname/) | يحصل ويعيّن اسم الماكرو. |
| [IsEquation](./isequation/) | يشير إلى ما إذا كان الشكل يحتوي فقط على معادلة. |
| [IsSmartArt](./issmartart/) | يشير إلى ما إذا كان الشكل فنًا ذكيًا. |
| [ToFrontOrBack](./tofrontorback/) | ينقل الشكل إلى الأمام أو يرسل الشكل إلى الخلف. |
| [GetZOrderPosition](./getzorderposition/) | يعيد موضع الشكل في ترتيب الـ z. |
| [SetZOrderPosition](./setzorderposition/) | يعيد موضع الشكل في ترتيب الـ z. |
| [GetName](./getname/) | يحصل على اسم الشكل ويضبطه. |
| [SetName](./setname/) | يحصل على اسم الشكل ويضبطه. |
| [GetAlternativeText](./getalternativetext/) | يعيد أو يضبط النص الوصفي (البديل) لكائن Shape. |
| [SetAlternativeText](./setalternativetext/) | يعيد أو يضبط النص الوصفي (البديل) لكائن Shape. |
| [GetTitle](./gettitle/) | يحدد العنوان (التسمية) لكائن الشكل الحالي. |
| [SetTitle](./settitle/) | يحدد العنوان (التسمية) لكائن الشكل الحالي. |
| [GetLine](./getline/) | يحصل على نمط الخط |
| [GetFill](./getfill/) | يعيد كائن FillFormat يحتوي على خصائص تنسيق التعبئة للشكل المحدد. |
| [GetShadowEffect](./getshadoweffect/) | يمثل كائن Drawing.ShadowEffect يحدد تأثير الظل لعنصر المخطط أو الشكل. |
| [GetReflection](./getreflection/) | يمثل كائن ReflectionEffect يحدد تأثير الانعكاس لعنصر المخطط أو الشكل. |
| [GetGlow](./getglow/) | يمثل كائن GlowEffect يحدد تأثير التوهج لعنصر المخطط أو الشكل. |
| [GetSoftEdges](./getsoftedges/) | يحصل ويضبط نصف قطر الضبابية لتطبيقه على الحواف بوحدة النقاط. |
| [SetSoftEdges](./setsoftedges/) | يحصل ويضبط نصف قطر الضبابية لتطبيقه على الحواف بوحدة النقاط. |
| [GetThreeDFormat](./getthreedformat/) | يحصل ويضبط تنسيق ثلاثي الأبعاد للشكل. |
| [GetFormatPicture](./getformatpicture/) | يحصل ويضبط خيارات تنسيق الصورة. |
| [IsHidden](./ishidden/) | يشير إلى ما إذا كان الكائن مرئيًا. |
| [SetIsHidden](./setishidden/) | يشير إلى ما إذا كان الكائن مرئيًا. |
| [IsAspectRatioLocked](./isaspectratiolocked/) | صحيح يعني أن نسبة أبعاد الشكل مقفلة. |
| [SetIsAspectRatioLocked](./setisaspectratiolocked/) | صحيح يعني أن نسبة أبعاد الشكل مقفلة. |
| [GetLockedProperty](./getlockedproperty/) | يحصل على قيمة الخاصية المقفلة. |
| [SetLockedProperty](./setlockedproperty/) | يضبط الخاصية المقفلة. |
| [GetRotationAngle](./getrotationangle/) | يحصل ويضبط دوران الشكل. |
| [SetRotationAngle](./setrotationangle/) | يحصل ويضبط دوران الشكل. |
| [AddHyperlink](./addhyperlink/) | يضيف ارتباطًا تشعبيًا إلى الشكل. |
| [RemoveHyperlink](./removehyperlink/) | يزيل الارتباط التشعبي للشكل. |
| [GetHyperlink](./gethyperlink/) | يحصل على الارتباط التشعبي للشكل. |
| [MoveToRange](./movetorange/) | ينقل الشكل إلى نطاق محدد. |
| [AlignTopRightCorner](./aligntoprightcorner/) | ينقل الصورة إلى الزاوية العليا اليمنى. |
| [GetId](./getid/) | يحصل على معرف هذا الشكل. |
| [GetSpid](./getspid/) | يحدد معرف سلسلة اختياري يمكن للتطبيق استخدامه لتحديد الشكل المحدد. |
| [GetSpt](./getspt/) | يحدد رقمًا اختياريًا يمكن للتطبيق استخدامه لربط الشكل المحدد بنوع شكل معرف. |
| [GetWorksheet](./getworksheet/) | يحصل على كائن Aspose.Cells.Worksheet الذي يحتوي على هذا الشكل. |
| [IsGroup](./isgroup/) | يشير إلى ما إذا كان هذا الشكل شكل مجموعة. |
| [IsInGroup](./isingroup/) | يشير إلى ما إذا كان الشكل مجمعًا. |
| [IsWordArt](./iswordart/) | يشير إلى ما إذا كان هذا الشكل فن كلمة. |
| [GetTextEffect](./gettexteffect/) | يعيد كائن TextEffectFormat الذي يحتوي على خصائص تنسيق تأثير النص للشكل المحدد. ينطبق على كائنات Shape التي تمثل WordArt. |
| [IsLocked](./islocked/) | True يعني أن الكائن لا يمكن تعديله عندما تكون الورقة محمية. لاحظ أن هذه القيمة ذات معنى فقط إذا كانت ورقة العمل أو الكائنات في ورقة العمل محمية. |
| [SetIsLocked](./setislocked/) | True يعني أن الكائن لا يمكن تعديله عندما تكون الورقة محمية. لاحظ أن هذه القيمة ذات معنى فقط إذا كانت ورقة العمل أو الكائنات في ورقة العمل محمية. |
| [IsPrintable](./isprintable/) | يشير إلى ما إذا كان الكائن قابلًا للطباعة. إذا كان False، فلن يتم طباعة هذا الشكل عند الطباعة. |
| [SetIsPrintable](./setisprintable/) | يشير إلى ما إذا كان الكائن قابلًا للطباعة. إذا كان False، فلن يتم طباعة هذا الشكل عند الطباعة. |
| [GetMsoDrawingType](./getmsodrawingtype/) | يحصل على نوع الرسم. |
| [GetAutoShapeType](./getautoshapetype/) | يحصل على نوع الشكل التلقائي ويضبطه. |
| [SetAutoShapeType](./setautoshapetype/) | يحصل على نوع الشكل التلقائي ويضبطه. |
| [GetAnchorType](./getanchortype/) | يحصل على نوع عنصر نائب مرساة الشكل ويضبطه. |
| [SetAnchorType](./setanchortype/) | يحصل على نوع عنصر نائب مرساة الشكل ويضبطه. |
| [GetPlacement](./getplacement/) | يمثل الطريقة التي يتم بها إرفاق كائن الرسم بالخلايا تحته. الخاصية تتحكم في وضع الكائن على ورقة العمل. |
| [SetPlacement](./setplacement/) | يمثل الطريقة التي يتم بها إرفاق كائن الرسم بالخلايا تحته. الخاصية تتحكم في وضع الكائن على ورقة العمل. |
| [GetUpperLeftRow](./getupperleftrow/) | يمثل فهرس الصف العلوي. |
| [SetUpperLeftRow](./setupperleftrow/) | يمثل فهرس الصف العلوي. |
| [GetUpperDeltaY](./getupperdeltay/) | يحصل على إزاحة الشكل العمودية من صف الزاوية العلوية اليسرى أو يضبطها. |
| [SetUpperDeltaY](./setupperdeltay/) | يحصل على إزاحة الشكل العمودية من صف الزاوية العلوية اليسرى أو يضبطها. |
| [GetUpperLeftColumn](./getupperleftcolumn/) | يمثل فهرس عمود الزاوية العلوية اليسرى. |
| [SetUpperLeftColumn](./setupperleftcolumn/) | يمثل فهرس عمود الزاوية العلوية اليسرى. |
| [GetUpperDeltaX](./getupperdeltax/) | يحصل على إزاحة الشكل الأفقية من عمود الزاوية العلوية اليسرى أو يضبطها. |
| [SetUpperDeltaX](./setupperdeltax/) | يحصل على إزاحة الشكل الأفقية من عمود الزاوية العلوية اليسرى أو يضبطها. |
| [GetLowerRightRow](./getlowerrightrow/) | يمثل فهرس صف الزاوية السفلية اليمنى. |
| [SetLowerRightRow](./setlowerrightrow/) | يمثل فهرس صف الزاوية السفلية اليمنى. |
| [GetLowerDeltaY](./getlowerdeltay/) | يحصل على إزاحة الشكل العمودية من صف الزاوية السفلية اليمنى أو يضبطها. |
| [SetLowerDeltaY](./setlowerdeltay/) | يحصل على إزاحة الشكل العمودية من صف الزاوية السفلية اليمنى أو يضبطها. |
| [GetLowerRightColumn](./getlowerrightcolumn/) | يمثل فهرس عمود الزاوية السفلية اليمنى. |
| [SetLowerRightColumn](./setlowerrightcolumn/) | يمثل فهرس عمود الزاوية السفلية اليمنى. |
| [GetLowerDeltaX](./getlowerdeltax/) | يحصل على إزاحة الشكل الأفقية من عمود الزاوية السفلية اليمنى أو يضبطها. |
| [SetLowerDeltaX](./setlowerdeltax/) | يحصل على إزاحة الشكل الأفقية من عمود الزاوية السفلية اليمنى أو يضبطها. |
| [GetRight](./getright/) | يمثل عرض إزاحة الشكل الأفقية من عمود الزاوية السفلية اليمنى، بوحدة البكسل. |
| [SetRight](./setright/) | يمثل عرض إزاحة الشكل الأفقية من عمود الزاوية السفلية اليمنى، بوحدة البكسل. |
| [GetBottom](./getbottom/) | يمثل عرض إزاحة الشكل العمودية من صف الزاوية السفلية السفلية، بوحدة البكسل. |
| [SetBottom](./setbottom/) | يمثل عرض إزاحة الشكل العمودية من صف الزاوية السفلية السفلية، بوحدة البكسل. |
| [GetWidth](./getwidth/) | يمثل عرض الشكل، بوحدة البكسل. |
| [SetWidth](./setwidth/) | يمثل عرض الشكل، بوحدة البكسل. |
| [GetWidthInch](./getwidthinch/) | يمثل عرض الشكل، بوحدة البوصة. |
| [SetWidthInch](./setwidthinch/) | يمثل عرض الشكل، بوحدة البوصة. |
| [GetWidthPt](./getwidthpt/) | يمثل عرض الشكل، بوحدة النقطة. |
| [SetWidthPt](./setwidthpt/) | يمثل عرض الشكل، بوحدة النقطة. |
| [GetWidthCM](./getwidthcm/) | يمثل عرض الشكل، بوحدة السنتيمتر. |
| [SetWidthCM](./setwidthcm/) | يمثل عرض الشكل، بوحدة السنتيمتر. |
| [GetHeight](./getheight/) | يمثل ارتفاع الشكل، بوحدة البكسل. |
| [SetHeight](./setheight/) | يمثل ارتفاع الشكل، بوحدة البكسل. |
| [GetHeightInch](./getheightinch/) | يمثل ارتفاع الشكل، بوحدة البوصة. |
| [SetHeightInch](./setheightinch/) | يمثل ارتفاع الشكل، بوحدة البوصة. |
| [GetHeightPt](./getheightpt/) | يمثل ارتفاع الشكل، بوحدة النقاط. |
| [SetHeightPt](./setheightpt/) | يمثل ارتفاع الشكل، بوحدة النقاط. |
| [GetHeightCM](./getheightcm/) | يمثل ارتفاع الشكل، بوحدة السنتيمتر. |
| [SetHeightCM](./setheightcm/) | يمثل ارتفاع الشكل، بوحدة السنتيمتر. |
| [GetLeft](./getleft/) | يمثل الإزاحة الأفقية للشكل من العمود الأيسر، بوحدة البكسل. |
| [SetLeft](./setleft/) | يمثل الإزاحة الأفقية للشكل من العمود الأيسر، بوحدة البكسل. |
| [GetLeftInch](./getleftinch/) | يمثل الإزاحة الأفقية للشكل من العمود الأيسر، بوحدة البوصة. |
| [SetLeftInch](./setleftinch/) | يمثل الإزاحة الأفقية للشكل من العمود الأيسر، بوحدة البوصة. |
| [GetLeftCM](./getleftcm/) | يمثل الإزاحة الأفقية للشكل من العمود الأيسر، بوحدة السنتيمتر. |
| [SetLeftCM](./setleftcm/) | يمثل الإزاحة الأفقية للشكل من العمود الأيسر، بوحدة السنتيمتر. |
| [GetTop](./gettop/) | يمثل الإزاحة العمودية للشكل من الصف العلوي، بوحدة البكسل. |
| [SetTop](./settop/) | يمثل الإزاحة العمودية للشكل من الصف العلوي، بوحدة البكسل. |
| [GetTopInch](./gettopinch/) | يمثل الإزاحة العمودية للشكل من الصف العلوي، بوحدة البوصة. |
| [SetTopInch](./settopinch/) | يمثل الإزاحة العمودية للشكل من الصف العلوي، بوحدة البوصة. |
| [GetTopCM](./gettopcm/) | يمثل الإزاحة العمودية للشكل من الصف العلوي، بوحدة السنتيمتر. |
| [SetTopCM](./settopcm/) | يمثل الإزاحة العمودية للشكل من الصف العلوي، بوحدة السنتيمتر. |
| [GetTopToCorner](./gettoptocorner/) | يحصل ويضبط الإزاحة العمودية للشكل من الحد العلوي لورقة العمل، بوحدة البكسل. |
| [SetTopToCorner](./settoptocorner/) | يحصل ويضبط الإزاحة العمودية للشكل من الحد العلوي لورقة العمل، بوحدة البكسل. |
| [GetLeftToCorner](./getlefttocorner/) | يحصل ويضبط الإزاحة الأفقية للشكل من الحد الأيسر لورقة العمل. |
| [SetLeftToCorner](./setlefttocorner/) | يحصل ويضبط الإزاحة الأفقية للشكل من الحد الأيسر لورقة العمل. |
| [GetX](./getx/) | يحصل ويضبط الإزاحة الأفقية للشكل من الحد الأيسر لورقة العمل، بوحدة البكسل. |
| [SetX](./setx/) | يحصل ويضبط الإزاحة الأفقية للشكل من الحد الأيسر لورقة العمل، بوحدة البكسل. |
| [GetY](./gety/) | يحصل ويضبط الإزاحة العمودية للشكل من الحد العلوي لورقة العمل، بوحدة البكسل. |
| [SetY](./sety/) | يحصل ويضبط الإزاحة العمودية للشكل من الحد العلوي لورقة العمل، بوحدة البكسل. |
| [GetWidthScale](./getwidthscale/) | يحصل ويضبط مقياس العرض، بوحدة النسبة المئوية لعرض الصورة الأصلية. إذا لم يكن الشكل صورة، فإن خاصية WidthScale تُعيد 100 فقط; |
| [SetWidthScale](./setwidthscale/) | يحصل ويضبط مقياس العرض، بوحدة النسبة المئوية لعرض الصورة الأصلية. إذا لم يكن الشكل صورة، فإن خاصية WidthScale تُعيد 100 فقط; |
| [GetHeightScale](./getheightscale/) | يحصل ويضبط مقياس الارتفاع، بوحدة النسبة المئوية لارتفاع الصورة الأصلية. إذا لم يكن الشكل صورة، فإن خاصية HeightScale تُعيد 100 فقط; |
| [SetHeightScale](./setheightscale/) | يحصل ويضبط مقياس الارتفاع، بوحدة النسبة المئوية لارتفاع الصورة الأصلية. إذا لم يكن الشكل صورة، فإن خاصية HeightScale تُعيد 100 فقط; |
| [GetTopInShape](./gettopinshape/) | يمثل الإزاحة العمودية للشكل من الحد العلوي للشكل الأب، بوحدة 1/4000 من ارتفاع الشكل الأب. |
| [SetTopInShape](./settopinshape/) | يمثل الإزاحة العمودية للشكل من الحد العلوي للشكل الأب، بوحدة 1/4000 من ارتفاع الشكل الأب. |
| [GetLeftInShape](./getleftinshape/) | يمثل الإزاحة الأفقية للشكل من الحد الأيسر للشكل الأب، بوحدة 1/4000 من عرض الشكل الأب. |
| [SetLeftInShape](./setleftinshape/) | يمثل الإزاحة الأفقية للشكل من الحد الأيسر للشكل الأب، بوحدة 1/4000 من عرض الشكل الأب. |
| [GetWidthInShape](./getwidthinshape/) | يمثل عرض الشكل، بوحدة 1/4000 من الشكل الأب. |
| [SetWidthInShape](./setwidthinshape/) | يمثل عرض الشكل، بوحدة 1/4000 من الشكل الأب. |
| [GetHeightInShape](./getheightinshape/) | يمثل الإزاحة العمودية للشكل من الحد العلوي للشكل الأب، بوحدة 1/4000 من ارتفاع الشكل الأب.. |
| [SetHeightInShape](./setheightinshape/) | يمثل الإزاحة العمودية للشكل من الحد العلوي للشكل الأب، بوحدة 1/4000 من ارتفاع الشكل الأب.. |
| [GetGroup](./getgroup/) | يحصل على الشكل الجماعي الذي يحتوي هذا الشكل. |
| [GetType](./gettype/) | يحصل على نوع الشكل التلقائي. |
| [GetHasLine](./gethasline/) | يحصل ويضبط ما إذا كان حد الخط للشكل مرئيًا. |
| [SetHasLine](./sethasline/) | يحصل ويضبط ما إذا كان حد الخط للشكل مرئيًا. |
| [IsFilled](./isfilled/) | يشير إلى ما إذا كان تنسيق التعبئة مرئيًا. |
| [SetIsFilled](./setisfilled/) | يشير إلى ما إذا كان تنسيق التعبئة مرئيًا. |
| [IsFlippedHorizontally](./isflippedhorizontally/) | يحصل ويضبط ما إذا كان الشكل مقلوبًا أفقيًا. |
| [SetIsFlippedHorizontally](./setisflippedhorizontally/) | يحصل ويضبط ما إذا كان الشكل مقلوبًا أفقيًا. |
| [IsFlippedVertically](./isflippedvertically/) | يحصل ويضبط ما إذا كان الشكل مقلوبًا عموديًا . |
| [SetIsFlippedVertically](./setisflippedvertically/) | يحصل ويضبط ما إذا كان الشكل مقلوبًا عموديًا . |
| [GetActualLowerRightRow](./getactuallowerrightrow/) | احصل على الصف السفلي الفعلي. |
| [GetConnectionPoints](./getconnectionpoints/) | احصل على نقاط الاتصال |
| [ToImage_ImageType](./toimage_imagetype/) | ينشئ صورة الشكل ويحفظها إلى تدفق بالتنسيق المحدد. |
| [GetRelativeToOriginalPictureSize](./getrelativetooriginalpicturesize/) | يشير إلى ما إذا كان الشكل نسبيًا لحجم الصورة الأصلي. |
| [SetRelativeToOriginalPictureSize](./setrelativetooriginalpicturesize/) | يشير إلى ما إذا كان الشكل نسبيًا لحجم الصورة الأصلي. |
| [GetLinkedCell](./getlinkedcell/) | يحصل أو يضبط نطاق ورقة العمل المرتبط بقيمة التحكم. |
| [SetLinkedCell_String](./setlinkedcell_string/) | يحصل أو يضبط نطاق ورقة العمل المرتبط بقيمة التحكم. |
| [GetInputRange](./getinputrange/) | يحصل أو يضبط نطاق ورقة العمل المستخدم لملء مربع الاختيار المحدد. |
| [SetInputRange_String](./setinputrange_string/) | يحصل أو يضبط نطاق ورقة العمل المستخدم لملء مربع الاختيار المحدد. |
| [UpdateSelectedValue](./updateselectedvalue/) | حدّث القيمة المحددة بقيمة الخلية المرتبطة. |
| [GetTextShapeType](./gettextshapetype/) | يحصل ويضبط نوع شكل النص المسبق. |
| [SetTextShapeType](./settextshapetype/) | يحصل ويضبط نوع شكل النص المسبق. |
| [GetTextBody](./gettextbody/) | يحصل ويضبط إعداد نص الشكل. |
| [GetFont](./getfont/) | يمثل خط الشكل. |
| [SetFont](./setfont/) | يمثل خط الشكل. |
| [GetTextOptions](./gettextoptions/) | يمثل خيارات نص الشكل. |
| [SetTextOptions](./settextoptions/) | يمثل خيارات نص الشكل. |
| [CalculateTextSize](./calculatetextsize/) | أعد حساب مساحة النص |
| [GetText](./gettext/) | يحصل ويضبط نص هذا الشكل. |
| [SetText](./settext/) | يحصل ويضبط نص هذا الشكل. |
| [IsRichText](./isrichtext/) | ما إذا كان النص نصًا غنيًا أم لا. |
| [GetHtmlText](./gethtmltext/) | يحصل ويضبط سلسلة HTML التي تحتوي على البيانات وبعض التنسيقات في مربع النص هذا. |
| [SetHtmlText](./sethtmltext/) | يحصل ويضبط سلسلة HTML التي تحتوي على البيانات وبعض التنسيقات في مربع النص هذا. |
| [FormatCharacters](./formatcharacters/) | يقوم بتنسيق بعض الأحرف باستخدام إعداد الخط. |
| [Characters](./characters/) | يعيد كائن Characters يمثل نطاقًا من الأحرف داخل النص. |
| [GetRichFormattings](./getrichformattings/) | يعيد جميع كائنات Characters التي تمثل نطاقًا من الأحرف داخل النص . |
| [GetTextVerticalOverflow](./gettextverticaloverflow/) | يحصل ويضبط نوع تجاوز النص العمودي للشكل الذي يحتوي على نص. |
| [SetTextVerticalOverflow](./settextverticaloverflow/) | يحصل ويضبط نوع تجاوز النص العمودي للشكل الذي يحتوي على نص. |
| [GetTextHorizontalOverflow](./gettexthorizontaloverflow/) | يحصل ويضبط نوع تجاوز النص الأفقي للشكل الذي يحتوي على نص. |
| [SetTextHorizontalOverflow](./settexthorizontaloverflow/) | يحصل ويضبط نوع تجاوز النص الأفقي للشكل الذي يحتوي على نص. |
| [IsTextWrapped](./istextwrapped/) | يحصل ويضبط نوع التفاف النص للشكل الذي يحتوي على نص. |
| [SetIsTextWrapped](./setistextwrapped/) | يحصل ويضبط نوع التفاف النص للشكل الذي يحتوي على نص. |
| [GetTextOrientationType](./gettextorientationtype/) | يحصل ويضبط نوع توجيه النص للشكل. |
| [SetTextOrientationType](./settextorientationtype/) | يحصل ويضبط نوع توجيه النص للشكل. |
| [GetTextHorizontalAlignment](./gettexthorizontalalignment/) | يحصل ويضبط نوع محاذاة النص الأفقي للشكل. |
| [SetTextHorizontalAlignment](./settexthorizontalalignment/) | يحصل ويضبط نوع محاذاة النص الأفقي للشكل. |
| [GetTextVerticalAlignment](./gettextverticalalignment/) | يحصل ويضبط نوع محاذاة النص العمودي للشكل. |
| [SetTextVerticalAlignment](./settextverticalalignment/) | يحصل ويضبط نوع محاذاة النص العمودي للشكل. |
| [GetTextDirection](./gettextdirection/) | يحصل/يضبط اتجاه تدفق النص لهذا الكائن. |
| [SetTextDirection](./settextdirection/) | يحصل/يضبط اتجاه تدفق النص لهذا الكائن. |
| [GetTextBoxOptions](./gettextboxoptions/) | يحصل على معلومات النص في الشكل |
| [GetControlData](./getcontroldata/) | يحصل على بيانات التحكم. |
| [GetActiveXControl](./getactivexcontrol/) | يحصل على عنصر التحكم ActiveX. |
| [RemoveActiveXControl](./removeactivexcontrol/) | إزالة عنصر التحكم activeX. |
| [GetPaths](./getpaths/) | يحصل على مسارات شكل هندسي مخصص. |
| [GetGeometry](./getgeometry/) | يحصل على الهندسة |
| [GetCreateId](./getcreateid/) | يحصل ويضبط معرف الإنشاء لهذا الشكل. |
| [SetCreateId](./setcreateid/) | يحصل ويضبط معرف الإنشاء لهذا الشكل. |
| [IsDecorative](./isdecorative/) | يشير إلى ما إذا كان الكائن زخرفيًا. |
| [SetIsDecorative](./setisdecorative/) | يشير إلى ما إذا كان الكائن زخرفيًا. |
| [GetActualBox](./getactualbox/) | احصل على الموضع الفعلي وحجم الشكل (بعد تطبيق الدوران، الانعكاس، إلخ). |
| [FitToTextSize](./fittotextsize/) | إعادة حساب مساحة النص المناسبة لعرض جميع محتويات النص. |
| [GetResultOfSmartArt](./getresultofsmartart/) | تحويل Smart Art إلى أشكال مجمعة. |
| [IsSameSetting](./issamesetting/) | يعيد ما إذا كان الشكل نفسه. |
