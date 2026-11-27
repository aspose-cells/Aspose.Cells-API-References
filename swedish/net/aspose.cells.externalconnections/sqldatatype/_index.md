---
title: "Enum SqlDataType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.ExternalConnections.SqlDataType enum. Anger SQL-datatyp för parametern. Giltig endast för ODBC-källor"
type: docs
url: /sv/net/aspose.cells.externalconnections/sqldatatype/
---
## SqlDataType enumeration

Anger SQL-datatyp för parametern. Gäller endast för ODBC-källor.

```csharp
public enum SqlDataType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| SqlUnsignedOffset | `-22` | sql osignerad offset |
| SqlSignedOffset | `-20` | sql signerad offset |
| SqlGUID | `-11` | sql guid |
| SqlWLongVarchar | `-10` | sql bred lång variabel char |
| SqlWVarchar | `-9` | sql bred variabel char |
| SqlWChar | `-8` | sql bred char |
| SqlBit | `-7` | sql bit |
| SqlTinyInt | `-6` | sql liten int |
| SqlBigInt | `-5` | sql stor int |
| SqlLongVarBinary | `-4` | sql lång variabel binary |
| SqlVarBinary | `-3` | sql variabel binary |
| SqlBinary | `-2` | sql binary |
| SqlLongVarChar | `-1` | sql lång variabel char |
| SqlUnknownType | `0` | sql okänd typ |
| SqlChar | `1` | sql char |
| SqlNumeric | `2` | sql numerisk |
| SqlDecimal | `3` | sql decimal |
| SqlInteger | `4` | sql heltal |
| SqlSmallInt | `5` | sql små int |
| SqlFloat | `6` | sql flyttal |
| SqlReal | `7` | sql reell |
| SqlDouble | `8` | sql dubbel |
| SqlTypeDate | `9` | sql datumtyp |
| SqlTypeTime | `10` | sql tidstyp |
| SqlTypeTimestamp | `11` | sql tidsstämpeltyp |
| SqlVarChar | `12` | sql variabel char |
| SqlIntervalYear | `101` | sql intervall år |
| SqlIntervalMonth | `102` | sql intervall månad |
| SqlIntervalDay | `103` | sql intervall dag |
| SqlIntervalHour | `104` | sql intervall timme |
| SqlIntervalMinute | `105` | sql intervall minut |
| SqlIntervalSecond | `106` | sql intervall sekund |
| SqlIntervalYearToMonth | `107` | sql intervall år till månad |
| SqlIntervalDayToHour | `108` | sql intervall dag till timme |
| SqlIntervalDayToMinute | `109` | sql intervall dag till minut |
| SqlIntervalDayToSecond | `110` | sql intervall dag till sekund |
| SqlIntervalHourToMinute | `111` | sql intervall timme till minut |
| SqlIntervalHourToSecond | `112` | sql intervall timme till sekund |
| SqlIntervalMinuteToSecond | `113` | sql intervall minut till sekund |

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Demonstrera SqlDataType enumvärden
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

            // Autoanpassa kolumner för bättre synlighet
            worksheet.AutoFitColumns();

            // Spara arbetsboken
            workbook.Save("SqlDataTypeDemo.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


