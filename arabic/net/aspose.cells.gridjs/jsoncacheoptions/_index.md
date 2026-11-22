---
title: "الفئة JsonCacheOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.GridJs.JsonCacheOptions. خيارات التكوين لتخزين JSON مؤقتًا في GridJs. يتحكم في سلوك الذاكرة L1 والقرص L2."
type: docs
url: /ar/net/aspose.cells.gridjs/jsoncacheoptions/
---
## JsonCacheOptions class

خيارات التكوين لتخزين JSON مؤقتًا في GridJs. يتحكم في سلوك الذاكرة (L1) والقرص (L2) للذاكرة المؤقتة.

```csharp
public class JsonCacheOptions
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [JsonCacheOptions](jsoncacheoptions/)() | البناء الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [CompressDisk](../../aspose.cells.gridjs/jsoncacheoptions/compressdisk/) { get; set; } | الحصول/التعيين ما إذا كان سيتم ضغط ذاكرة التخزين المؤقت على القرص باستخدام Gzip (الافتراضي: true). يؤثر عندما Enable = true ويستخدم الذاكرة المؤقتة الافتراضية. |
| [DiskPath](../../aspose.cells.gridjs/jsoncacheoptions/diskpath/) { get; set; } | الحصول/التعيين لمسار دليل ذاكرة التخزين المؤقت على القرص. يؤثر عندما Enable = true ويستخدم الذاكرة المؤقتة الافتراضية. الافتراضي: [FileCacheDirectory]/json_cache |
| [DiskTtl](../../aspose.cells.gridjs/jsoncacheoptions/diskttl/) { get; set; } | الحصول/التعيين للـ TTL لذاكرة التخزين المؤقت على القرص (الافتراضي: 24 ساعة). يؤثر عندما Enable = true ويستخدم الذاكرة المؤقتة الافتراضية. |
| [Enable](../../aspose.cells.gridjs/jsoncacheoptions/enable/) { get; set; } | الحصول/التعيين ما إذا كان سيتم تمكين تخزين JSON مؤقتًا للحصول على استجابة أسرع. عندما يتم تمكينه، سيقوم GridJs بتخزين JSON المُولد مؤقتًا وإعادة استخدامه للطلبات اللاحقة. القيمة الافتراضية هي false. ملاحظة: تحتاج إلى تعيين Implementation لاستخدام تخزين مؤقت مخصص. |
| [EnableDisk](../../aspose.cells.gridjs/jsoncacheoptions/enabledisk/) { get; set; } | الحصول/التعيين ما إذا كان سيتم تمكين ذاكرة التخزين المؤقت على القرص (الافتراضي: true). يؤثر عندما Enable = true ويستخدم الذاكرة المؤقتة الافتراضية. |
| [Implementation](../../aspose.cells.gridjs/jsoncacheoptions/implementation/) { get; set; } | الحصول/التعيين لتنفيذ تخزين JSON المؤقت المخصص. إذا لم يتم تعيينه، سيستخدم GridJs الذاكرة + ذاكرة التخزين المؤقت على القرص الافتراضية. |
| [MaxDiskSizeMB](../../aspose.cells.gridjs/jsoncacheoptions/maxdisksizemb/) { get; set; } | الحصول/التعيين للحد الأقصى لحجم ذاكرة التخزين المؤقت على القرص بالميغابايت (الافتراضي: 500 ميغابايت). يؤثر عندما Enable = true ويستخدم الذاكرة المؤقتة الافتراضية. |
| [MaxMemoryEntries](../../aspose.cells.gridjs/jsoncacheoptions/maxmemoryentries/) { get; set; } | الحصول/التعيين للحد الأقصى لعدد الإدخالات في ذاكرة التخزين المؤقت في الذاكرة (الافتراضي: 1000). يؤثر عندما Enable = true ويستخدم الذاكرة المؤقتة الافتراضية. |
| [MemoryTtl](../../aspose.cells.gridjs/jsoncacheoptions/memoryttl/) { get; set; } | الحصول/التعيين للـ TTL لذاكرة التخزين المؤقت في الذاكرة (الافتراضي: ساعة واحدة). يؤثر عندما Enable = true ويستخدم الذاكرة المؤقتة الافتراضية. |

### انظر أيضًا

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


