---
title: "Enumeración SqlDataType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.ExternalConnections.SqlDataType enum. Especifica el tipo de datos SQL del parámetro. Sólo válido para fuentes ODBC"
type: docs
url: /es/net/aspose.cells.externalconnections/sqldatatype/
---
## SqlDataType enumeration

Especifica el tipo de datos SQL del parámetro. Solo válido para fuentes ODBC.

```csharp
public enum SqlDataType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| SqlUnsignedOffset | `-22` | sql desplazamiento sin signo |
| SqlSignedOffset | `-20` | sql desplazamiento con signo |
| SqlGUID | `-11` | sql guid |
| SqlWLongVarchar | `-10` | sql carácter variable ancho largo |
| SqlWVarchar | `-9` | sql carácter variable ancho |
| SqlWChar | `-8` | sql carácter ancho |
| SqlBit | `-7` | sql bit |
| SqlTinyInt | `-6` | sql tiny int |
| SqlBigInt | `-5` | sql big int |
| SqlLongVarBinary | `-4` | sql binario variable largo |
| SqlVarBinary | `-3` | sql binario variable |
| SqlBinary | `-2` | sql binary |
| SqlLongVarChar | `-1` | sql carácter variable largo |
| SqlUnknownType | `0` | sql tipo desconocido |
| SqlChar | `1` | sql char |
| SqlNumeric | `2` | sql numeric |
| SqlDecimal | `3` | sql decimal |
| SqlInteger | `4` | sql integer |
| SqlSmallInt | `5` | sql small int |
| SqlFloat | `6` | sql float |
| SqlReal | `7` | sql real |
| SqlDouble | `8` | sql doble |
| SqlTypeDate | `9` | tipo de fecha sql |
| SqlTypeTime | `10` | tipo de hora sql |
| SqlTypeTimestamp | `11` | tipo de marca de tiempo sql |
| SqlVarChar | `12` | sql char variable |
| SqlIntervalYear | `101` | intervalo de año sql |
| SqlIntervalMonth | `102` | intervalo de mes sql |
| SqlIntervalDay | `103` | intervalo de día sql |
| SqlIntervalHour | `104` | intervalo de hora sql |
| SqlIntervalMinute | `105` | intervalo de minuto sql |
| SqlIntervalSecond | `106` | intervalo de segundo sql |
| SqlIntervalYearToMonth | `107` | intervalo de año a mes sql |
| SqlIntervalDayToHour | `108` | intervalo de día a hora sql |
| SqlIntervalDayToMinute | `109` | intervalo de día a minuto sql |
| SqlIntervalDayToSecond | `110` | intervalo de día a segundo sql |
| SqlIntervalHourToMinute | `111` | intervalo de hora a minuto sql |
| SqlIntervalHourToSecond | `112` | intervalo de hora a segundo sql |
| SqlIntervalMinuteToSecond | `113` | intervalo de minuto a segundo sql |

### Ejemplos

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
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Demostrar valores del enum SqlDataType
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

            // Ajustar automáticamente las columnas para una mejor visibilidad
            worksheet.AutoFitColumns();

            // Guarda el libro de trabajo
            workbook.Save("SqlDataTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


