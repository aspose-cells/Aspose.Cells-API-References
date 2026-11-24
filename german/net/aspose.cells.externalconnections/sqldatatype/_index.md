---
title: "Enum SqlDataType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.ExternalConnections.SqlDataType Enum. Gibt den SQL-Datentyp des Parameters an. Nur für ODBC-Quellen gültig"
type: docs
url: /de/net/aspose.cells.externalconnections/sqldatatype/
---
## SqlDataType enumeration

Gibt den SQL-Datentyp des Parameters an. Nur für ODBC-Quellen gültig.

```csharp
public enum SqlDataType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| SqlUnsignedOffset | `-22` | SQL vorzeichenloser Offset |
| SqlSignedOffset | `-20` | SQL signierter Offset |
| SqlGUID | `-11` | SQL GUID |
| SqlWLongVarchar | `-10` | SQL breite lange variable CHAR |
| SqlWVarchar | `-9` | SQL breite variable CHAR |
| SqlWChar | `-8` | SQL breiter CHAR |
| SqlBit | `-7` | SQL Bit |
| SqlTinyInt | `-6` | SQL kleine Ganzzahl |
| SqlBigInt | `-5` | SQL große Ganzzahl |
| SqlLongVarBinary | `-4` | SQL lange variable Binär |
| SqlVarBinary | `-3` | SQL variable Binär |
| SqlBinary | `-2` | SQL Binär |
| SqlLongVarChar | `-1` | SQL lange variable CHAR |
| SqlUnknownType | `0` | SQL unbekannter Typ |
| SqlChar | `1` | SQL CHAR |
| SqlNumeric | `2` | SQL NUMERIC |
| SqlDecimal | `3` | SQL DECIMAL |
| SqlInteger | `4` | SQL INTEGER |
| SqlSmallInt | `5` | SQL kleine Ganzzahl |
| SqlFloat | `6` | SQL FLOAT |
| SqlReal | `7` | SQL REAL |
| SqlDouble | `8` | SQL DOUBLE |
| SqlTypeDate | `9` | SQL Datumstyp |
| SqlTypeTime | `10` | SQL Zeittyp |
| SqlTypeTimestamp | `11` | SQL Zeitstempeltyp |
| SqlVarChar | `12` | SQL variable CHAR |
| SqlIntervalYear | `101` | SQL-Intervall Jahr |
| SqlIntervalMonth | `102` | SQL-Intervall Monat |
| SqlIntervalDay | `103` | SQL-Intervall Tag |
| SqlIntervalHour | `104` | SQL-Intervall Stunde |
| SqlIntervalMinute | `105` | SQL-Intervall Minute |
| SqlIntervalSecond | `106` | SQL-Intervall Sekunde |
| SqlIntervalYearToMonth | `107` | SQL-Intervall Jahr bis Monat |
| SqlIntervalDayToHour | `108` | SQL-Intervall Tag bis Stunde |
| SqlIntervalDayToMinute | `109` | SQL-Intervall Tag bis Minute |
| SqlIntervalDayToSecond | `110` | SQL-Intervall Tag bis Sekunde |
| SqlIntervalHourToMinute | `111` | SQL-Intervall Stunde bis Minute |
| SqlIntervalHourToSecond | `112` | SQL-Intervall Stunde bis Sekunde |
| SqlIntervalMinuteToSecond | `113` | SQL-Intervall Minute bis Sekunde |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Demonstriere SqlDataType-Enum-Werte
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

            // Spalten automatisch anpassen für bessere Sichtbarkeit
            worksheet.AutoFitColumns();

            // Speichere die Arbeitsmappe
            workbook.Save("SqlDataTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


