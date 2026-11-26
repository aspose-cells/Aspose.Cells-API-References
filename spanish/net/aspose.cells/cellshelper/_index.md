---
title: "Clase CellsHelper"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.CellsHelper. Proporciona funciones auxiliares"
type: docs
url: /es/net/aspose.cells/cellshelper/
---
## CellsHelper class

Proporciona funciones auxiliares.

```csharp
public class CellsHelper
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| static [AltStartPath](../../aspose.cells/cellshelper/altstartpath/) { get; set; } | Obtiene o establece la ruta de inicio alternativa, a la que se hace referencia en algunas referencias de fórmulas externas. |
| static [CustomImplementationFactory](../../aspose.cells/cellshelper/customimplementationfactory/) { get; set; } | Obtiene o establece la fábrica para crear instancias con implementación especial. |
| static [DPI](../../aspose.cells/cellshelper/dpi/) { get; set; } | Obtiene los DPI de la máquina. |
| static [IsCloudPlatform](../../aspose.cells/cellshelper/iscloudplatform/) { get; set; } | Por favor, establezca esta propiedad en True al ejecutar en una plataforma en la nube, como: Azure, AWSLambda, etc, |
| static [LibraryPath](../../aspose.cells/cellshelper/librarypath/) { get; set; } | Obtiene o establece la ruta de la biblioteca a la que se hace referencia en algunas referencias de fórmulas externas. |
| static [SignificantDigits](../../aspose.cells/cellshelper/significantdigits/) { get; set; } | (**Obsolete.**) Obtiene y establece el número de dígitos significativos. El valor predeterminado es 17. |
| static [SignificantDigitsType](../../aspose.cells/cellshelper/significantdigitstype/) { get; set; } | Obtiene y establece el tipo predeterminado de dígitos significativos para la salida de valores numéricos. El valor predeterminado es G17. |
| static [StartupPath](../../aspose.cells/cellshelper/startuppath/) { get; set; } | Obtiene o establece la ruta de inicio a la que se hace referencia en algunas referencias de fórmulas externas. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| static [AddAddInFunction](../../aspose.cells/cellshelper/addaddinfunction/)(string, int, int, ParameterType[], ParameterType) | (**Obsolete.**) Añadir función de complemento. |
| static [CellIndexToName](../../aspose.cells/cellshelper/cellindextoname/)(int, int) | Obtiene el nombre de la celda según sus índices de fila y columna. |
| static [CellNameToIndex](../../aspose.cells/cellshelper/cellnametoindex/)(string, out int, out int) | Obtiene los índices de fila y columna de la celda según su nombre. |
| static [ColumnIndexToName](../../aspose.cells/cellshelper/columnindextoname/)(int) | Obtiene el nombre de la columna según el índice de columna. |
| static [ColumnNameToIndex](../../aspose.cells/cellshelper/columnnametoindex/)(string) | Obtiene el índice de columna según el nombre de columna. |
| static [ConvertA1FormulaToR1C1](../../aspose.cells/cellshelper/converta1formulator1c1/)(string, int, int) | (**Obsoleto.**) Convierte la fórmula A1 de la celda a la fórmula r1c1. |
| static [ConvertR1C1FormulaToA1](../../aspose.cells/cellshelper/convertr1c1formulatoa1/)(string, int, int) | (**Obsoleto.**) Convierte la fórmula r1c1 de la celda a la fórmula A1. |
| static [CreateSafeSheetName](../../aspose.cells/cellshelper/createsafesheetname/#createsafesheetname)(string) | Verifica el nombre de hoja proporcionado y crea uno válido cuando sea necesario. Si el nombre de hoja proporcionado cumple con las reglas de los nombres de hoja de Excel, lo devuelve. De lo contrario, la cadena se truncará si su longitud supera el límite y los caracteres no válidos se reemplazarán por ' ', luego se devuelve el valor de cadena reconstruido. |
| static [CreateSafeSheetName](../../aspose.cells/cellshelper/createsafesheetname/#createsafesheetname_1)(string, char) | Verifica el nombre de hoja proporcionado y crea uno válido cuando sea necesario. Si el nombre de hoja proporcionado cumple con las reglas de los nombres de hoja de Excel, lo devuelve. De lo contrario, la cadena se truncará si su longitud supera el límite y los caracteres no válidos se reemplazarán por el carácter especificado, luego se devuelve el valor de cadena reconstruido. |
| static [GetCacheFolder](../../aspose.cells/cellshelper/getcachefolder/)() | Obtiene la carpeta para archivos temporales que pueden usarse como caché de datos. |
| static [GetDateTimeFromDouble](../../aspose.cells/cellshelper/getdatetimefromdouble/)(double, bool) | Convierte el valor double al valor de fecha y hora. |
| static [GetDoubleFromDateTime](../../aspose.cells/cellshelper/getdoublefromdatetime/)(DateTime, bool) | Convierte la fecha y hora a un valor double. |
| static [GetTextWidth](../../aspose.cells/cellshelper/gettextwidth/)(string, Font, double) | Obtiene el ancho del texto en unidades de puntos. |
| static [GetUsedColors](../../aspose.cells/cellshelper/getusedcolors/)(Workbook) | Obtiene todos los colores usados en el libro de trabajo. |
| static [GetVersion](../../aspose.cells/cellshelper/getversion/)() | Obtiene la versión de lanzamiento. |
| static [MergeFiles](../../aspose.cells/cellshelper/mergefiles/)(string[], string, string) | Fusiona varios archivos xls grandes en un archivo xls. |
| static [NeedQuoteInFormula](../../aspose.cells/cellshelper/needquoteinformula/)(string) | Indica si el nombre de la hoja debe estar entre comillas simples |
| static [RowIndexToName](../../aspose.cells/cellshelper/rowindextoname/)(int) | Obtiene el nombre de fila según el índice de fila. |
| static [RowNameToIndex](../../aspose.cells/cellshelper/rownametoindex/)(string) | Obtiene el índice de fila según el nombre de fila. |
| static [SetCacheFolder](../../aspose.cells/cellshelper/setcachefolder/)(string) | Establece la carpeta para archivos temporales que pueden usarse como caché de datos. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsHelperDemo
    {
        public static void CellsHelperExample()
        {
            // Configurando propiedades de CellsHelper
            CellsHelper.SignificantDigits = 15;
            CellsHelper.DPI = 96.0;
            CellsHelper.StartupPath = "C:\\Program Files\\Aspose\\Cells";
            CellsHelper.AltStartPath = "D:\\Aspose\\Cells";
            CellsHelper.LibraryPath = "E:\\Aspose\\Cells\\Library";
            CellsHelper.IsCloudPlatform = true;

            // Suponiendo que CustomImplementationFactory ya está definido e instanciado en otro lugar
            CellsHelper.CustomImplementationFactory = new CustomImplementationFactory();

            // Demostrando el uso de las propiedades de CellsHelper
            Console.WriteLine("Significant Digits: " + CellsHelper.SignificantDigits);
            Console.WriteLine("DPI: " + CellsHelper.DPI);
            Console.WriteLine("Startup Path: " + CellsHelper.StartupPath);
            Console.WriteLine("Alternate Startup Path: " + CellsHelper.AltStartPath);
            Console.WriteLine("Library Path: " + CellsHelper.LibraryPath);
            Console.WriteLine("Is Cloud Platform: " + CellsHelper.IsCloudPlatform);

            // Ejemplo de uso de CustomImplementationFactory
            var memoryStream = CellsHelper.CustomImplementationFactory.CreateMemoryStream();
            Console.WriteLine("MemoryStream created with CustomImplementationFactory: " + (memoryStream != null));

            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


