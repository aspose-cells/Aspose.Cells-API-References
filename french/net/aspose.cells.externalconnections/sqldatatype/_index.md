---
title: "Enum SqlDataType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Enum Aspose.Cells.ExternalConnections.SqlDataType. Spécifie le type de données SQL du paramètre. Valide uniquement pour les sources ODBC"
type: docs
url: /fr/net/aspose.cells.externalconnections/sqldatatype/
---
## SqlDataType enumeration

Spécifie le type de données SQL du paramètre. Valide uniquement pour les sources ODBC.

```csharp
public enum SqlDataType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| SqlUnsignedOffset | `-22` | sql offset non signé |
| SqlSignedOffset | `-20` | sql offset signé |
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
| SqlUnknownType | `0` | sql type inconnu |
| SqlChar | `1` | sql char |
| SqlNumeric | `2` | sql numeric |
| SqlDecimal | `3` | sql decimal |
| SqlInteger | `4` | sql integer |
| SqlSmallInt | `5` | sql small int |
| SqlFloat | `6` | sql float |
| SqlReal | `7` | sql real |
| SqlDouble | `8` | sql double |
| SqlTypeDate | `9` | sql type de date |
| SqlTypeTime | `10` | sql type de temps |
| SqlTypeTimestamp | `11` | sql type d'horodatage |
| SqlVarChar | `12` | sql char variable |
| SqlIntervalYear | `101` | sql interval année |
| SqlIntervalMonth | `102` | sql interval mois |
| SqlIntervalDay | `103` | sql interval jour |
| SqlIntervalHour | `104` | sql interval heure |
| SqlIntervalMinute | `105` | sql interval minute |
| SqlIntervalSecond | `106` | sql interval seconde |
| SqlIntervalYearToMonth | `107` | sql interval année à mois |
| SqlIntervalDayToHour | `108` | sql interval jour à heure |
| SqlIntervalDayToMinute | `109` | sql interval jour à minute |
| SqlIntervalDayToSecond | `110` | sql interval jour à seconde |
| SqlIntervalHourToMinute | `111` | sql interval heure à minute |
| SqlIntervalHourToSecond | `112` | sql interval heure à seconde |
| SqlIntervalMinuteToSecond | `113` | sql interval minute à seconde |

### Exemples

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
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Démontrer les valeurs de l'énumération SqlDataType
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

            // Ajuster automatiquement les colonnes pour une meilleure visibilité
            worksheet.AutoFitColumns();

            // Enregistrez le classeur
            workbook.Save("SqlDataTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


