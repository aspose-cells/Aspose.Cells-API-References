---
title: "PageSetup Class"
linktitle: "PageSetup"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "PageSetup class. يغلف الكائن الذي يمثل pagesetup في Go."
type: docs
weight: 200
url: /ar/go-cpp/pagesetup/
---

## PageSetup class

يغلف الكائن الذي يمثل وصف إعداد الصفحة. يحتوي كائن PageSetup على جميع خيارات إعداد الصفحة.

```go

type PageSetup struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |

## طرق

| طريقة | الوصف |
| --- | --- |
| [IsNull](./isnull/) | يتحقق مما إذا كان كائن التنفيذ هو nullptr. |
| [GetODSPageBackground](./getodspagebackground/) | يحصل على خلفية ODS. |
| [Copy](./copy/) | ينسخ إعداد page setup. |
| [GetPrintArea](./getprintarea/) | يمثل النطاق الذي سيتم طباعته. |
| [SetPrintArea](./setprintarea/) | يمثل النطاق الذي سيتم طباعته. |
| [GetPrintTitleColumns](./getprinttitlecolumns/) | يمثل الأعمدة التي تحتوي على الخلايا التي ستُعاد على الجانب الأيسر من كل صفحة. |
| [SetPrintTitleColumns](./setprinttitlecolumns/) | يمثل الأعمدة التي تحتوي على الخلايا التي ستُعاد على الجانب الأيسر من كل صفحة. |
| [GetPrintTitleRows](./getprinttitlerows/) | يمثل الصفوف التي تحتوي على الخلايا التي ستُعاد في أعلى كل صفحة. |
| [SetPrintTitleRows](./setprinttitlerows/) | يمثل الصفوف التي تحتوي على الخلايا التي ستُعاد في أعلى كل صفحة. |
| [GetBlackAndWhite](./getblackandwhite/) | يمثل ما إذا كانت عناصر المستند ستُطبع بالأبيض والأسود. |
| [SetBlackAndWhite](./setblackandwhite/) | يمثل ما إذا كانت عناصر المستند ستُطبع بالأبيض والأسود. |
| [GetCenterHorizontally](./getcenterhorizontally/) | يمثل ما إذا كانت الورقة تُطبع مركزة أفقياً. |
| [SetCenterHorizontally](./setcenterhorizontally/) | يمثل ما إذا كانت الورقة تُطبع مركزة أفقياً. |
| [GetCenterVertically](./getcentervertically/) | يمثل ما إذا تم طباعة الورقة مركزة عموديًا. |
| [SetCenterVertically](./setcentervertically/) | يمثل ما إذا تم طباعة الورقة مركزة عموديًا. |
| [GetPrintDraft](./getprintdraft/) | يمثل ما إذا سيتم طباعة الورقة بدون رسومات. |
| [SetPrintDraft](./setprintdraft/) | يمثل ما إذا سيتم طباعة الورقة بدون رسومات. |
| [GetFooterMargin](./getfootermargin/) | يمثل المسافة من أسفل الصفحة إلى التذييل، بوحدة السنتيمترات. |
| [SetFooterMargin](./setfootermargin/) | يمثل المسافة من أسفل الصفحة إلى التذييل، بوحدة السنتيمترات. |
| [GetFooterMarginInch](./getfootermargininch/) | يمثل المسافة من أسفل الصفحة إلى التذييل، بوحدة البوصات. |
| [SetFooterMarginInch](./setfootermargininch/) | يمثل المسافة من أسفل الصفحة إلى التذييل، بوحدة البوصات. |
| [GetHeaderMargin](./getheadermargin/) | يمثل المسافة من أعلى الصفحة إلى الترويسة، بوحدة السنتيمترات. |
| [SetHeaderMargin](./setheadermargin/) | يمثل المسافة من أعلى الصفحة إلى الترويسة، بوحدة السنتيمترات. |
| [GetHeaderMarginInch](./getheadermargininch/) | يمثل المسافة من أعلى الصفحة إلى الترويسة، بوحدة البوصات. |
| [SetHeaderMarginInch](./setheadermargininch/) | يمثل المسافة من أعلى الصفحة إلى الترويسة، بوحدة البوصات. |
| [GetPrinterSettings](./getprintersettings/) | يحصل على إعدادات الطابعة الافتراضية ويضبطها. |
| [SetPrinterSettings](./setprintersettings/) | يحصل على إعدادات الطابعة الافتراضية ويضبطها. |
| [GetLeftMargin](./getleftmargin/) | يمثل حجم الهامش الأيسر، بوحدة السنتيمترات. |
| [SetLeftMargin](./setleftmargin/) | يمثل حجم الهامش الأيسر، بوحدة السنتيمترات. |
| [GetLeftMarginInch](./getleftmargininch/) | يمثل حجم الهامش الأيسر، بوحدة البوصات. |
| [SetLeftMarginInch](./setleftmargininch/) | يمثل حجم الهامش الأيسر، بوحدة البوصات. |
| [GetRightMargin](./getrightmargin/) | يمثل حجم الهامش الأيمن، بوحدة السنتيمترات. |
| [SetRightMargin](./setrightmargin/) | يمثل حجم الهامش الأيمن، بوحدة السنتيمترات. |
| [GetRightMarginInch](./getrightmargininch/) | يمثل حجم الهامش الأيمن، بوحدة البوصات. |
| [SetRightMarginInch](./setrightmargininch/) | يمثل حجم الهامش الأيمن، بوحدة البوصات. |
| [GetTopMargin](./gettopmargin/) | يمثل حجم الهامش العلوي، بوحدة السنتيمترات. |
| [SetTopMargin](./settopmargin/) | يمثل حجم الهامش العلوي، بوحدة السنتيمترات. |
| [GetTopMarginInch](./gettopmargininch/) | يمثل حجم الهامش العلوي، بوحدة البوصات. |
| [SetTopMarginInch](./settopmargininch/) | يمثل حجم الهامش العلوي، بوحدة البوصات. |
| [GetBottomMargin](./getbottommargin/) | يمثل حجم الهامش السفلي، بوحدة السنتيمترات. |
| [SetBottomMargin](./setbottommargin/) | يمثل حجم الهامش السفلي، بوحدة السنتيمترات. |
| [GetBottomMarginInch](./getbottommargininch/) | يمثل حجم الهامش السفلي، بوحدة البوصات. |
| [SetBottomMarginInch](./setbottommargininch/) | يمثل حجم الهامش السفلي، بوحدة البوصات. |
| [GetFirstPageNumber](./getfirstpagenumber/) | يمثل رقم الصفحة الأولى التي سيتم استخدامها عند طباعة هذه الورقة. |
| [SetFirstPageNumber](./setfirstpagenumber/) | يمثل رقم الصفحة الأولى التي سيتم استخدامها عند طباعة هذه الورقة. |
| [SetFitToPages](./setfittopages/) | يضبط عدد الصفحات التي سيتم تحجيم ورقة العمل إليها عند طباعتها. |
| [GetFitToPagesTall](./getfittopagestall/) | يمثل عدد الصفحات ارتفاعًا التي سيتم تحجيم ورقة العمل إليها عند طباعتها. القيمة الافتراضية هي 1. |
| [SetFitToPagesTall](./setfittopagestall/) | يمثل عدد الصفحات ارتفاعًا التي سيتم تحجيم ورقة العمل إليها عند طباعتها. القيمة الافتراضية هي 1. |
| [GetFitToPagesWide](./getfittopageswide/) | يمثل عدد الصفحات عرضًا التي سيتم تحجيم ورقة العمل إليها عند طباعتها. القيمة الافتراضية هي 1. |
| [SetFitToPagesWide](./setfittopageswide/) | يمثل عدد الصفحات عرضًا التي سيتم تحجيم ورقة العمل إليها عند طباعتها. القيمة الافتراضية هي 1. |
| [IsPercentScale](./ispercentscale/) | إذا كانت هذه الخاصية False، فإن خاصيتي FitToPagesWide وFitToPagesTall تتحكمان في كيفية تحجيم ورقة العمل. |
| [SetIsPercentScale](./setispercentscale/) | إذا كانت هذه الخاصية False، فإن خاصيتي FitToPagesWide وFitToPagesTall تتحكمان في كيفية تحجيم ورقة العمل. |
| [GetOrder](./getorder/) | يمثل الترتيب الذي يستخدمه Microsoft Excel لترقيم الصفحات عند طباعة ورقة عمل كبيرة. |
| [SetOrder](./setorder/) | يمثل الترتيب الذي يستخدمه Microsoft Excel لترقيم الصفحات عند طباعة ورقة عمل كبيرة. |
| [IsAutomaticPaperSize](./isautomaticpapersize/) | يشير إلى ما إذا كان حجم الورق تلقائيًا. |
| [GetPaperSize](./getpapersize/) | يمثل حجم الورق. |
| [SetPaperSize](./setpapersize/) | يمثل حجم الورق. |
| [GetPaperWidth](./getpaperwidth/) | يحصل على عرض الورق بوحدة البوصات، مع مراعاة اتجاه الصفحة. |
| [GetPaperHeight](./getpaperheight/) | يحصل على ارتفاع الورق بوحدة البوصات، مع مراعاة اتجاه الصفحة. |
| [CustomPaperSize](./custompapersize/) | يضبط حجم الورق المخصص، بوحدة البوصة. |
| [GetOrientation](./getorientation/) | يمثل اتجاه طباعة الصفحة. |
| [SetOrientation](./setorientation/) | يمثل اتجاه طباعة الصفحة. |
| [GetPrintComments](./getprintcomments/) | يمثل طريقة طباعة التعليقات مع الورقة. |
| [SetPrintComments](./setprintcomments/) | يمثل طريقة طباعة التعليقات مع الورقة. |
| [GetPrintErrors](./getprinterrors/) | يحدد نوع خطأ الطباعة المعروض. |
| [SetPrintErrors](./setprinterrors/) | يحدد نوع خطأ الطباعة المعروض. |
| [GetPrintHeadings](./getprintheadings/) | يمثل ما إذا كانت عناوين الصفوف والأعمدة مطبوعة مع هذه الصفحة. |
| [SetPrintHeadings](./setprintheadings/) | يمثل ما إذا كانت عناوين الصفوف والأعمدة مطبوعة مع هذه الصفحة. |
| [GetPrintGridlines](./getprintgridlines/) | يمثل ما إذا كانت خطوط شبكة الخلايا مطبوعة على الصفحة. |
| [SetPrintGridlines](./setprintgridlines/) | يمثل ما إذا كانت خطوط شبكة الخلايا مطبوعة على الصفحة. |
| [GetZoom](./getzoom/) | يمثل عامل التحجيم بالنسبة المئوية. يجب أن يكون بين 10 و 400. |
| [SetZoom](./setzoom/) | يمثل عامل التحجيم بالنسبة المئوية. يجب أن يكون بين 10 و 400. |
| [IsAutoFirstPageNumber](./isautofirstpagenumber/) | يشير إلى ما إذا كان رقم الصفحة الأول يُعيّن تلقائيًا. |
| [SetIsAutoFirstPageNumber](./setisautofirstpagenumber/) | يشير إلى ما إذا كان رقم الصفحة الأول يُعيّن تلقائيًا. |
| [GetPrintQuality](./getprintquality/) | يمثل جودة الطباعة. |
| [SetPrintQuality](./setprintquality/) | يمثل جودة الطباعة. |
| [GetPrintCopies](./getprintcopies/) | يحصل على عدد النسخ للطباعة ويضبطه. |
| [SetPrintCopies](./setprintcopies/) | يحصل على عدد النسخ للطباعة ويضبطه. |
| [ClearHeaderFooter](./clearheaderfooter/) | يمسح إعدادات الرأس والتذييل. |
| [GetHeader](./getheader/) | يحصل على نص برمجي ينسق رأس ملف Excel. |
| [GetCommands](./getcommands/) | يحصل على جميع أوامر الرأس أو التذييل. |
| [GetFooter](./getfooter/) | يحصل على نص برمجي ينسق تذييل ملف Excel. |
| [SetHeader](./setheader/) | يضبط نصًا برمجيًا ينسق رأس ملف Excel. |
| [SetFooter](./setfooter/) | يضبط نصًا برمجيًا ينسق تذييل ملف Excel. |
| [SetEvenHeader](./setevenheader/) | يضبط نصًا برمجيًا ينسق رأس الصفحات الزوجية في ملف Excel. يؤثر فقط في Excel 2007 عندما تكون IsHFDiffOddEven صحيحة. |
| [GetEvenHeader](./getevenheader/) | يحصل على نص برمجي ينسق رأس الصفحات الزوجية في ملف Excel. |
| [SetEvenFooter](./setevenfooter/) | يضبط نصًا برمجيًا ينسق تذييل الصفحات الزوجية في ملف Excel. يؤثر فقط في Excel 2007 عندما تكون IsHFDiffOddEven صحيحة. |
| [GetEvenFooter](./getevenfooter/) | يحصل على نص برمجي ينسق تذييل الصفحات الزوجية في ملف Excel. |
| [SetFirstPageHeader](./setfirstpageheader/) | يضبط نصًا برمجيًا ينسق رأس الصفحة الأولى في ملف Excel. يؤثر فقط في Excel 2007 عندما تكون IsHFDiffFirst صحيحة. |
| [GetFirstPageHeader](./getfirstpageheader/) | يحصل على نص برمجي ينسق رأس الصفحة الأولى في ملف Excel. |
| [SetFirstPageFooter](./setfirstpagefooter/) | يضبط نصًا برمجيًا ينسق تذييل الصفحة الأولى في ملف Excel. |
| [GetFirstPageFooter](./getfirstpagefooter/) | يحصل على نص برمجي ينسق تذييل الصفحة الأولى في ملف Excel. |
| [IsHFDiffOddEven](./ishfdiffoddeven/) | صحيح يعني أن رأس/تذييل الصفحات الفردية يختلف عن الصفحات الفردية. |
| [SetIsHFDiffOddEven](./setishfdiffoddeven/) | صحيح يعني أن رأس/تذييل الصفحات الفردية يختلف عن الصفحات الفردية. |
| [IsHFDiffFirst](./ishfdifffirst/) | صحيح يعني أن رأس/تذييل الصفحة الأولى مختلف عن باقي الصفحات. |
| [SetIsHFDiffFirst](./setishfdifffirst/) | صحيح يعني أن رأس/تذييل الصفحة الأولى مختلف عن باقي الصفحات. |
| [IsHFScaleWithDoc](./ishfscalewithdoc/) | يشير إلى ما إذا كان يتم تحجيم الرأس والتذييل مع تحجيم المستند. ينطبق فقط على Excel 2007. |
| [SetIsHFScaleWithDoc](./setishfscalewithdoc/) | يشير إلى ما إذا كان يتم تحجيم الرأس والتذييل مع تحجيم المستند. ينطبق فقط على Excel 2007. |
| [IsHFAlignMargins](./ishfalignmargins/) | يشير إلى ما إذا كانت هوامش الرأس والتذييل محاذاة مع هوامش الصفحة. إذا كانت هذه الخاصية صحيحة، سيتم محاذاة رأس وتذييل اليسار مع الهامش الأيسر، ورأس وتذييل اليمين مع الهامش الأيمن. يتم تمكين هذا الخيار بشكل افتراضي. |
| [SetIsHFAlignMargins](./setishfalignmargins/) | يشير إلى ما إذا كانت هوامش الرأس والتذييل محاذاة مع هوامش الصفحة. إذا كانت هذه الخاصية صحيحة، سيتم محاذاة رأس وتذييل اليسار مع الهامش الأيسر، ورأس وتذييل اليمين مع الهامش الأيمن. يتم تمكين هذا الخيار بشكل افتراضي. |
| [SetHeaderPicture](./setheaderpicture/) | يضبط صورة في رأس ورقة العمل. |
| [SetFooterPicture](./setfooterpicture/) | يضبط صورة في تذييل ورقة العمل. |
| [SetPicture](./setpicture/) | يضبط صورة في رأس/تذييل ورقة العمل. |
| [GetPicture_Bool_Int](./getpicture_bool_int/) | يحصل على كائن Picture للرأس / التذييل. |
| [GetPicture_Bool_Bool_Bool_Int](./getpicture_bool_bool_bool_int/) | يحصل على كائن Picture للرأس / التذييل. |
