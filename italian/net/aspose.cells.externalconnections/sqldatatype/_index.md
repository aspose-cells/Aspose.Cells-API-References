---
title: "Enum SqlDataType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.ExternalConnections.SqlDataType enum. Specifica il tipo di dato SQL del parametro. Valido solo per le origini ODBC"
type: docs
url: /it/net/aspose.cells.externalconnections/sqldatatype/
---
## SqlDataType enumeration

Specifica il tipo di dato SQL del parametro. Valido solo per le origini ODBC.

```csharp
public enum SqlDataType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| SqlUnsignedOffset | `-22` | sql offset senza segno |
| SqlSignedOffset | `-20` | sql offset con segno |
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
| SqlUnknownType | `0` | sql tipo sconosciuto |
| SqlChar | `1` | sql char |
| SqlNumeric | `2` | sql numeric |
| SqlDecimal | `3` | sql decimal |
| SqlInteger | `4` | sql integer |
| SqlSmallInt | `5` | sql small int |
| SqlFloat | `6` | sql float |
| SqlReal | `7` | sql real |
| SqlDouble | `8` | sql double |
| SqlTypeDate | `9` | sql date tipo |
| SqlTypeTime | `10` | sql time tipo |
| SqlTypeTimestamp | `11` | sql timestamp tipo |
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

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Dimostrare i valori dell'enumerazione SqlDataType
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

            // Adatta automaticamente le colonne per una migliore visibilità
            worksheet.AutoFitColumns();

            // Salva la cartella di lavoro
            workbook.Save("SqlDataTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


