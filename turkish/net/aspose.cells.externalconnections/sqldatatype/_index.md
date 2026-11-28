---
title: "Enum SqlDataType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.ExternalConnections.SqlDataType enum. Parametrenin SQL veri tipini belirtir. Yalnızca ODBC kaynakları için geçerlidir"
type: docs
url: /tr/net/aspose.cells.externalconnections/sqldatatype/
---
## SqlDataType enumeration

Parametrenin SQL veri tipini belirtir. Yalnızca ODBC kaynakları için geçerlidir.

```csharp
public enum SqlDataType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| SqlUnsignedOffset | `-22` | sql işaretsiz offset |
| SqlSignedOffset | `-20` | sql işaretli offset |
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
| SqlUnknownType | `0` | sql bilinmeyen tip |
| SqlChar | `1` | sql char |
| SqlNumeric | `2` | sql numeric |
| SqlDecimal | `3` | sql decimal |
| SqlInteger | `4` | sql integer |
| SqlSmallInt | `5` | sql small int |
| SqlFloat | `6` | sql float |
| SqlReal | `7` | sql real |
| SqlDouble | `8` | sql double |
| SqlTypeDate | `9` | sql date türü |
| SqlTypeTime | `10` | sql time türü |
| SqlTypeTimestamp | `11` | sql timestamp türü |
| SqlVarChar | `12` | sql variable char |
| SqlIntervalYear | `101` | sql interval yıl |
| SqlIntervalMonth | `102` | sql interval ay |
| SqlIntervalDay | `103` | sql interval gün |
| SqlIntervalHour | `104` | sql interval saat |
| SqlIntervalMinute | `105` | sql interval dakika |
| SqlIntervalSecond | `106` | sql interval saniye |
| SqlIntervalYearToMonth | `107` | sql interval yıl'dan aya |
| SqlIntervalDayToHour | `108` | sql interval gün'den saate |
| SqlIntervalDayToMinute | `109` | sql interval gün'den dakikaya |
| SqlIntervalDayToSecond | `110` | sql interval gün'den saniyeye |
| SqlIntervalHourToMinute | `111` | sql interval saat'tan dakikaya |
| SqlIntervalHourToSecond | `112` | sql interval saat'tan saniyeye |
| SqlIntervalMinuteToSecond | `113` | sql interval dakikadan saniyeye |

### Örnekler

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
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // SqlDataType enum değerlerini göster
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

            // Daha iyi görünürlük için sütunları otomatik sığdır
            worksheet.AutoFitColumns();

            // Çalışma kitabını kaydedin
            workbook.Save("SqlDataTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


