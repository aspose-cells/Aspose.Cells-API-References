---
title: "SqlScriptSaveOptions Class"
linktitle: "SqlScriptSaveOptions"
articleTitle: "SqlScriptSaveOptions"
second_title: "Aspose.Cells for Python via Java"
description: "Represents the options of saving sql."
type: docs
weight: 6400
url: /python-java/asposecells.api/sqlscriptsaveoptions/
---

## SqlScriptSaveOptions class

Represents the options of saving sql.

## Constructors

| Name | Description |
| --- | --- |
| [SqlScriptSaveOptions](#constructor) | Creates options for saving sql file. |

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [CheckIfTableExists](#checkiftableexists) | boolean | Check if the table name exists before creating |
| [ColumnTypeMap](#columntypemap) | SqlScriptColumnTypeMap | Gets and sets the map of column type for different database. |
| [CheckAllDataForColumnType](#checkalldataforcolumntype) | boolean | Check all data to find columns' data type. The default value is false, we only check the first row for performance. If t |
| [AddBlankLineBetweenRows](#addblanklinebetweenrows) | boolean | Insert blank line between each data. If Separator is '\n' , it's better to set this property as true to increase readabi |
| [Separator](#separator) | char | Gets and sets character separator of sql script. Only can be ' ' or '\n'. If the |
| [OperatorType](#operatortype) | int | Gets and sets the operator type of sql. The value of the property is SqlScriptOperatorType integer constant. |
| [PrimaryKey](#primarykey) | int | Represents which column is primary key of the data table. |
| [CreateTable](#createtable) | boolean | Indicates whether exporting sql of creating table. |
| [IdName](#idname) | String | Gets and sets the name of id column. If this property is set , a column will be inserted with automatical increment int  |
| [StartId](#startid) | int | Gets and sets the start id. Only works when IdName is set. |
| [TableName](#tablename) | String | Gets and sets the table name. |
| [ExportAsString](#exportasstring) | boolean | Indicates whether exporting all data as string value. |
| [SheetIndexes](#sheetindexes) | int[] | Represents the indexes of exported sheets. |
| [ExportArea](#exportarea) | CellArea | Gets or sets the exporting range. |
| [HasHeaderRow](#hasheaderrow) | boolean | Indicates whether the range contains header row. |
| [SaveFormat](#saveformat) | int | Gets the save file format. The value of the property is SaveFormat integer constant. |
| [ClearData](#cleardata) | boolean | Make the workbook empty after saving the file. |
| [CachedFileFolder](#cachedfilefolder) | String | The cached file folder is used to store some large data. |
| [ValidateMergedAreas](#validatemergedareas) | boolean | Indicates whether validate merged cells before saving the file. The default value is false. |
| [MergeAreas](#mergeareas) | boolean | Indicates whether merge the areas of conditional formatting and validation before saving the file. The default value is  |
| [CreateDirectory](#createdirectory) | boolean | If true and the directory does not exist, the directory will be automatically created before saving the file. The defaul |
| [SortNames](#sortnames) | boolean | Indicates whether sorting defined names before saving file. |
| [SortExternalNames](#sortexternalnames) | boolean | Indicates whether sorting external defined names before saving file. |
| [RefreshChartCache](#refreshchartcache) | boolean | Indicates whether refreshing chart cache data |
| [WarningCallback](#warningcallback) | IWarningCallback | Gets or sets warning callback. |
| [CheckExcelRestriction](#checkexcelrestriction) | boolean |  |
| [UpdateSmartArt](#updatesmartart) | boolean | Indicates whether updating smart art setting. The default value is false. Only effects after calling Shape.GetResultOfSm |
| [EncryptDocumentProperties](#encryptdocumentproperties) | boolean |  |

### SqlScriptSaveOptions() {#constructor}

Creates options for saving sql file.

### SqlScriptSaveOptions.CheckIfTableExists property {#checkiftableexists}

Check if the table name exists before creating

**Type:** boolean

### SqlScriptSaveOptions.ColumnTypeMap property {#columntypemap}

Gets and sets the map of column type for different database.

**Type:** SqlScriptColumnTypeMap

### SqlScriptSaveOptions.CheckAllDataForColumnType property {#checkalldataforcolumntype}

Check all data to find columns' data type. The default value is false, we only check the first row for performance. If this property is true and the columns contains mixed value type, the columns' type will be text.

**Type:** boolean

### SqlScriptSaveOptions.AddBlankLineBetweenRows property {#addblanklinebetweenrows}

Insert blank line between each data. If Separator is '\n' , it's better to set this property as true to increase readability.

**Type:** boolean

### SqlScriptSaveOptions.Separator property {#separator}

Gets and sets character separator of sql script. Only can be ' ' or '\n'. If the

**Type:** char

### SqlScriptSaveOptions.OperatorType property {#operatortype}

Gets and sets the operator type of sql. The value of the property is SqlScriptOperatorType integer constant.

**Type:** int

### SqlScriptSaveOptions.PrimaryKey property {#primarykey}

Represents which column is primary key of the data table.

**Type:** int

### SqlScriptSaveOptions.CreateTable property {#createtable}

Indicates whether exporting sql of creating table.

**Type:** boolean

### SqlScriptSaveOptions.IdName property {#idname}

Gets and sets the name of id column. If this property is set , a column will be inserted with automatical increment int value.

**Type:** String

### SqlScriptSaveOptions.StartId property {#startid}

Gets and sets the start id. Only works when IdName is set.

**Type:** int

### SqlScriptSaveOptions.TableName property {#tablename}

Gets and sets the table name.

**Type:** String

### SqlScriptSaveOptions.ExportAsString property {#exportasstring}

Indicates whether exporting all data as string value.

**Type:** boolean

### SqlScriptSaveOptions.SheetIndexes property {#sheetindexes}

Represents the indexes of exported sheets.

**Type:** int[]

### SqlScriptSaveOptions.ExportArea property {#exportarea}

Gets or sets the exporting range.

**Type:** CellArea

### SqlScriptSaveOptions.HasHeaderRow property {#hasheaderrow}

Indicates whether the range contains header row.

**Type:** boolean

### SqlScriptSaveOptions.SaveFormat property {#saveformat}

Gets the save file format. The value of the property is SaveFormat integer constant.

**Type:** int

### SqlScriptSaveOptions.ClearData property {#cleardata}

Make the workbook empty after saving the file.

**Type:** boolean

### SqlScriptSaveOptions.CachedFileFolder property {#cachedfilefolder}

The cached file folder is used to store some large data.

**Type:** String

### SqlScriptSaveOptions.ValidateMergedAreas property {#validatemergedareas}

Indicates whether validate merged cells before saving the file. The default value is false.

**Type:** boolean

### SqlScriptSaveOptions.MergeAreas property {#mergeareas}

Indicates whether merge the areas of conditional formatting and validation before saving the file. The default value is false.

**Type:** boolean

### SqlScriptSaveOptions.CreateDirectory property {#createdirectory}

If true and the directory does not exist, the directory will be automatically created before saving the file. The default value is false.

**Type:** boolean

### SqlScriptSaveOptions.SortNames property {#sortnames}

Indicates whether sorting defined names before saving file.

**Type:** boolean

### SqlScriptSaveOptions.SortExternalNames property {#sortexternalnames}

Indicates whether sorting external defined names before saving file.

**Type:** boolean

### SqlScriptSaveOptions.RefreshChartCache property {#refreshchartcache}

Indicates whether refreshing chart cache data

**Type:** boolean

### SqlScriptSaveOptions.WarningCallback property {#warningcallback}

Gets or sets warning callback.

**Type:** IWarningCallback

### SqlScriptSaveOptions.CheckExcelRestriction property {#checkexcelrestriction}

**Type:** boolean

### SqlScriptSaveOptions.UpdateSmartArt property {#updatesmartart}

Indicates whether updating smart art setting. The default value is false. Only effects after calling Shape.GetResultOfSmartArt() method and the cached shapes exist in the template file.

**Type:** boolean

### SqlScriptSaveOptions.EncryptDocumentProperties property {#encryptdocumentproperties}

**Type:** boolean
