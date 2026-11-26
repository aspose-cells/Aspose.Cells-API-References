---
title: "Clase WorkbookDesigner"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.WorkbookDesigner. Encapsula el objeto que representa una hoja de cálculo de diseño"
type: docs
url: /es/net/aspose.cells/workbookdesigner/
---
## WorkbookDesigner class

Encapsula el objeto que representa una hoja de cálculo de diseñador.

```csharp
public class WorkbookDesigner
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [WorkbookDesigner](workbookdesigner/#constructor)() | Inicializa una nueva instancia de la clase `WorkbookDesigner`. |
| [WorkbookDesigner](workbookdesigner/#constructor_1)(Workbook) | Inicializa una nueva instancia de la clase `WorkbookDesigner`. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [CalculateFormula](../../aspose.cells/workbookdesigner/calculateformula/) { get; set; } | Indica si las fórmulas deben calcularse. |
| [CallBack](../../aspose.cells/workbookdesigner/callback/) { get; set; } | Obtiene y establece la interfaz de devolución de llamada del procesamiento de smartmarker. |
| [ContainsVariables](../../aspose.cells/workbookdesigner/containsvariables/) { get; set; } | (**Obsolete.**) Indica si la primera hoja de cálculo contiene variables personalizadas. |
| [EnableHeaderFooterMarkers](../../aspose.cells/workbookdesigner/enableheaderfootermarkers/) { get; set; } | Indica si el encabezado/pie de página contiene smart markers y debe procesarse junto. |
| [LineByLine](../../aspose.cells/workbookdesigner/linebyline/) { get; set; } | (**Obsolete.**) Indica si el procesamiento del marcador inteligente se realiza línea por línea. |
| [RepeatFormulasWithSubtotal](../../aspose.cells/workbookdesigner/repeatformulaswithsubtotal/) { get; set; } | Indica si se repiten fórmulas con fila de subtotal. |
| [SortDataSource](../../aspose.cells/workbookdesigner/sortdatasource/) { get; set; } | Indica si se ordena la fuente de datos. |
| [UpdateEmptyStringAsNull](../../aspose.cells/workbookdesigner/updateemptystringasnull/) { get; set; } | Si TRUE, se insertará Null si el valor es ""; |
| [UpdateReference](../../aspose.cells/workbookdesigner/updatereference/) { get; set; } | Indica si las referencias en otras hojas de cálculo se actualizarán. |
| [VariablesWorksheetName](../../aspose.cells/workbookdesigner/variablesworksheetname/) { get; set; } | Obtiene y establece el nombre de la hoja de cálculo que contiene variables smart marker. |
| [Workbook](../../aspose.cells/workbookdesigner/workbook/) { get; set; } | Obtiene y establece el objeto [`Workbook`](./workbook/). |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [ClearDataSource](../../aspose.cells/workbookdesigner/cleardatasource/)() | Borra todas las fuentes de datos. |
| [GetSmartMarkers](../../aspose.cells/workbookdesigner/getsmartmarkers/)() | Devuelve una colección de marcadores inteligentes en una hoja de cálculo. |
| [Process](../../aspose.cells/workbookdesigner/process/#process)() | Procesa los marcadores inteligentes y rellena los valores de la fuente de datos. |
| [Process](../../aspose.cells/workbookdesigner/process/#process_2)(bool) | Procesa los marcadores inteligentes y rellena los valores de la fuente de datos. |
| [Process](../../aspose.cells/workbookdesigner/process/#process_3)(int, bool) | Procesa los marcadores inteligentes y rellena los valores de la fuente de datos. |
| [Process](../../aspose.cells/workbookdesigner/process/#process_1)(Range, bool) | (**Obsoleto.**) Procesa los marcadores inteligentes y rellena los valores de la fuente de datos. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource)(DataSet) | Establece la fuente de datos de un objeto DataSet. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_1)(DataTable) | Establece la fuente de datos de un objeto DataTable. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_2)(DataView) | Establece la fuente de datos de un objeto DataView. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_3)(OleDbConnection) | Establece la fuente de datos de un objeto OleDbConnection. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_4)(SqlConnection) | Establece la fuente de datos de un objeto SqlConnection. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_6)(string, DataView) | Establece la fuente de datos de un objeto DataView y lo vincula a un nombre de fuente de datos. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_5)(string, ICellsDataTable) | Establece la fuente de datos de un objeto [`ICellsDataTable`](../icellsdatatable/). |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_8)(string, object) | Establece el enlace de datos a una variable. |
| [SetDataSource](../../aspose.cells/workbookdesigner/setdatasource/#setdatasource_7)(string, IDataReader, int) | Establece la fuente de datos de un objeto IDataReader. |
| [SetJsonDataSource](../../aspose.cells/workbookdesigner/setjsondatasource/)(string, string) | Establece el valor de cadena JSON como fuente de datos de los marcadores inteligentes. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Data;

    public class WorkbookDesignerDemo
    {
        public static void WorkbookDesignerExample()
        {
            // Crear objeto WorkbookDesigner
            WorkbookDesigner wd = new WorkbookDesigner();

            // Abrir el archivo de plantilla (que contiene marcadores inteligentes)
            wd.Workbook = new Workbook("SmartMarker_Designer_original.xlsx");

            // Inicialice sus datos desde la fuente de datos
            DataSet ds = new DataSet();
            // Agregar datos al conjunto de datos (esto es solo un ejemplo, reemplazar con la fuente de datos real)
            DataTable dt = new DataTable("Table1");
            dt.Columns.Add("Column1");
            dt.Columns.Add("Column2");
            dt.Rows.Add("Value1", "Value2");
            dt.Rows.Add("Value11", "Value22");
            ds.Tables.Add(dt);

            // Establecer el conjunto de datos como la fuente de datos
            wd.SetDataSource(ds);

            // Procese los smart markers para rellenar los datos en las hojas de cálculo
            wd.Process(true);

            // Guardar el archivo Excel
            wd.Workbook.Save("WorkbookDesignerExample.xlsx");

            // Demostrando otras propiedades
            wd.RepeatFormulasWithSubtotal = true;
            wd.UpdateEmptyStringAsNull = true;
            wd.UpdateReference = true;
            wd.CalculateFormula = true;
            wd.LineByLine = true;

            // Borrar la fuente de datos
            wd.ClearDataSource();

            // Establecer la fuente de datos usando diferentes métodos
            wd.SetDataSource("dataSourceName", dt);
            wd.SetDataSource(dt);
            wd.SetDataSource(ds);
            wd.SetDataSource("dataSourceName", new DataView(dt));
            wd.SetDataSource(new DataView(dt));
            wd.SetDataSource("name", new DataTableReader(dt), dt.Rows.Count);
            wd.SetJsonDataSource("variable", "{\"key\":\"value\"}");
            wd.SetDataSource("variable", new object());

            // Procesar los marcadores inteligentes nuevamente
            wd.Process();
            wd.Process(true);
            wd.Process(0, true);

            // Guardar el archivo Excel nuevamente
            wd.Workbook.Save("WorkbookDesignerExample_SmartMarker_Designer_Processed.xlsx");

            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


