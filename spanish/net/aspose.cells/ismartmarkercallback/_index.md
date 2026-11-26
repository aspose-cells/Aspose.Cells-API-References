---
title: "Interfaz ISmartMarkerCallBack"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Interfaz Aspose.Cells.ISmartMarkerCallBack. Representa la interfaz de devolución de llamada del procesamiento de smartmarker"
type: docs
url: /es/net/aspose.cells/ismartmarkercallback/
---
## ISmartMarkerCallBack interface

Representa la interfaz de devolución de llamada del procesamiento de smartmarker.

```csharp
public interface ISmartMarkerCallBack
```

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Process](../../aspose.cells/ismartmarkercallback/process/)(int, int, int, string, string) | Devolución de llamada para procesar un smart marker. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ISmartMarkerCallBackDemo : ISmartMarkerCallBack
    {
        // Implementando el método Process de la interfaz ISmartMarkerCallBack
        public void Process(int sheetIndex, int rowIndex, int colIndex, string tableName, string columnName)
        {
            // Ejemplo de implementación del método Process
            Console.WriteLine($"Processing sheetIndex: {sheetIndex}, rowIndex: {rowIndex}, colIndex: {colIndex}, tableName: {tableName}, columnName: {columnName}");
        }

        public static void ISmartMarkerCallBackExample()
        {
            // Cree una nueva instancia de WorkbookDesigner
            WorkbookDesigner designer = new WorkbookDesigner();
            // Abra un archivo de plantilla (que contiene smart markers)
            designer.Workbook = new Workbook("ISmartMarkerCallBackExample_original.xlsx");

            // Establezca la interfaz de devolución de llamada
            designer.CallBack = new ISmartMarkerCallBackDemo();

            // Inicialice sus datos desde la fuente de datos
            // Para demostración, utilizaremos una DataTable simple
            System.Data.DataTable dataTable = new System.Data.DataTable("Table1");
            dataTable.Columns.Add("Column1", typeof(string));
            dataTable.Rows.Add("Value1");
            dataTable.Rows.Add("Value2");

            // Establezca la DataTable como la fuente de datos
            designer.SetDataSource(dataTable);

            // Procese los smart markers para rellenar los datos en las hojas de cálculo
            designer.Process(true);

            // Guardar el archivo Excel
            designer.Workbook.Save("ISmartMarkerCallBackExample.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


