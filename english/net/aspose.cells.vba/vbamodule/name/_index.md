---
title: VbaModule.Name
second_title: Aspose.Cells for .NET API Reference
description: VbaModule property. Gets and sets the name of Module
type: docs
url: /net/aspose.cells.vba/vbamodule/name/
---
## VbaModule.Name property

Gets and sets the name of Module.

```csharp
public string Name { get; set; }
```

### Examples

```csharp
// Called: Worksheet sheet = (Worksheet)table[vbaItem.Name];
[Test]
        public void Property_Name()
        {
            Workbook target = new Workbook(Constants.sourcePath + &quot;CellsNet45588_TargetFile.xlsx&quot;);
            Workbook templateFile = new Workbook(Constants.sourcePath + &quot;CellsNet45588_TemplateFileToImport.xlsm&quot;);
            Hashtable table = new Hashtable();
            foreach (Worksheet ws in templateFile.Worksheets)
            {
                if (ws.Type == SheetType.Worksheet)
                {
                     Worksheet s = target.Worksheets.Add(ws.Name);
                    s.Copy(ws);
                    table.Add(ws.CodeName, s);
                }
            }


            foreach (VbaModule vbaItem in templateFile.VbaProject.Modules)
            {
                if (vbaItem.Name == &quot;ThisWorkbook&quot;)
                {
                    target.VbaProject.Modules[&quot;ThisWorkbook&quot;].Codes = vbaItem.Codes;
                }
                else
                {
                    int vbaMod = 0;
                    Worksheet sheet = (Worksheet)table[vbaItem.Name];
                    if (sheet == null)
                        vbaMod = target.VbaProject.Modules.Add(vbaItem.Type, vbaItem.Name);
                    else
                        vbaMod = target.VbaProject.Modules.Add(sheet);
               

                    target.VbaProject.Modules[vbaMod].Codes = vbaItem.Codes;
                    if (vbaItem.Type == VbaModuleType.Designer)
                    {
                        target.VbaProject.Modules.AddDesignerStorage(vbaItem.Name,
                            templateFile.VbaProject.Modules.GetDesignerStorage(vbaItem.Name));
                    }
                }
               
            }
            target.Save(Constants.destPath + &quot;CellsNet45588.xlsm&quot;);
         

     


        }
```

### See Also

* class [VbaModule](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


