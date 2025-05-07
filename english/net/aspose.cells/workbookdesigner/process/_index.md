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
[Test]
        public void Method_Boolean_()
        {
            Workbook wb = new Workbook(Constants.sourcePath + "CELLSJAVA46279.xlsx");
            WorkbookDesigner designer = new WorkbookDesigner();
            designer.LineByLine = (false);
            designer.Workbook = (wb);
            designer.SetJsonDataSource("RootData", File.ReadAllText(Constants.sourcePath + "CELLSJAVA46279.json"));
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
            wb.Save(Constants.destPath + "CELLSJAVA46279.xlsx");
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
// Called: designer.Process();
[Test]
        public void Method_Process()
        {
            Workbook wb = new Workbook(Constants.sourcePath + "CELLSJAVA45705_2.xlsx");
            String data = "{\n" + "    \"array\": [\n" + "        \"English\",\n" + "        \"Arabic\",\n"
                  + "        \"Hindi\",\n" + "        \"Urdu\",\n" + "        \"French\"\n" + "    ],\n"
                  + "    \"var\": \"This is a sentence using one place holder\",\n" + "\"arrObj\": [\n" + "    {\n"
                  + "        \"name\": \"John Doe\",\n" + "        \"age\": \"27\"\n" + "    },\n" + "    {\n"
                  + "        \"name\": \"Jane Doe\",\n" + "        \"age\": \"27\"\n" + "    }\n" + "]" + "}";

            WorkbookDesigner designer = new WorkbookDesigner(wb);
            designer.SetJsonDataSource("ds", data);
            designer.LineByLine = false;

            designer.Process();
            wb.Save(Constants.destPath + "CELLSJAVA45705_2.xlsx");
            Assert.AreEqual("Arabic", wb.Worksheets[0].Cells["A9"].StringValue);
            Assert.AreEqual("27", wb.Worksheets[0].Cells["B3"].StringValue);

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
[Test]
        public void Method_Boolean_()
        {
            Workbook wb = new Workbook(Constants.sourcePath + "JAVA45749.xlsx");
            wb.Worksheets[0].Cells.CreateRange("A4:K19").Name = ("_CellsSmartMarkers");
            WorkbookDesigner designer = new WorkbookDesigner();
            designer.LineByLine = (false);
            designer.Workbook = (wb);
            designer.SetJsonDataSource("RootData", File.ReadAllText(Constants.sourcePath + "CellsJava45708.json"));
            // designer.SetDataSource("Directors", res.Directors);
            designer.Process(true);
            ListObject listObject = wb.Worksheets[0].ListObjects[0];
            Assert.AreEqual(47,listObject.EndRow);
            Chart chart = wb.Worksheets[0].Charts[0];
            Assert.AreEqual("=Template!$D$47:$D$48",chart.NSeries[0].Values);//=Template!$D$47:$D$48
            wb.Save(Constants.destPath + "JAVA45749.xlsx");
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
[Test]
        public void Method_Boolean_()
        {
            var book = new Workbook(Constants.sourcePath + "SmartMarker/CellsNet44389.xlsx");
            var table = book.Worksheets["Data"].Cells.ExportDataTable(0, 0, book.Worksheets["Data"].Cells.MaxDataRow, book.Worksheets["Data"].Cells.MaxDataColumn + 1, new ExportTableOptions() { CheckMixedValueType = true, ExportColumnName = true });
            table.TableName = "Table";

            var designer = new WorkbookDesigner();

            //Assign the Workbook property to the instance of Workbook created in first step
            designer.Workbook = book;

            //Set the data source
            designer.SetDataSource(table);

            //Call Process method to populate data
            designer.Process(0, true);

            designer.Workbook.Save(Constants.destPath + "CellsNet44389.xlsx");
            Assert.AreEqual("=SUM(E3:E9)/SUM(B3:B9)", book.Worksheets[0].Cells["E10"].Formula);
            Assert.AreEqual("1594", book.Worksheets[0].Cells["C9"].StringValue);
        }
```

### See Also

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


