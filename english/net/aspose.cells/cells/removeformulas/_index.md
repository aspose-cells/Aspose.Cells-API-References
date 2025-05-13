---
title: Cells.RemoveFormulas
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Removes all formula and replaces with the value of the formula
type: docs
url: /net/aspose.cells/cells/removeformulas/
---
## Cells.RemoveFormulas method

Removes all formula and replaces with the value of the formula.

```csharp
public void RemoveFormulas()
```

### Examples

```csharp
// Called: wkb.Worksheets[0].Cells.RemoveFormulas();
public void Cells_Method_RemoveFormulas()
{
    DataSet ds = new DataSet();

    DataTable dtMaster = new DataTable("Master");
    DataColumn dtcol1 = new DataColumn("ACCOUNT");
    DataColumn dtcol2 = new DataColumn("ACCOUNT_CREATEDBY_NAME");
    dtMaster.Columns.Add(dtcol1);
    dtMaster.Columns.Add(dtcol2);
    DataRow dr = dtMaster.NewRow();
    dr["ACCOUNT"] = "Test_Account";
    dr["ACCOUNT_CREATEDBY_NAME"] = "Test_user";
    dtMaster.Rows.Add(dr);
    ds.Tables.Add(dtMaster);

    DataTable lineIteams = new DataTable("OppLineItems");
    DataColumn lineIteamscol1 = new DataColumn("Id");
    lineIteamscol1.DataType = typeof(Int32);
    DataColumn lineIteamscol2 = new DataColumn("Name");
    DataColumn lineIteamscol3 = new DataColumn("SALESPRICE");
    lineIteamscol3.DataType = typeof(Int32);
    lineIteams.Columns.Add(lineIteamscol1);
    lineIteams.Columns.Add(lineIteamscol2);
    lineIteams.Columns.Add(lineIteamscol3);
    DataRow drlineIteams = lineIteams.NewRow();
    drlineIteams["Id"] = 1;
    drlineIteams["Name"] = "lineIteam1";
    drlineIteams["SALESPRICE"] = 10;
    lineIteams.Rows.Add(drlineIteams);

    DataRow drlineIteams2 = lineIteams.NewRow();
    drlineIteams2["Id"] = 2;
    drlineIteams2["Name"] = "lineIteam2";
    drlineIteams2["SALESPRICE"] = 20;
    lineIteams.Rows.Add(drlineIteams2);
    ds.Tables.Add(lineIteams);
    ds.AcceptChanges();


    Console.WriteLine($"Start.....");
    Workbook wkb = new Workbook(Constants.sourcePath + @"example.xlsx");
    WorkbookDesigner _designer = new WorkbookDesigner { Workbook = wkb };
    _designer.SetDataSource(ds);
    _designer.Process(false);


    //var dt = new DataTable("Empty");
    //_designer.SetDataSource(dt);
    //_designer.Process(false);

    wkb.CalculateFormula(true);
    wkb.Worksheets[0].Cells.RemoveFormulas();
    Assert.AreEqual("", wkb.Worksheets[0].Cells["A18"].StringValue);
    wkb.Save(Constants.destPath + @"example.xlsx");
}
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


