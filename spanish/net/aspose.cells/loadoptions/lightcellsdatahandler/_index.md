---
title: "LoadOptions.LightCellsDataHandler"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad LoadOptions. El controlador de datos para procesar los datos de celdas al leer el archivo de plantilla"
type: docs
url: /es/net/aspose.cells/loadoptions/lightcellsdatahandler/
---
## LoadOptions.LightCellsDataHandler property

El controlador de datos para procesar los datos de celdas al leer el archivo de plantilla.

```csharp
public LightCellsDataHandler LightCellsDataHandler { get; set; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyLightCellsDataHandlerDemo
    {
        public static void Run()
        {
            // Crear un LightCellsDataHandler personalizado para procesar los datos de celdas
            var dataHandler = new CustomLightCellsDataHandler();
            
            // Crear opciones de carga y establecer el controlador de datos
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.LightCellsDataHandler = dataHandler;

            // Cargar el libro de trabajo con el controlador personalizado
            using (Workbook workbook = new Workbook("sample.xlsx", loadOptions))
            {
                Console.WriteLine("Workbook processed successfully with LightCellsDataHandler");
            }
        }
    }

    public class CustomLightCellsDataHandler : LightCellsDataHandler
    {
        public bool StartSheet(Worksheet sheet)
        {
            Console.WriteLine($"Processing sheet: {sheet.Name}");
            return true; // Continue processing this sheet
        }

        public bool StartRow(int rowIndex)
        {
            Console.WriteLine($"  Starting row: {rowIndex}");
            return true; // Continue processing this row
        }

        public bool ProcessRow(Row row)
        {
            // Puede procesar los datos de fila aquí si es necesario
            return true;
        }

        public bool StartCell(int columnIndex)
        {
            Console.WriteLine($"    Starting cell at column: {columnIndex}");
            return true; // Continue processing this cell
        }

        public bool ProcessCell(Cell cell)
        {
            Console.WriteLine($"      Cell[{cell.Row},{cell.Column}]: {cell.Value}");
            return true;
        }
    }
}
```

### Ver también

* interface [LightCellsDataHandler](../../lightcellsdatahandler/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


