---
title: "WorkbookDesigner.CallBack"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad WorkbookDesigner. Obtiene y establece la interfaz de devolución de llamada del procesamiento de smartmarker"
type: docs
url: /es/net/aspose.cells/workbookdesigner/callback/
---
## WorkbookDesigner.CallBack property

Obtiene y establece la interfaz de devolución de llamada del procesamiento de smartmarker.

```csharp
public ISmartMarkerCallBack CallBack { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerPropertyCallBackDemo : ISmartMarkerCallBack
    {
        public void Process(int sheetIndex, int rowIndex, int colIndex, string tableName, string columnName)
        {
            Console.WriteLine($"Processing - Sheet: {sheetIndex}, Row: {rowIndex}, Column: {colIndex}");
            Console.WriteLine($"Table: {tableName}, Column: {columnName}");
        }

        public static void Run()
        {
            WorkbookDesigner designer = new WorkbookDesigner();
            designer.Workbook = new Workbook();
            
            Worksheet worksheet = designer.Workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("&=$Table1.Column1");
            
            designer.CallBack = new WorkbookDesignerPropertyCallBackDemo();

            System.Data.DataTable dataTable = new System.Data.DataTable("Table1");
            dataTable.Columns.Add("Column1", typeof(string));
            dataTable.Rows.Add("Data1");
            dataTable.Rows.Add("Data2");

            designer.SetDataSource(dataTable);
            designer.Process(false);
            
            designer.Workbook.Save("WorkbookDesignerCallBackDemo.xlsx");
        }
    }
}
```

### Ver también

* interface [ISmartMarkerCallBack](../../ismartmarkercallback/)
* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


