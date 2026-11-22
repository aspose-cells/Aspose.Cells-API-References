---
title: "GridJsLogger.SetLogDirectory"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة GridJsLogger. تعيين دليل السجل باستخدام استراتيجية تدوير الملفات اليومية وتمكين إخراج الملفات. سيتم تسمية ملفات السجل كـ gridjs_period.log"
type: docs
url: /ar/net/aspose.cells.gridjs/gridjslogger/setlogdirectory/
---
## SetLogDirectory(string) {#setlogdirectory}

يضبط دليل السجل باستخدام استراتيجية تدوير يومية للملفات ويفعل إخراج الملف. سيتم تسمية ملفات السجل كالتالي: gridjs_{period}.log

```csharp
public static void SetLogDirectory(string directory)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| الدليل | String | الدليل لتخزين ملفات السجل. |

### انظر أيضًا

* class [GridJsLogger](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)

---

## SetLogDirectory(string, GridJsLogRolling) {#setlogdirectory_1}

يضبط دليل السجل باستخدام استراتيجية تدوير للملفات ويفعل إخراج الملف. سيتم تسمية ملفات السجل كالتالي: gridjs_{period}.log

```csharp
public static void SetLogDirectory(string directory, GridJsLogRolling rolling)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| الدليل | String | الدليل لتخزين ملفات السجل. |
| التدوير | GridJsLogRolling | استراتيجية التدوير (يومي/أسبوعي/شهري). |

### انظر أيضًا

* enum [GridJsLogRolling](../../gridjslogrolling/)
* class [GridJsLogger](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)

---

## SetLogDirectory(string, GridJsLogRolling, string) {#setlogdirectory_2}

يضبط دليل السجل باستخدام استراتيجية تدوير للملفات ويفعل إخراج الملف. سيتم تسمية ملفات السجل كالتالي: {prefix}_{period}.log أمثلة: gridjs_2026-07-27.log (يومي)، gridjs_2026-W30.log (أسبوعي)، gridjs_2026-07.log (شهري).

```csharp
public static void SetLogDirectory(string directory, GridJsLogRolling rolling, string filePrefix)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| الدليل | String | الدليل لتخزين ملفات السجل. |
| التدوير | GridJsLogRolling | استراتيجية التدوير (يومي/أسبوعي/شهري). |
| filePrefix | String | بادئة اسم الملف. |

### انظر أيضًا

* enum [GridJsLogRolling](../../gridjslogrolling/)
* class [GridJsLogger](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)


