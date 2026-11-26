---
title: "Interfaz LightCellsDataHandler"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Interfaz Aspose.Cells.LightCellsDataHandler. Representa el manejador de datos de celdas para leer archivos de hoja de cálculo grandes en modo ligero."
type: docs
url: /es/net/aspose.cells/lightcellsdatahandler/
---
## LightCellsDataHandler interface

Representa el manejador de datos de celdas para leer archivos de hoja de cálculo grandes en modo ligero.

```csharp
public interface LightCellsDataHandler
```

## Métodos

| Nombre | Descripción |
| --- | --- |
| [ProcessCell](../../aspose.cells/lightcellsdatahandler/processcell/)(Cell) | Comienza a procesar una celda. |
| [ProcessRow](../../aspose.cells/lightcellsdatahandler/processrow/)(Row) | Comienza a procesar una fila. |
| [StartCell](../../aspose.cells/lightcellsdatahandler/startcell/)(int) | Prepara procesar una celda. |
| [StartRow](../../aspose.cells/lightcellsdatahandler/startrow/)(int) | Prepara procesar una fila. |
| [StartSheet](../../aspose.cells/lightcellsdatahandler/startsheet/)(Worksheet) | Comienza a procesar una hoja de cálculo. |

### Observaciones

Al leer un libro de trabajo en este modo, [`StartSheet`](./startsheet/) se verificará al leer cada hoja de cálculo del libro. Para una hoja, si [`StartSheet`](./startsheet/) devuelve true, entonces todos los datos y propiedades de filas/celdas de esa hoja serán verificados y procesados por la implementación de esta interfaz. Para cada fila, se llamará a [`StartRow`](./startrow/) para comprobar si necesita ser procesada. Si una fila necesita ser procesada, sus propiedades se leerán primero y el usuario podrá acceder a ellas mediante [`ProcessRow`](./processrow/). Si también es necesario procesar las celdas de la fila, entonces [`ProcessRow`](./processrow/) debe devolver true y luego se llamará a [`StartCell`](./startcell/) para cada celda existente en esa fila para comprobar si una celda necesita ser procesada. Si una celda necesita ser procesada, se llamará a [`ProcessCell`](./processcell/) para procesarla mediante la implementación de esta interfaz.  Tenga en cuenta que el usuario solo debe operar sobre los valores y propiedades del objeto Row/Cell actual proporcionado por el método correspondiente. Debido a que los datos de las celdas se leen del archivo de plantilla de forma streaming, la mayoría de los demás objetos pueden ser restablecidos/actualizados más tarde después de que los datos de las celdas se hayan cargado. Por lo tanto, al operar con otros objetos en esta implementación, esas operaciones pueden no afectar a los objetos existentes en el libro de trabajo. O peor aún, esas operaciones pueden causar datos inconsistentes en el libro y generar problemas o excepciones inesperadas más adelante. Así que, para todos los demás objetos como formas, ancho de columnas y estilos, formatos condicionales, ...etc., por favor no los manipule en ninguno de los métodos de esta implementación. En su lugar, adminístrelos después de que el libro de trabajo haya sido construido.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LightCellsDataHandlerDemo : LightCellsDataHandler
    {
        public static void LightCellsDataHandlerExample()
        {
            // Crear un libro de trabajo y cargarlo con LightCellsDataHandler
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear una instancia de LightCellsDataHandlerDemo
            LightCellsDataHandlerDemo handler = new LightCellsDataHandlerDemo();

            // Establecer el LightCellsDataHandler para el libro de trabajo
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.LightCellsDataHandler = handler;

            // Cargar el libro de trabajo con las opciones de carga especificadas
            workbook = new Workbook("LargeFile_original.xlsx", loadOptions);

            // Guardar el libro de trabajo para demostrar el proceso
            workbook.Save("ProcessedLargeFile.xlsx");
        }

        // Implementar el método StartSheet
        public bool StartSheet(Worksheet sheet)
        {
            Console.WriteLine("Starting to process sheet: " + sheet.Name);
            return true; // Continue processing
        }

        // Implementar el método StartRow
        public bool StartRow(int rowIndex)
        {
            Console.WriteLine("Starting to process row: " + rowIndex);
            return true; // Continue processing
        }

        // Implementar el método ProcessRow
        public bool ProcessRow(Row row)
        {
            Console.WriteLine("Processing row: " + row.Index);
            return true; // Continue processing
        }

        // Implementar el método StartCell
        public bool StartCell(int columnIndex)
        {
            Console.WriteLine("Starting to process cell in column: " + columnIndex);
            return true; // Continue processing
        }

        // Implementar el método ProcessCell
        public bool ProcessCell(Cell cell)
        {
            Console.WriteLine("Processing cell: " + cell.Name + " with value: " + cell.StringValue);
            return true; // Continue processing
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


