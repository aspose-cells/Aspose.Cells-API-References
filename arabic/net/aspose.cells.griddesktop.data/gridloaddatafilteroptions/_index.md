---
title: "Enum GridLoadDataFilterOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.GridDesktop.Data.GridLoadDataFilterOptions enum. يمثل الخيارات لتصفية البيانات عند تحميل دفتر العمل من القالب"
type: docs
url: /ar/net/aspose.cells.griddesktop.data/gridloaddatafilteroptions/
---
## GridLoadDataFilterOptions enumeration

يمثل الخيارات لتصفية البيانات عند تحميل دفتر العمل من القالب.

```csharp
public enum GridLoadDataFilterOptions
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| All | `2147483647` | تحميل الكل |
| CellBlank | `1` | تحميل الخلايا التي قيمتها فارغة |
| CellString | `2` | تحميل الخلايا التي قيمتها نص |
| CellNumeric | `4` | تحميل الخلايا التي قيمتها رقمية (بما في ذلك التاريخ والوقت) |
| CellError | `8` | تحميل الخلايا التي قيمتها خطأ |
| CellBool | `16` | تحميل الخلايا التي قيمتها منطقية |
| CellValue | `31` | تحميل قيم الخلايا (جميع أنواع القيم) فقط |
| Formula | `32` | تحميل صيغ الخلية. |
| CellData | `67108927` | تحميل بيانات الخلايا بما في ذلك القيم، الصيغ والتنسيق |
| Chart | `256` | تحميل المخططات |
| Drawing | `402653952` | كائنات الرسم (بما في ذلك المخطط، الصورة، OleObject وجميع كائنات الرسم الأخرى) |
| MergedArea | `1024` | تحميل الخلايا المدمجة |
| ConditionalFormatting | `2048` | تحميل التنسيق الشرطي |
| DataValidation | `4096` | تحميل التحقق من صحة البيانات |
| PivotTable | `8192` | تحميل جداول المحورية |
| Table | `16384` | تحميل الجداول |
| Hyperlinks | `32768` | تحميل الروابط التشعبية |
| SheetSettings | `65536` | تحميل إعدادات ورقة العمل |
| SheetData | `403701759` | تحميل جميع بيانات ورقة العمل، مثل بيانات الخلايا، الإعدادات، الكائنات، ...إلخ. |
| BookSettings | `1048576` | تحميل إعدادات المصنف |
| Settings | `1114112` | تحميل إعدادات المصنف وورقة العمل |
| XmlMap | `2097152` | تحميل XmlMap |
| Structure | `4194304` | تحميل بنية المصنف |
| DocumentProperties | `8388608` | تحميل خصائص المستند |
| DefinedNames | `16777216` | تحميل كائنات الاسم المعرفة |
| VBA | `33554432` | تحميل مشاريع VBA |
| Style | `67108864` | تحميل الأنماط لتنسيق الخلية |
| Picture | `134217728` | تحميل الصور |
| OleObject | `268435456` | تحميل OleObjects |
| Revision | `536870912` | تحميل سجلات المراجعة |

### انظر أيضًا

* namespace [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../)


