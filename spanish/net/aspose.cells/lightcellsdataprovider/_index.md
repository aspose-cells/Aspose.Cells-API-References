---
title: "Interfaz LightCellsDataProvider"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Interfaz Aspose.Cells.LightCellsDataProvider. Representa el proveedor de datos para guardar archivos de hoja de cálculo grandes en modo ligero."
type: docs
url: /es/net/aspose.cells/lightcellsdataprovider/
---
## LightCellsDataProvider interface

Representa el proveedor de datos para guardar archivos de hoja de cálculo grandes en modo ligero.

```csharp
public interface LightCellsDataProvider
```

## Métodos

| Nombre | Descripción |
| --- | --- |
| [IsGatherString](../../aspose.cells/lightcellsdataprovider/isgatherstring/)() | Comprueba si el valor de cadena actual de la celda necesita recopilarse en un pool global. |
| [NextCell](../../aspose.cells/lightcellsdataprovider/nextcell/)() | Obtiene la siguiente celda a guardar. |
| [NextRow](../../aspose.cells/lightcellsdataprovider/nextrow/)() | Obtiene la siguiente fila a guardar. |
| [StartCell](../../aspose.cells/lightcellsdataprovider/startcell/)(Cell) | Comienza a guardar datos de una celda. |
| [StartRow](../../aspose.cells/lightcellsdataprovider/startrow/)(Row) | Comienza a guardar datos de una fila. |
| [StartSheet](../../aspose.cells/lightcellsdataprovider/startsheet/)(int) | Comienza a guardar una hoja de cálculo. |

### Observaciones

Al guardar un libro de trabajo con este modo, [`StartSheet`](./startsheet/) se verificará al guardar cada hoja de cálculo en el libro. Para una hoja, si [`StartSheet`](./startsheet/) devuelve true, entonces todos los datos y propiedades que se deben guardar para filas/celdas de esa hoja serán proporcionados por la implementación de esta interfaz. En primer lugar, se llamará a [`NextRow`](./nextrow/) para obtener el índice de la siguiente fila a guardar. Si se devuelve un índice de fila válido (el índice de fila debe estar en orden ascendente para las filas que se van a guardar), entonces un objeto Row que representa esa fila será proporcionado por [`StartRow`](./startrow/) para que la implementación establezca sus propiedades. Para una fila, se comprobará primero [`NextCell`](./nextcell/). Si se devuelve un índice de columna válido (el índice de columna debe estar en orden ascendente para todas las celdas de la fila actual), entonces un objeto Cell que representa esa celda será proporcionado por [`StartCell`](./startcell/) para que la implementación establezca sus datos y propiedades. Después de [`StartCell`](./startcell/) la celda se guardará directamente en el archivo de hoja de cálculo resultante. Luego se comprobará y procesará la siguiente celda.  Tenga en cuenta que el usuario solo debe actualizar los valores y propiedades del objeto Row/Cell actual proporcionado por el método correspondiente. Debido a que los datos de las celdas se escriben en el archivo resultante de forma continua, la mayoría de los demás objetos pueden haber sido ya escritos en el archivo resultante, o haberse recopilado y escrito algunos datos globales para ellos. Por lo tanto, cuando el usuario actualiza otros objetos mientras se guardan los datos de las celdas, esas operaciones pueden no afectar los datos guardados. O peor aún, esas operaciones pueden causar que datos inconsistentes se guarden en el archivo resultante y finalmente corrompan el archivo. Así que, para todos los demás objetos como formas, ancho de columnas y estilos, formatos condicionales, ...etc., por favor no los manipule en ningún método de esta implementación. En su lugar, adminístrelos y ajústelos al estado final antes de llamar al método "Save" del Workbook.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LightCellsDataProviderDemo
    {
        public static void LightCellsDataProviderExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear un LightCellsDataProvider personalizado
            CustomLightCellsDataProvider dataProvider = new CustomLightCellsDataProvider();

            // Establecer el LightCellsDataProvider para guardar el libro de trabajo
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions(SaveFormat.Xlsx)
            {
                LightCellsDataProvider = dataProvider
            };

            // Guardar el libro de trabajo con el LightCellsDataProvider personalizado
            workbook.Save("LightCellsDataProviderExample.xlsx", saveOptions);
        }
    }

    public class CustomLightCellsDataProvider : LightCellsDataProvider
    {
        private int currentRow = -1;
        private int currentCell = -1;

        public bool StartSheet(int sheetIndex)
        {
            // Comenzar a procesar la primera hoja
            return sheetIndex == 0;
        }

        public int NextRow()
        {
            // Moverse a la siguiente fila
            currentRow++;
            currentCell = -1;

            // Devolver el índice de fila actual o -1 si no hay más filas
            return currentRow < 10 ? currentRow : -1;
        }

        public void StartRow(Row row)
        {
            // Inicializar la fila si es necesario
        }

        public int NextCell()
        {
            // Moverse a la siguiente celda
            currentCell++;

            // Devolver el índice de celda actual o -1 si no hay más celdas
            return currentCell < 10 ? currentCell : -1;
        }

        public void StartCell(Cell cell)
        {
            // Establezca el valor de la celda
            cell.PutValue($"R{currentRow}C{currentCell}");
        }

        public bool IsGatherString()
        {
            // Devolver si se deben recopilar cadenas en un pool global
            return false;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


