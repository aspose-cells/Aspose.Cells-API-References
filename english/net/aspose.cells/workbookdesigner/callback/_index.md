---
title: WorkbookDesigner.CallBack
second_title: Aspose.Cells for .NET API Reference
description: WorkbookDesigner property. Gets and sets callback interface of processing smartmarker
type: docs
url: /net/aspose.cells/workbookdesigner/callback/
---
## WorkbookDesigner.CallBack property

Gets and sets callback interface of processing smartmarker.

```csharp
public ISmartMarkerCallBack CallBack { get; set; }
```

### Examples

```csharp
// Called: designer.CallBack = new ISmartMarkerCallBackDemo();
public static void Property_CallBack()
        {
            // Create a new WorkbookDesigner instance
            WorkbookDesigner designer = new WorkbookDesigner();
            // Open a template file (which contains smart markers)
            designer.Workbook = new Workbook("ISmartMarkerCallBackExample_original.xlsx");

            // Set the callback interface
            designer.CallBack = new ISmartMarkerCallBackDemo();

            // Initialize your data from data source
            // For demonstration, we will use a simple DataTable
            System.Data.DataTable dataTable = new System.Data.DataTable("Table1");
            dataTable.Columns.Add("Column1", typeof(string));
            dataTable.Rows.Add("Value1");
            dataTable.Rows.Add("Value2");

            // Set the datatable as the data source
            designer.SetDataSource(dataTable);

            // Process the smart markers to fill the data into the worksheets
            designer.Process(true);

            // Save the excel file
            designer.Workbook.Save("ISmartMarkerCallBackExample.xlsx");
        }
```

### See Also

* interface [ISmartMarkerCallBack](../../ismartmarkercallback/)
* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


