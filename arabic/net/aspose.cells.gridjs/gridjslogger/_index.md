---
title: "الفئة GridJsLogger"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.GridJs.GridJsLogger. توفر نظام تسجيل خفيف الوزن لخادم GridJs. تدعم إخراج إلى وحدة التحكم والملف مع مستويات سجل قابلة للتكوين. المستوى الافتراضي هو None. في بناء DEBUG يكون المستوى الافتراضي هو Debug ويخرج جميع الرسائل. تدعم تدوير ملفات السجل حسب اليوم/الأسبوع/الشهر."
type: docs
url: /ar/net/aspose.cells.gridjs/gridjslogger/
---
## GridJsLogger class

يوفر نظام تسجيل خفيف الوزن لخادم GridJs. يدعم إخراج إلى وحدة التحكم والملف مع مستويات سجل قابلة للتكوين. المستوى الافتراضي هو لا شيء. في بناء DEBUG، يكون المستوى الافتراضي هو Debug (يعرض جميع الرسائل). يدعم تدوير ملفات السجل حسب اليوم/الأسبوع/الشهر.

```csharp
public static class GridJsLogger
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| static [EnableConsoleOutput](../../aspose.cells.gridjs/gridjslogger/enableconsoleoutput/) { get; set; } | يحصل أو يضبط ما إذا كان سيتم إخراج رسائل السجل إلى وحدة التحكم. الافتراضي هو false. |
| static [EnableFileOutput](../../aspose.cells.gridjs/gridjslogger/enablefileoutput/) { get; set; } | يحصل أو يضبط ما إذا كان سيتم إخراج رسائل السجل إلى ملف. الافتراضي هو false. يجب استدعاء [`SetLogFile`](./setlogfile/) أو [`SetLogDirectory`](./setlogdirectory/) قبل التفعيل. |
| static [Level](../../aspose.cells.gridjs/gridjslogger/level/) { get; set; } | يحصل أو يضبط الحد الأدنى لمستوى السجل. سيتم تجاهل الرسائل التي أدنى من هذا المستوى. الافتراضي هو None. |
| static [LogFilePath](../../aspose.cells.gridjs/gridjslogger/logfilepath/) { get; } | يحصل على مسار ملف السجل الحالي، أو null إذا لم يتم ضبطه. |
| static [MaxFileSize](../../aspose.cells.gridjs/gridjslogger/maxfilesize/) { get; set; } | يحصل أو يضبط الحد الأقصى للحجم (بالبايت) لملف سجل واحد قبل التدوير. يكون فعالًا فقط عندما يكون التدوير مفعلاً. 0 يعني عدم وجود حد للحجم. الافتراضي هو 0. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| static [CloseLogFile](../../aspose.cells.gridjs/gridjslogger/closelogfile/)() | يغلق كاتب ملف السجل ويعطل إخراج الملف. |
| static [Debug](../../aspose.cells.gridjs/gridjslogger/debug/)(string) | يسجل رسالة بمستوى debug. |
| static [Error](../../aspose.cells.gridjs/gridjslogger/error/)(string) | يسجل رسالة بمستوى error. |
| static [Info](../../aspose.cells.gridjs/gridjslogger/info/)(string) | يسجل رسالة بمستوى info. |
| static [Log](../../aspose.cells.gridjs/gridjslogger/log/)(GridJsLogLevel, string) | يسجل رسالة بالمستوى المحدد. |
| static [SetLogDirectory](../../aspose.cells.gridjs/gridjslogger/setlogdirectory/#setlogdirectory)(string) | يضبط دليل السجل باستخدام استراتيجية تدوير يومية للملفات ويفعل إخراج الملف. سيتم تسمية ملفات السجل كالتالي: gridjs_{period}.log |
| static [SetLogDirectory](../../aspose.cells.gridjs/gridjslogger/setlogdirectory/#setlogdirectory_1)(string, GridJsLogRolling) | يضبط دليل السجل باستخدام استراتيجية تدوير للملفات ويفعل إخراج الملف. سيتم تسمية ملفات السجل كالتالي: gridjs_{period}.log |
| static [SetLogDirectory](../../aspose.cells.gridjs/gridjslogger/setlogdirectory/#setlogdirectory_2)(string, GridJsLogRolling, string) | يضبط دليل السجل باستخدام استراتيجية تدوير للملفات ويفعل إخراج الملف. سيتم تسمية ملفات السجل كالتالي: {prefix}_{period}.log أمثلة: gridjs_2026-07-27.log (يومي)، gridjs_2026-W30.log (أسبوعي)، gridjs_2026-07.log (شهري). |
| static [SetLogFile](../../aspose.cells.gridjs/gridjslogger/setlogfile/#setlogfile)(string) | يضبط مسار ملف السجل ويفعل إخراج الملف (وضع ملف واحد، بدون تدوير). يضيف إلى الملف الموجود. |
| static [SetLogFile](../../aspose.cells.gridjs/gridjslogger/setlogfile/#setlogfile_1)(string, bool) | يضبط مسار ملف السجل ويفعل إخراج الملف (وضع ملف واحد، بدون تدوير). |
| static [Warn](../../aspose.cells.gridjs/gridjslogger/warn/)(string) | يسجل رسالة بمستوى تحذير. |

### انظر أيضًا

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


