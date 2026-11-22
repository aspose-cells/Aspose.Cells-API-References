---
title: "تعداد SqlDataType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.ExternalConnections.SqlDataType. يحدد نوع بيانات SQL للمعامل. صالح فقط لمصادر ODBC"
type: docs
url: /ar/net/aspose.cells.externalconnections/sqldatatype/
---
## SqlDataType enumeration

يحدد نوع بيانات SQL للمعامل. صالح فقط لمصادر ODBC.

```csharp
public enum SqlDataType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| SqlUnsignedOffset | `-22` | sql إزاحة غير موقعة |
| SqlSignedOffset | `-20` | sql إزاحة موقعة |
| SqlGUID | `-11` | sql guid |
| SqlWLongVarchar | `-10` | sql حرف متغير عريض طويل |
| SqlWVarchar | `-9` | sql حرف متغير عريض |
| SqlWChar | `-8` | sql حرف عريض |
| SqlBit | `-7` | sql بت |
| SqlTinyInt | `-6` | sql عدد صحيح صغير |
| SqlBigInt | `-5` | sql عدد صحيح كبير |
| SqlLongVarBinary | `-4` | sql ثنائي متغير طويل |
| SqlVarBinary | `-3` | sql ثنائي متغير |
| SqlBinary | `-2` | sql ثنائي |
| SqlLongVarChar | `-1` | sql حرف متغير طويل |
| SqlUnknownType | `0` | sql نوع غير معروف |
| SqlChar | `1` | sql حرف |
| SqlNumeric | `2` | sql رقمي |
| SqlDecimal | `3` | sql عشري |
| SqlInteger | `4` | sql عدد صحيح |
| SqlSmallInt | `5` | sql عدد صحيح صغير |
| SqlFloat | `6` | sql عائم |
| SqlReal | `7` | sql حقيقي |
| SqlDouble | `8` | sql مزدوج |
| SqlTypeDate | `9` | sql نوع التاريخ |
| SqlTypeTime | `10` | sql نوع الوقت |
| SqlTypeTimestamp | `11` | sql نوع الطابع الزمني |
| SqlVarChar | `12` | sql حرف متغير |
| SqlIntervalYear | `101` | sql فترة السنة |
| SqlIntervalMonth | `102` | sql فترة الشهر |
| SqlIntervalDay | `103` | sql فترة اليوم |
| SqlIntervalHour | `104` | sql فترة الساعة |
| SqlIntervalMinute | `105` | sql فترة الدقيقة |
| SqlIntervalSecond | `106` | sql فترة الثانية |
| SqlIntervalYearToMonth | `107` | sql فترة السنة إلى الشهر |
| SqlIntervalDayToHour | `108` | sql فترة اليوم إلى الساعة |
| SqlIntervalDayToMinute | `109` | sql فترة اليوم إلى الدقيقة |
| SqlIntervalDayToSecond | `110` | sql فترة اليوم إلى الثانية |
| SqlIntervalHourToMinute | `111` | sql فترة الساعة إلى الدقيقة |
| SqlIntervalHourToSecond | `112` | sql فترة الساعة إلى الثانية |
| SqlIntervalMinuteToSecond | `113` | sql فترة الدقيقة إلى الثانية |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionsClassSqlDataTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // عرض قيم تعداد SqlDataType
            worksheet.Cells["A1"].PutValue("SQL Data Type Examples");
            worksheet.Cells["A2"].PutValue("SqlChar:");
            worksheet.Cells["B2"].PutValue(SqlDataType.SqlChar.ToString());
            
            worksheet.Cells["A3"].PutValue("SqlDecimal:");
            worksheet.Cells["B3"].PutValue(SqlDataType.SqlDecimal.ToString());
            
            worksheet.Cells["A4"].PutValue("SqlInteger:");
            worksheet.Cells["B4"].PutValue(SqlDataType.SqlInteger.ToString());
            
            worksheet.Cells["A5"].PutValue("SqlTypeDate:");
            worksheet.Cells["B5"].PutValue(SqlDataType.SqlTypeDate.ToString());
            
            worksheet.Cells["A6"].PutValue("SqlVarChar:");
            worksheet.Cells["B6"].PutValue(SqlDataType.SqlVarChar.ToString());
            
            worksheet.Cells["A7"].PutValue("SqlBigInt:");
            worksheet.Cells["B7"].PutValue(SqlDataType.SqlBigInt.ToString());

            // ضبط الأعمدة تلقائيًا لتحسين الرؤية
            worksheet.AutoFitColumns();

            // احفظ المصنف
            workbook.Save("SqlDataTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


