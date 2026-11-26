---
title: "Clase SqlScriptSaveOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Saving.SqlScriptSaveOptions. Representa las opciones de guardado de sql"
type: docs
url: /es/net/aspose.cells.saving/sqlscriptsaveoptions/
---
## SqlScriptSaveOptions class

Representa las opciones de guardar sql.

```csharp
public class SqlScriptSaveOptions : SaveOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [SqlScriptSaveOptions](sqlscriptsaveoptions/)() | Crea opciones para guardar el archivo sql. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AddBlankLineBetweenRows](../../aspose.cells.saving/sqlscriptsaveoptions/addblanklinebetweenrows/) { get; set; } | Insertar una línea en blanco entre cada dato. |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | La carpeta para archivos temporales que pueden usarse como caché de datos. (Hereditado de [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [CheckAllDataForColumnType](../../aspose.cells.saving/sqlscriptsaveoptions/checkalldataforcolumntype/) { get; set; } | Comprobar todos los datos para encontrar el tipo de datos de las columnas. |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Si se verifica la restricción del archivo excel cuando el usuario modifica objetos relacionados con celdas. Por ejemplo, excel no permite ingresar un valor de cadena mayor a 32K. Cuando se ingresa un valor mayor a 32K, se truncará. (Hereditado de [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [CheckIfTableExists](../../aspose.cells.saving/sqlscriptsaveoptions/checkiftableexists/) { get; set; } | Comprobar si el nombre de la tabla existe antes de crearla |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Deja el libro de trabajo vacío después de guardar el archivo. (Hereditado de [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [ColumnTypeMap](../../aspose.cells.saving/sqlscriptsaveoptions/columntypemap/) { get; set; } | Obtiene y establece el mapa de tipos de columna para diferentes bases de datos. |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | Si es true y el directorio no existe, el directorio se creará automáticamente antes de guardar el archivo. (Hereditado de [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [CreateTable](../../aspose.cells.saving/sqlscriptsaveoptions/createtable/) { get; set; } | Indica si se exporta sql al crear la tabla. |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Indica si se encriptan las propiedades del documento al guardar como archivo .xls. El valor predeterminado es true. (Heredado de [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [ExportArea](../../aspose.cells.saving/sqlscriptsaveoptions/exportarea/) { get; set; } | Obtiene o establece el rango de exportación. |
| [ExportAsString](../../aspose.cells.saving/sqlscriptsaveoptions/exportasstring/) { get; set; } | Indica si se exportan todos los datos como valor de cadena. |
| [HasHeaderRow](../../aspose.cells.saving/sqlscriptsaveoptions/hasheaderrow/) { get; set; } | Indica si el rango contiene una fila de encabezado. |
| [IdName](../../aspose.cells.saving/sqlscriptsaveoptions/idname/) { get; set; } | Obtiene y establece el nombre de la columna id. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Indica si se fusionan las áreas de formato condicional y validación antes de guardar el archivo.(Inherited from [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [OperatorType](../../aspose.cells.saving/sqlscriptsaveoptions/operatortype/) { get; set; } | Obtiene y establece el tipo de operador de sql. |
| [PrimaryKey](../../aspose.cells.saving/sqlscriptsaveoptions/primarykey/) { get; set; } | Representa qué columna es la clave primaria de la tabla de datos. |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Indica si se almacena en caché los datos más recientes del gráfico.(Inherited from [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Obtiene el formato de archivo guardado.(Inherited from [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [Separator](../../aspose.cells.saving/sqlscriptsaveoptions/separator/) { get; set; } | Obtiene y establece el separador de caracteres del script sql. |
| [SheetIndexes](../../aspose.cells.saving/sqlscriptsaveoptions/sheetindexes/) { get; set; } | Representa los índices de las hojas exportadas. |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Indica si se ordenan los nombres definidos externos antes de guardar el archivo.(Inherited from [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Indica si se ordenan los nombres definidos antes de guardar el archivo.(Inherited from [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [StartId](../../aspose.cells.saving/sqlscriptsaveoptions/startid/) { get; set; } | Obtiene y establece el id inicial. |
| [TableName](../../aspose.cells.saving/sqlscriptsaveoptions/tablename/) { get; set; } | Obtiene y establece el nombre de la tabla. |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Indica si se actualiza la configuración de smart art. El valor predeterminado es false.(Inherited from [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Indica si se validan las celdas combinadas antes de guardar el archivo.(Inherited from [`SaveOptions`](../../aspose.cells/saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Obtiene o establece la devolución de llamada de advertencia.(Inherited from [`SaveOptions`](../../aspose.cells/saveoptions/).) |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Saving;
    using System;

    public class SqlScriptSaveOptionsDemo
    {
        public static void SqlScriptSaveOptionsExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Rellenar la hoja de cálculo con algunos datos
            worksheet.Cells[0, 0].PutValue("ID");
            worksheet.Cells[0, 1].PutValue("Name");
            worksheet.Cells[1, 0].PutValue(1);
            worksheet.Cells[1, 1].PutValue("John Doe");
            worksheet.Cells[2, 0].PutValue(2);
            worksheet.Cells[2, 1].PutValue("Jane Doe");

            // Crear una instancia de SqlScriptSaveOptions
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
            {
                CheckIfTableExists = true,
                ColumnTypeMap = new SqlScriptColumnTypeMap(),
                CheckAllDataForColumnType = true,
                AddBlankLineBetweenRows = false,
                Separator = ';',
                OperatorType = SqlScriptOperatorType.Insert,
                PrimaryKey = 0,
                CreateTable = true,
                IdName = "ID",
                StartId = 1,
                TableName = "MyTable",
                ExportAsString = false,
                ExportArea = new CellArea { StartRow = 0, EndRow = 2, StartColumn = 0, EndColumn = 1 },
                HasHeaderRow = true,
                ClearData = false,
                CachedFileFolder = "C:\\Temp",
                ValidateMergedAreas = true,
                MergeAreas = false,
                SortNames = false,
                SortExternalNames = false,
                RefreshChartCache = false,
                WarningCallback = null,
                UpdateSmartArt = false
            };

            // Guardar el libro de trabajo como script SQL.
            workbook.Save("MyTable.sql", saveOptions);

            return;
        }
    }
}
```

### Ver también

* class [SaveOptions](../../aspose.cells/saveoptions/)
* namespace [Aspose.Cells.Saving](../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../)


