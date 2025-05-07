---
title: WorksheetCollection.AddCopy
second_title: Aspose.Cells for .NET API Reference
description: WorksheetCollection method. Adds a worksheet to the collection and copies data from an existed worksheet
type: docs
url: /net/aspose.cells/worksheetcollection/addcopy/
---
## AddCopy(string) {#addcopy_1}

Adds a worksheet to the collection and copies data from an existed worksheet.

```csharp
public int AddCopy(string sheetName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sheetName | String | Name of source worksheet. |

### Return Value

[`Worksheet`](../../worksheet/) object index.

### Exceptions

| exception | condition |
| --- | --- |
| [CellsException](../../cellsexception/) | Specifies an invalid worksheet name. |

### Examples

```csharp
// Called: int iDesign = wb.Worksheets.AddCopy("Designer");
[Test]
         //http://www.aspose.com/community/forums/thread/347146.aspx
         public void Method_String_()
         {
             Console.WriteLine("testCELLSNET_40157 ()");
             string infn = path + @"CELLSNET-40157\template.xlsx";
             string outfn = destpath + @"template.out.xlsx";

             string infn1 = path + @"CELLSNET-40157\template.xls";
             string outfn1 = destpath + @"template.out1.xlsx";


             Workbook wb = new Workbook(infn);
             int iDesign = wb.Worksheets.AddCopy("Designer");
             Worksheet wsDesigner = wb.Worksheets[iDesign];
             wsDesigner.Name = "Copy";
             wb.Save(outfn);
#if WTEST
             Process.Start("explorer.exe", string.Format("\"{0}\"", outfn));
#endif
             wb = new Workbook(infn1);
             wb.Save(outfn1);
#if WTEST
             Process.Start("explorer.exe", string.Format("\"{0}\"", outfn1));
#endif
         }
```

### See Also

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AddCopy(int) {#addcopy}

Adds a worksheet to the collection and copies data from an existed worksheet.

```csharp
public int AddCopy(int sheetIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sheetIndex | Int32 | Index of source worksheet. |

### Return Value

[`Worksheet`](../../worksheet/) object index.

### Examples

```csharp
// Called: int index = workbook.Worksheets.AddCopy(1);
[Test]
        public void Method_Int32_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "TX_-_Tax_Statement.xls");

            int index = workbook.Worksheets.AddCopy(1);
            Worksheet sheet = workbook.Worksheets[index];
            sheet.Shapes[0].Name = "";
            Assert.AreEqual(workbook.Worksheets[1].Shapes[0].Name, "RESWARE_SHEET_SNAPSHOT");
            workbook.Save(Constants.destPath + "Test_163767.xls");
        }
```

### See Also

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AddCopy(Worksheet[], string[]) {#addcopy_2}

Copy a group of worksheets.

```csharp
public void AddCopy(Worksheet[] source, string[] destSheetNames)
```

| Parameter | Type | Description |
| --- | --- | --- |
| source | Worksheet[] | The source worksheets. |
| destSheetNames | String[] | The names of the copied sheets. |

### See Also

* class [Worksheet](../../worksheet/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


