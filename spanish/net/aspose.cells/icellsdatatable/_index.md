---
title: "Interfaz ICellsDataTable"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Interfaz Aspose.Cells.ICellsDataTable. Representa una tabla de datos"
type: docs
url: /es/net/aspose.cells/icellsdatatable/
---
## ICellsDataTable interface

Representa una tabla de datos.

```csharp
public interface ICellsDataTable
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Columns](../../aspose.cells/icellsdatatable/columns/) { get; } | Obtiene el nombre de las columnas. |
| [Count](../../aspose.cells/icellsdatatable/count/) { get; } | Obtiene el recuento de los registros. -1 para recuento de registros desconocido. |
| [Item](../../aspose.cells/icellsdatatable/item/) { get; } | Obtiene los datos almacenados en la columna especificada por índice. (2 indexadores) |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [BeforeFirst](../../aspose.cells/icellsdatatable/beforefirst/)() | Mueve el cursor al inicio de este objeto, justo antes de la primera fila. |
| [Next](../../aspose.cells/icellsdatatable/next/)() | Mueve el cursor una fila hacia abajo desde su posición actual. |

### Ejemplos

```csharp
using System;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassICellsDataTableDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();

            ArrayList dataLists = new ArrayList();
            ArrayList list1 = new ArrayList();
            list1.AddRange(new object[] { "Name", "Age", "Gender" });
            ArrayList list2 = new ArrayList();
            list2.AddRange(new object[] { "Alice", 30, "Female" });
            ArrayList list3 = new ArrayList();
            list3.AddRange(new object[] { "Bob", 25, "Male" });
            ArrayList list4 = new ArrayList();
            list4.AddRange(new object[] { "Charlie", 35, "Male" });
            dataLists.Add(list1);
            dataLists.Add(list2);
            dataLists.Add(list3);
            dataLists.Add(list4);

            ICellsDataTable dt = wb.CellsDataTableFactory.GetInstance(dataLists, true);
            
            wb.Worksheets[0].Cells.ImportData(dt, 0, 0, new ImportTableOptions());
            Console.WriteLine("First worksheet A2 value: " + wb.Worksheets[0].Cells["A2"].StringValue);

            wb.Worksheets.Add();
            wb.Worksheets[1].Cells.ImportArrayList(dataLists, 0, 0, true);
            Console.WriteLine("Second worksheet A3 value: " + wb.Worksheets[1].Cells["A3"].StringValue);
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


