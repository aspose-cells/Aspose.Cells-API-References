---
title: Worksheet.CodeName
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Gets worksheet code name
type: docs
url: /net/aspose.cells/worksheet/codename/
---
## Worksheet.CodeName property

Gets worksheet code name.

```csharp
public string CodeName { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual("Sheet1", workbook.Worksheets[0].CodeName);
public void Worksheet_Property_CodeName()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsm");
    Console.WriteLine("Before Deleting Sheet & Module: " + "workbook.Worksheets.Count: " + workbook.Worksheets.Count.ToString() + "workbook.VbaProject.Modules.Count: " + workbook.VbaProject.Modules.Count.ToString());
    workbook.Worksheets.RemoveAt(workbook.Worksheets.Count - 1);
    workbook.VbaProject.Modules.RemoveAt(workbook.VbaProject.Modules.Count - 1);
    Console.WriteLine("After Deleting Sheet & Module: " + "workbook.Worksheets.Count: " + workbook.Worksheets.Count.ToString() + "workbook.VbaProject.Modules.Count: " + workbook.VbaProject.Modules.Count.ToString());

    Console.WriteLine("Before Adding Sheet & Module: " + "workbook.Worksheets.Count: " + workbook.Worksheets.Count.ToString() + "workbook.VbaProject.Modules.Count: " + workbook.VbaProject.Modules.Count.ToString());
    workbook.VbaProject.Modules.Add(workbook.Worksheets.Add("TestSheet"));
    Console.WriteLine("After Adding Sheet & Module: " + "workbook.Worksheets.Count: " + workbook.Worksheets.Count.ToString() + "workbook.VbaProject.Modules.Count: " + workbook.VbaProject.Modules.Count.ToString());
    for (int i = 0; i <= workbook.VbaProject.Modules.Count - 1; i++)
    {
        workbook.VbaProject.Modules[i].Codes += " '" + i.ToString() + " ";
    }
    workbook.Save(Constants.destPath + "example.xlsm");
    workbook = new Workbook(Constants.destPath + "example.xlsm");
    Assert.AreEqual("Sheet1", workbook.Worksheets[0].CodeName);
}
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


