---
title: "Enumeración ExceptionType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.ExceptionType. Representa un código de tipo de excepción personalizado"
type: docs
url: /es/net/aspose.cells/exceptiontype/
---
## ExceptionType enumeration

Representa el código del tipo de excepción personalizada.

```csharp
public enum ExceptionType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Chart | `0` | Configuración de gráfico no válida. |
| DataType | `1` | Configuración de tipo de datos no válida. |
| DataValidation | `2` | Configuración de validación de datos no válida. |
| ConditionalFormatting | `3` | Configuración de validación de datos no válida. |
| FileFormat | `4` | Formato de archivo no válido. |
| Formula | `5` | Fórmula inválida. |
| InvalidData | `6` | Datos inválidos. |
| InvalidOperator | `7` | Operador inválido. |
| IncorrectPassword | `8` | Contraseña incorrecta. |
| License | `9` | Errores relacionados con la licencia. |
| Limitation | `10` | Error por exceder la limitación de MS Excel. |
| PageSetup | `11` | Configuración de configuración de página no válida. |
| PivotTable | `12` | Configuración de tabla dinámica no válida. |
| Shape | `13` | Configuración de objeto de dibujo no válida. |
| Sparkline | `14` | Configuración de objeto de línea de tendencia no válida. |
| SheetName | `15` | Nombre de hoja de cálculo no válido. |
| SheetType | `16` | Tipo de hoja de cálculo no válido. |
| Interrupted | `17` | El proceso está interrumpido. |
| IO | `18` | El archivo es inválido. |
| Permission | `19` | Se requiere permiso para abrir este archivo. |
| UnsupportedFeature | `20` | Funcionalidad no soportada. |
| UnsupportedStream | `21` | Flujo no soportado para abrir. |
| UndisclosedInformation | `22` | Los archivos contienen información no revelada. |
| FileCorrupted | `23` | El contenido del archivo está corrupto. |
| DefinedName | `25` | Nombre definido no válido |
| Font | `26` | Fuente no válida |
| AutoFilter | `27` | Configuración de filtro automático no válida. |
| FontSubstitution | `28` | Tipo de advertencia de sustitución de fuente cuando no se encuentra una fuente, este tipo de advertencia se puede obtener. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ExceptionTypeDemo
    {
        public static void ExceptionTypeExample()
        {
            try
            {
                // Crear un nuevo libro de trabajo
                Workbook workbook = new Workbook();

                // Intento de establecer un nombre de hoja de cálculo no válido para generar una excepción
                workbook.Worksheets[0].Name = "Invalid/Name";

                // Guarda el libro de trabajo
                workbook.Save("ExceptionTypeExample.xlsx");
            }
            catch (CellsException ex)
            {
                // Manejar la CellsException
                Console.WriteLine("An error occurred: " + ex.Message);
                Console.WriteLine("Exception Type Code: " + ex.Code);
                
                // Verifique el tipo de excepción
                switch (ex.Code)
                {
                    case ExceptionType.SheetName:
                        Console.WriteLine("The worksheet name is invalid.");
                        break;
                    case ExceptionType.FileFormat:
                        Console.WriteLine("The file format is invalid.");
                        break;
                    // Agregue más casos según sea necesario para diferentes tipos de excepción
                    default:
                        Console.WriteLine("An unknown error occurred.");
                        break;
                }
            }
            catch (Exception ex)
            {
                // Maneje cualquier otra excepción
                Console.WriteLine("An unexpected error occurred: " + ex.Message);
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


