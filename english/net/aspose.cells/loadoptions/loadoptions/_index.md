---
title: LoadOptions.LoadOptions
second_title: Aspose.Cells for .NET API Reference
description: LoadOptions constructor. Creates an options of loading the file
type: docs
url: /net/aspose.cells/loadoptions/loadoptions/
---
## LoadOptions() {#constructor}

Creates an options of loading the file.

```csharp
public LoadOptions()
```

### Examples

```csharp
// Called: var loadOptions = new Aspose.Cells.LoadOptions
private void LoadOptions_Constructor(string filePath, string ticket, string fileName)
        {
           // try
            {
                string newFilename = ticket + &quot;_&quot; + fileName;
                string saveFilePath = Constants.PIVOT_CHECK_FILE_PATH + newFilename;
                filePath = filePath + fileName;

                // 22.6 has 20 members in LoadOptions
                // 19.8 has 17 members in LoadOptions
                var loadOptions = new Aspose.Cells.LoadOptions
                {
                    MemorySetting = MemorySetting.MemoryPreference

                };

                int tryCOunt = 0;

                bool isPasswordProtected = false;
                bool fileOpened = false;

                while (true &amp;&amp; tryCOunt &lt; 3)
                {
                    fileOpened = OpenFileNET51506(loadOptions, filePath, saveFilePath, ref isPasswordProtected);
                    if (!fileOpened)
                    {
                        if (isPasswordProtected)
                        {
                            loadOptions.Password = &quot;sasap&quot;;
                            tryCOunt++;
                        }
                        else
                        {
                            break;
                        }
                    }
                    else
                    {
                        break;
                    }
                }
                if (fileOpened)
                {
                    Console.WriteLine(&quot;File successfully loaded and saved!&quot;);
                }
                else
                {
                    Console.WriteLine(&quot;File could not be loaded!&quot;);
                }
            }
            //catch (Exception ex)
            //{
            //    Console.WriteLine(ex.Message);
            //}
        }
```

### See Also

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## LoadOptions(LoadFormat) {#constructor_1}

Creates an options of loading the file.

```csharp
public LoadOptions(LoadFormat loadFormat)
```

| Parameter | Type | Description |
| --- | --- | --- |
| loadFormat | LoadFormat | The loading format. |

### See Also

* enum [LoadFormat](../../loadformat/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


