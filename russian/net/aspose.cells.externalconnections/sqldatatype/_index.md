---
title: "Перечисление SqlDataType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.ExternalConnections.SqlDataType. Указывает тип данных SQL параметра. Действительно только для источников ODBC"
type: docs
url: /ru/net/aspose.cells.externalconnections/sqldatatype/
---
## SqlDataType enumeration

Указывает тип данных SQL параметра. Действительно только для источников ODBC.

```csharp
public enum SqlDataType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| SqlUnsignedOffset | `-22` | sql беззнаковый offset |
| SqlSignedOffset | `-20` | sql знаковый offset |
| SqlGUID | `-11` | sql guid |
| SqlWLongVarchar | `-10` | sql wide long variable char |
| SqlWVarchar | `-9` | sql wide variable char |
| SqlWChar | `-8` | sql wide char |
| SqlBit | `-7` | sql bit |
| SqlTinyInt | `-6` | sql tiny int |
| SqlBigInt | `-5` | sql big int |
| SqlLongVarBinary | `-4` | sql long variable binary |
| SqlVarBinary | `-3` | sql variable binary |
| SqlBinary | `-2` | sql binary |
| SqlLongVarChar | `-1` | sql long variable char |
| SqlUnknownType | `0` | sql неизвестный тип |
| SqlChar | `1` | sql char |
| SqlNumeric | `2` | sql numeric |
| SqlDecimal | `3` | sql decimal |
| SqlInteger | `4` | sql integer |
| SqlSmallInt | `5` | sql small int |
| SqlFloat | `6` | sql float |
| SqlReal | `7` | sql real |
| SqlDouble | `8` | sql double |
| SqlTypeDate | `9` | sql тип даты |
| SqlTypeTime | `10` | sql тип времени |
| SqlTypeTimestamp | `11` | sql тип метки времени |
| SqlVarChar | `12` | sql переменный char |
| SqlIntervalYear | `101` | sql интервал год |
| SqlIntervalMonth | `102` | sql интервал месяц |
| SqlIntervalDay | `103` | sql интервал день |
| SqlIntervalHour | `104` | sql интервал час |
| SqlIntervalMinute | `105` | sql интервал минута |
| SqlIntervalSecond | `106` | sql интервал секунда |
| SqlIntervalYearToMonth | `107` | sql интервал год до месяца |
| SqlIntervalDayToHour | `108` | sql интервал день до часа |
| SqlIntervalDayToMinute | `109` | sql интервал день до минуты |
| SqlIntervalDayToSecond | `110` | sql интервал день до секунды |
| SqlIntervalHourToMinute | `111` | sql интервал час до минуты |
| SqlIntervalHourToSecond | `112` | sql интервал час до секунды |
| SqlIntervalMinuteToSecond | `113` | sql интервал минута до секунды |

### Примеры

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
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Продемонстрировать значения перечисления SqlDataType
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

            // Автоматически подгонять столбцы для лучшей видимости
            worksheet.AutoFitColumns();

            // Сохраните книгу
            workbook.Save("SqlDataTypeDemo.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


