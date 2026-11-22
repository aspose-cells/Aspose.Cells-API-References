---
title: "التعداد CountryCode"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "التعداد Aspose.Cells.CountryCode. يمثل معرفات دول Excel"
type: docs
url: /ar/net/aspose.cells/countrycode/
---
## CountryCode enumeration

يمثل معرفات دول Excel.

```csharp
public enum CountryCode
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Default | `0` |  |
| USA | `1` | الولايات المتحدة |
| Canada | `2` | كندا |
| LatinAmeric | `3` | أمريكا اللاتينية، باستثناء البرازيل |
| Russia | `7` | روسيا |
| Egypt | `20` | مصر |
| Greece | `30` | اليونان |
| Netherlands | `31` | هولندا |
| Belgium | `32` | بلجيكا |
| France | `33` | فرنسا |
| Spain | `34` | إسبانيا |
| Hungary | `36` | المجر |
| Italy | `39` | إيطاليا |
| Switzerland | `41` | سويسرا |
| Austria | `43` | النمسا |
| UnitedKingdom | `44` | المملكة المتحدة |
| Denmark | `45` | الدنمارك |
| Sweden | `46` | السويد |
| Norway | `47` | النرويج |
| Poland | `48` | بولندا |
| Germany | `49` | ألمانيا |
| Mexico | `52` | المكسيك |
| Brazil | `55` | البرازيل |
| Australia | `61` | أستراليا |
| NewZealand | `64` | نيوزيلندا |
| Thailand | `66` | تايلاند |
| Japan | `81` | اليابان |
| SouthKorea | `82` | كوريا الجنوبية |
| VietNam | `84` | فيتنام |
| China | `86` | جمهورية الصين الشعبية |
| Turkey | `90` | تركيا |
| India | `91` | الهند |
| Algeria | `213` | الجزائر |
| Morocco | `216` | المغرب |
| Libya | `218` | ليبيا |
| Portugal | `351` | البرتغال |
| Iceland | `354` | آيسلندا |
| Finland | `358` | فنلندا |
| Czech | `420` | جمهورية التشيك |
| Taiwan | `886` | تايوان |
| Lebanon | `961` | لبنان |
| Jordan | `962` | الأردن |
| Syria | `963` | سوريا |
| Iraq | `964` | العراق |
| Kuwait | `965` | الكويت |
| Saudi | `966` | المملكة العربية السعودية |
| UnitedArabEmirates | `971` | الإمارات العربية المتحدة |
| Israel | `972` | إسرائيل |
| Qatar | `974` | قطر |
| Iran | `981` | إيران |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CountryCodeDemo
    {
        public static void CountryCodeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // تعيين رمز الدولة لدفتر العمل
            workbook.Settings.LanguageCode = CountryCode.USA;
            workbook.Settings.Region = CountryCode.USA;

            // إضافة بعض البيانات إلى ورقة العمل
            worksheet.Cells[0, 0].PutValue("Country");
            worksheet.Cells[0, 1].PutValue("Code");

            worksheet.Cells[1, 0].PutValue("United States");
            worksheet.Cells[1, 1].PutValue((int)CountryCode.USA);

            worksheet.Cells[2, 0].PutValue("Canada");
            worksheet.Cells[2, 1].PutValue((int)CountryCode.Canada);

            worksheet.Cells[3, 0].PutValue("France");
            worksheet.Cells[3, 1].PutValue((int)CountryCode.France);

            worksheet.Cells[4, 0].PutValue("Germany");
            worksheet.Cells[4, 1].PutValue((int)CountryCode.Germany);

            // احفظ المصنف
            workbook.Save("CountryCodeExample.xlsx");
            workbook.Save("CountryCodeExample.pdf");
            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


