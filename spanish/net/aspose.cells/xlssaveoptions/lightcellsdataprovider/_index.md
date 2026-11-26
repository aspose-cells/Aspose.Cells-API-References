---
title: "XlsSaveOptions.LightCellsDataProvider"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de XlsSaveOptions. El proveedor de datos para guardar el libro de trabajo en modo ligero"
type: docs
url: /es/net/aspose.cells/xlssaveoptions/lightcellsdataprovider/
---
## XlsSaveOptions.LightCellsDataProvider property

El proveedor de datos para guardar el libro de trabajo en modo ligero.

```csharp
public LightCellsDataProvider LightCellsDataProvider { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XlsSaveOptionsPropertyLightCellsDataProviderDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            
            // Crear opciones de guardado XLS
            XlsSaveOptions saveOptions = new XlsSaveOptions();
            
            // Establecer el LightCellsDataProvider
            saveOptions.LightCellsDataProvider = new CustomLightCellsDataProvider();
            
            // Guardar el libro de trabajo con modo LightCells
            workbook.Save("output.xls", saveOptions);
        }
    }

    public class CustomLightCellsDataProvider : LightCellsDataProvider
    {
        public bool IsGatherString()
        {
            return true;
        }

        public int NextCell()
        {
            return 0; // Only process first cell for demonstration
        }

        public int NextRow()
        {
            return 0; // Only process first row for demonstration
        }

        public void StartCell(Cell cell)
        {
            // Establecer un valor de cadena largo para demostrar el manejo de LightCells
            cell.PutValue(new string('X', 257));
        }

        public void StartRow(Row row)
        {
            // No se necesita un manejo especial de filas para esta demostración
        }

        public bool StartSheet(int sheetIndex)
        {
            // No se necesita un manejo especial de hojas para esta demostración
            return false;
        }
    }
}
```

### Ver también

* interface [LightCellsDataProvider](../../lightcellsdataprovider/)
* class [XlsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


