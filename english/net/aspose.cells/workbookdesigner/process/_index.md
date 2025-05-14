---
title: WorkbookDesigner.Process
second_title: Aspose.Cells for .NET API Reference
description: WorkbookDesigner method. Processes the smart markers and populates the data source values
type: docs
url: /net/aspose.cells/workbookdesigner/process/
---
## Process(Range, bool) {#process_1}

Processes the smart markers and populates the data source values.

```csharp
public void Process(Range range, bool isPreserved)
```

| Parameter | Type | Description |
| --- | --- | --- |
| range | Range | The range to be processed |
| isPreserved | Boolean | True if the unrecognized smart marker is preserved. |

### Examples

```csharp
// Called: designer.Process(range, true);
public void WorkbookDesigner_Method_Process()
{
    Workbook wb = new Workbook(Constants.sourcePath + @"example.xlsx");
    WorkbookDesigner designer = new WorkbookDesigner();
    designer.LineByLine = (false);
    designer.Workbook = (wb);
    designer.SetJsonDataSource("RootData", File.ReadAllText(Constants.sourcePath + @"example.json"));
    Aspose.Cells.Range range = wb.Worksheets[0].Cells.CreateRange("A24:H28");
    range.Name = "_CellsSmartMarkers";
    designer.Process(range, true);

    range = wb.Worksheets[0].Cells.CreateRange("A18:D19");
    range.Name = "_CellsSmartMarkers";
    designer.Process(range, true);

    range = wb.Worksheets[0].Cells.CreateRange("A2:H15");
    range.Name = "_CellsSmartMarkers";
    designer.Process(range, true);
    Assert.AreEqual("director last 2", wb.Worksheets[0].Cells["D38"].StringValue);
    Assert.AreEqual("fff department", wb.Worksheets[0].Cells["H61"].StringValue);
    wb.Save(Constants.destPath + @"example.xlsx");
}
```

### See Also

* class [Range](../../range/)
* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Process() {#process}

Processes the smart markers and populates the data source values.

```csharp
public void Process()
```

### Examples

```csharp
// Called: d.Process();
public void WorkbookDesigner_Method_Process()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    WorkbookDesigner d = new WorkbookDesigner(workbook);
    ArrayList list = new ArrayList();
    Person p = new Person("abc", 1);
    p.FOTO = File.ReadAllBytes(Constants.sourcePath + "1.jpg");
    list.Add(p);
    p = new Person("abc", 1);
    p.FOTO = File.ReadAllBytes(Constants.sourcePath + "1.jpg");
    list.Add(p);
    d.SetDataSource("Datos", list);
    d.Process();
    Assert.AreEqual(workbook.Worksheets[0].Pictures.Count, 2);
}
```

### See Also

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Process(bool) {#process_2}

Processes the smart markers and populates the data source values.

```csharp
public void Process(bool isPreserved)
```

| Parameter | Type | Description |
| --- | --- | --- |
| isPreserved | Boolean | True if the unrecognized smart marker is preserved. |

### Examples

```csharp
// Called: designer.Process(true);
public void WorkbookDesigner_Method_Process()
{
    Workbook wb = new Workbook(Constants.sourcePath + "example.xlsx");
    JsonSerializer serializer = new JsonSerializer();
    // TextReader rdr = new StringReader(dir + "t (2).json");
    // ABC_1_Data p1 = (ABC_1_Data)serializer.Deserialize(new JsonTextReader(rdr), typeof(ABC_1_Data));
    ABC_1_Data res = (ABC_1_Data)JsonConvert.DeserializeObject(File.ReadAllText(Constants.sourcePath + "example.json"), typeof(ABC_1_Data));

    //		
    wb.Worksheets[0].Cells.CreateRange("A13:K19").Name = ("_CellsSmartMarkers");
    //		// Load the data from the input json file
    List<ABC_1_Data> listFormData = new List<ABC_1_Data>();
    listFormData.Add(res);
    WorkbookDesigner designer = new WorkbookDesigner();
    designer.LineByLine = (false);
    designer.Workbook = (wb);
    designer.SetDataSource("RootData", listFormData);
    designer.SetDataSource("Directors", res.Directors);
    designer.Process(true);
    wb.Save(Constants.destPath + "example.xlsx");
    Assert.AreEqual("DRFNAME2", wb.Worksheets[0].Cells["G31"].StringValue);
           
}
```

### See Also

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Process(int, bool) {#process_3}

Processes the smart markers and populates the data source values.

```csharp
public void Process(int sheetIndex, bool isPreserved)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sheetIndex | Int32 | Worksheet index. |
| isPreserved | Boolean | True if the unrecognized smart marker is preserved. |

### Remarks

This method works on worksheet level.

### Examples

```csharp
// Called: designer.Process(0, true);
public void WorkbookDesigner_Method_Process()
{
    var book = new Workbook(Constants.sourcePath + "example.xlsx");
    var table = book.Worksheets["Data"].Cells.ExportDataTable(0, 0, book.Worksheets["Data"].Cells.MaxDataRow, book.Worksheets["Data"].Cells.MaxDataColumn + 1, new ExportTableOptions() { CheckMixedValueType = true, ExportColumnName = true });
    table.TableName = "Table";

    var designer = new WorkbookDesigner();

    //Assign the Workbook property to the instance of Workbook created in first step
    designer.Workbook = book;

    //Set the data source
    designer.SetDataSource(table);

    //Call Process method to populate data
    designer.Process(0, true);

    designer.Workbook.Save(Constants.destPath + "example.xlsx");
    Assert.AreEqual("=SUM(E3:E9)/SUM(B3:B9)", book.Worksheets[0].Cells["E10"].Formula);
    Assert.AreEqual("1594", book.Worksheets[0].Cells["C9"].StringValue);
}
```

### See Also

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


