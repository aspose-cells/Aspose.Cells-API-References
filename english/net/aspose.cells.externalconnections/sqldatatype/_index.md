---
title: Enum SqlDataType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.ExternalConnections.SqlDataType enum. Specifies SQL data type of the parameter. Only valid for ODBC sources
type: docs
url: /net/aspose.cells.externalconnections/sqldatatype/
---
## SqlDataType enumeration

Specifies SQL data type of the parameter. Only valid for ODBC sources.

```csharp
public enum SqlDataType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| SqlUnsignedOffset | `-22` | sql unsigned offset |
| SqlSignedOffset | `-20` | sql signed offset |
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
| SqlUnknownType | `0` | sql unknown type |
| SqlChar | `1` | sql char |
| SqlNumeric | `2` | sql numeric |
| SqlDecimal | `3` | sql decimal |
| SqlInteger | `4` | sql integer |
| SqlSmallInt | `5` | sql small int |
| SqlFloat | `6` | sql float |
| SqlReal | `7` | sql real |
| SqlDouble | `8` | sql double |
| SqlTypeDate | `9` | sql date type |
| SqlTypeTime | `10` | sql time type |
| SqlTypeTimestamp | `11` | sql timestamp type |
| SqlVarChar | `12` | sql variable char |
| SqlIntervalYear | `101` | sql interval year |
| SqlIntervalMonth | `102` | sql interval month |
| SqlIntervalDay | `103` | sql interval day |
| SqlIntervalHour | `104` | sql interval hour |
| SqlIntervalMinute | `105` | sql interval minute |
| SqlIntervalSecond | `106` | sql interval second |
| SqlIntervalYearToMonth | `107` | sql interval year to month |
| SqlIntervalDayToHour | `108` | sql interval day to hour |
| SqlIntervalDayToMinute | `109` | sql interval day to minute |
| SqlIntervalDayToSecond | `110` | sql interval day to second |
| SqlIntervalHourToMinute | `111` | sql interval hour to minute |
| SqlIntervalHourToSecond | `112` | sql interval hour to second |
| SqlIntervalMinuteToSecond | `113` | sql interval minute to second |

### Examples

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
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Demonstrate SqlDataType enum values
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

            // Auto-fit columns for better visibility
            worksheet.AutoFitColumns();

            // Save the workbook
            workbook.Save("SqlDataTypeDemo.xlsx");
        }
    }
}
```

### See Also

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


