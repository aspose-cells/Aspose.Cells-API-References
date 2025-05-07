---
title: WorkbookSettings.IsEncrypted
second_title: Aspose.Cells for .NET API Reference
description: WorkbookSettings property. Gets a value that indicates whether a password is required to open this workbook
type: docs
url: /net/aspose.cells/workbooksettings/isencrypted/
---
## WorkbookSettings.IsEncrypted property

Gets a value that indicates whether a password is required to open this workbook.

```csharp
public bool IsEncrypted { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(isEncrypted, d.Settings.IsEncrypted);
[Test]
        public void Property_IsEncrypted()
        {
            //CELLSNET-43977,CELLSNET-43980,CELLSNET-43981
            //CELLSNET-43982,CELLSNET-43983

            var di = new DirectoryInfo(Constants.sourcePath + "CellsNet43950");
            var files = di.GetFiles("x*");
            //string f = @"D:\FileTemp\sample_files\xlsx_M.xlsx";
            foreach (var f in files)
            {
                Console.WriteLine(f);

                var d = new Workbook(f.FullName, new LoadOptions() { Password = "1" });
                string s = Path.GetFileNameWithoutExtension(f.FullName);
                int index = s.IndexOf('_');
                string str = s.Substring(index + 1);
                bool isEncrypted = false;
                bool isWriteProtected = false;
                switch (str)
                {
                    case "O":
                        isEncrypted = true;
                        break;
                    case "M":
                        isWriteProtected = true;
                        break;
                    case "OM":
                        isEncrypted = true;
                        isWriteProtected = true;
                        break;
                    default:
                        break;
                }
                
               Assert.AreEqual(isEncrypted, FileFormatUtil.DetectFileFormat(f.FullName).IsEncrypted);

                Assert.AreEqual(isEncrypted, d.Settings.IsEncrypted);
                Assert.AreEqual(isWriteProtected, d.Settings.WriteProtection.IsWriteProtected);
            }
        }
```

### See Also

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


