##LowCodeSaveOptionsProviderOfPlaceHolders
Implementation to provide save options which save split parts to files and the path of resultant file are defined with placeholders.
**Inheritance:**
java.lang.Object, [com.aspose.cells.AbstractLowCodeSaveOptionsProvider](../../com.aspose.cells/abstractlowcodesaveoptionsprovider)
```
public class LowCodeSaveOptionsProviderOfPlaceHolders extends AbstractLowCodeSaveOptionsProvider
```
Implementation to provide save options which save split parts to files and the path of resultant file are defined with placeholders.
## Constructors
| Constructor | Description |
| --- | --- |
| [LowCodeSaveOptionsProviderOfPlaceHolders(String pathTemplate)](#LowCodeSaveOptionsProviderOfPlaceHolders-java.lang.String-) | Instantiates an instance to provide save options according to specified templates. |
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [finish(LowCodeSaveOptions part)](#finish-com.aspose.cells.LowCodeSaveOptions-) | Releases resources after processing currently split part. |
| [getBuildPathWithSheetAlways()](#getBuildPathWithSheetAlways--) | Whether add sheet index or name to file path always. |
| [getBuildPathWithSplitPartAlways()](#getBuildPathWithSplitPartAlways--) | Whether add split part index to file path always. |
| [getClass()](#getClass--) |  |
| [getSaveOptions(SplitPartInfo part)](#getSaveOptions-com.aspose.cells.SplitPartInfo-) | Gets the save options from which to get the output settings for currently split part. |
| [getSaveOptionsTemplate()](#getSaveOptionsTemplate--) | The template for creating instance of save options in [AbstractLowCodeSaveOptionsProvider.getSaveOptions(SplitPartInfo)](../../com.aspose.cells/abstractlowcodesaveoptionsprovider\#getSaveOptions-SplitPartInfo-). |
| [getSheetIndexOffset()](#getSheetIndexOffset--) | Offset of sheet's index between what used in file path and its actual value([SplitPartInfo.getSheetIndex()](../../com.aspose.cells/splitpartinfo\#getSheetIndex--)). |
| [getSheetIndexPrefix()](#getSheetIndexPrefix--) | Prefix for the index of worksheet. |
| [getSheetNamePrefix()](#getSheetNamePrefix--) | Prefix for the index of worksheet. |
| [getSplitPartIndexOffset()](#getSplitPartIndexOffset--) | Offset of split part's index between what used in file path and its actual value([SplitPartInfo.getPartIndex()](../../com.aspose.cells/splitpartinfo\#getPartIndex--)). |
| [getSplitPartPrefix()](#getSplitPartPrefix--) | Prefix for the index of split part. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBuildPathWithSheetAlways(boolean value)](#setBuildPathWithSheetAlways-boolean-) | Whether add sheet index or name to file path always. |
| [setBuildPathWithSplitPartAlways(boolean value)](#setBuildPathWithSplitPartAlways-boolean-) | Whether add split part index to file path always. |
| [setSaveOptionsTemplate(LowCodeSaveOptions value)](#setSaveOptionsTemplate-com.aspose.cells.LowCodeSaveOptions-) | The template for creating instance of save options in [AbstractLowCodeSaveOptionsProvider.getSaveOptions(SplitPartInfo)](../../com.aspose.cells/abstractlowcodesaveoptionsprovider\#getSaveOptions-SplitPartInfo-). |
| [setSheetIndexOffset(int value)](#setSheetIndexOffset-int-) | Offset of sheet's index between what used in file path and its actual value([SplitPartInfo.getSheetIndex()](../../com.aspose.cells/splitpartinfo\#getSheetIndex--)). |
| [setSheetIndexPrefix(String value)](#setSheetIndexPrefix-java.lang.String-) | Prefix for the index of worksheet. |
| [setSheetNamePrefix(String value)](#setSheetNamePrefix-java.lang.String-) | Prefix for the index of worksheet. |
| [setSplitPartIndexOffset(int value)](#setSplitPartIndexOffset-int-) | Offset of split part's index between what used in file path and its actual value([SplitPartInfo.getPartIndex()](../../com.aspose.cells/splitpartinfo\#getPartIndex--)). |
| [setSplitPartPrefix(String value)](#setSplitPartPrefix-java.lang.String-) | Prefix for the index of split part. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### LowCodeSaveOptionsProviderOfPlaceHolders(String pathTemplate) {#LowCodeSaveOptionsProviderOfPlaceHolders-java.lang.String-}
```
public LowCodeSaveOptionsProviderOfPlaceHolders(String pathTemplate)
```
Instantiates an instance to provide save options according to specified templates.
**Remarks**
The supported placeholders in file path template:
*  $\{SheetIndex\}: will be replaced by the sheet index of the split part
*  $\{SheetName\}: will be replaced by the sheet name of the split part
*  $\{SplitPartIndex\}: will be replaced by the index of the split part
*  $\{SheetIndexPrefix\}: will be replaced by
*  $\{SheetNamePrefix\}: will be replaced by
*  $\{SplitPartPrefix\}: will be replaced by
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pathTemplate | java.lang.String | The template of the resultant file path. |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | java.lang.Object |  |
**Returns:**
boolean
### finish(LowCodeSaveOptions part) {#finish-com.aspose.cells.LowCodeSaveOptions-}
```
public void finish(LowCodeSaveOptions part)
```
Releases resources after processing currently split part.
**Remarks**
By default this method just closes the stream specified by the [LowCodeSaveOptions.getOutputStream()](../../com.aspose.cells/lowcodesaveoptions\#getOutputStream--) directly(if the save options specified a Stream as destination). User may overwrite this method to control how to release resources according to their requirement and the implementation of [getSaveOptions(SplitPartInfo)](../../com.aspose.cells/abstractlowcodesaveoptionsprovider\#getSaveOptions-SplitPartInfo-).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| part | [LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions) | the save options used for currently split part. |
### getBuildPathWithSheetAlways() {#getBuildPathWithSheetAlways--}
```
public boolean getBuildPathWithSheetAlways()
```
Whether add sheet index or name to file path always. Default value is false, that is, when there is only one sheet, the sheet index and name and corresponding prefix([getSheetNamePrefix()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getSheetNamePrefix--)) will not be added to the file path.
**Returns:**
boolean
### getBuildPathWithSplitPartAlways() {#getBuildPathWithSplitPartAlways--}
```
public boolean getBuildPathWithSplitPartAlways()
```
Whether add split part index to file path always. Default value is false, that is, when there is only one split part, the split part index and corresponding prefix([LowCodeSaveOptionsProviderOfAssembling.getSplitPartPrefix()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getSplitPartPrefix--)) will not be added to the file path.
**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getSaveOptions(SplitPartInfo part) {#getSaveOptions-com.aspose.cells.SplitPartInfo-}
```
public LowCodeSaveOptions getSaveOptions(SplitPartInfo part)
```
Gets the save options from which to get the output settings for currently split part.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| part | [SplitPartInfo](../../com.aspose.cells/splitpartinfo) |  |
**Returns:**
[LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions)
### getSaveOptionsTemplate() {#getSaveOptionsTemplate--}
```
public LowCodeSaveOptions getSaveOptionsTemplate()
```
The template for creating instance of save options in [AbstractLowCodeSaveOptionsProvider.getSaveOptions(SplitPartInfo)](../../com.aspose.cells/abstractlowcodesaveoptionsprovider\#getSaveOptions-SplitPartInfo-).
**Remarks**
If the template has been specified, then the created instance will copy all setting from it and update the output file accordingly.
**Returns:**
[LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions)
### getSheetIndexOffset() {#getSheetIndexOffset--}
```
public int getSheetIndexOffset()
```
Offset of sheet's index between what used in file path and its actual value([SplitPartInfo.getSheetIndex()](../../com.aspose.cells/splitpartinfo\#getSheetIndex--)).
**Returns:**
int
### getSheetIndexPrefix() {#getSheetIndexPrefix--}
```
public String getSheetIndexPrefix()
```
Prefix for the index of worksheet.
**Remarks**
If there is only one worksheet and [LowCodeSaveOptionsProviderOfAssembling.getBuildPathWithSheetAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getBuildPathWithSheetAlways--) is false, then this prefix and the sheet index(or name) will not be added to the resultant file path.
**Returns:**
java.lang.String
### getSheetNamePrefix() {#getSheetNamePrefix--}
```
public String getSheetNamePrefix()
```
Prefix for the index of worksheet.
**Remarks**
If there is only one worksheet and [LowCodeSaveOptionsProviderOfAssembling.getBuildPathWithSheetAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getBuildPathWithSheetAlways--) is false, then this prefix and the sheet index(or name) will not be added to the resultant file path.
**Returns:**
java.lang.String
### getSplitPartIndexOffset() {#getSplitPartIndexOffset--}
```
public int getSplitPartIndexOffset()
```
Offset of split part's index between what used in file path and its actual value([SplitPartInfo.getPartIndex()](../../com.aspose.cells/splitpartinfo\#getPartIndex--)).
**Returns:**
int
### getSplitPartPrefix() {#getSplitPartPrefix--}
```
public String getSplitPartPrefix()
```
Prefix for the index of split part.
**Remarks**
If there is only one split part and [LowCodeSaveOptionsProviderOfAssembling.getBuildPathWithSplitPartAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getBuildPathWithSplitPartAlways--) is false, then this prefix and the split part index(0) will not be added to the resultant file path.
**Returns:**
java.lang.String
### hashCode() {#hashCode--}
```
public native int hashCode()
```
**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```
### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```
### setBuildPathWithSheetAlways(boolean value) {#setBuildPathWithSheetAlways-boolean-}
```
public void setBuildPathWithSheetAlways(boolean value)
```
Whether add sheet index or name to file path always. Default value is false, that is, when there is only one sheet, the sheet index and name and corresponding prefix([getSheetNamePrefix()](../../com.aspose.cells/lowcodesaveoptionsproviderofplaceholders\#getSheetNamePrefix--)) will not be added to the file path.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setBuildPathWithSplitPartAlways(boolean value) {#setBuildPathWithSplitPartAlways-boolean-}
```
public void setBuildPathWithSplitPartAlways(boolean value)
```
Whether add split part index to file path always. Default value is false, that is, when there is only one split part, the split part index and corresponding prefix([LowCodeSaveOptionsProviderOfAssembling.getSplitPartPrefix()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getSplitPartPrefix--)) will not be added to the file path.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setSaveOptionsTemplate(LowCodeSaveOptions value) {#setSaveOptionsTemplate-com.aspose.cells.LowCodeSaveOptions-}
```
public void setSaveOptionsTemplate(LowCodeSaveOptions value)
```
The template for creating instance of save options in [AbstractLowCodeSaveOptionsProvider.getSaveOptions(SplitPartInfo)](../../com.aspose.cells/abstractlowcodesaveoptionsprovider\#getSaveOptions-SplitPartInfo-).
**Remarks**
If the template has been specified, then the created instance will copy all setting from it and update the output file accordingly.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [LowCodeSaveOptions](../../com.aspose.cells/lowcodesaveoptions) |  |
### setSheetIndexOffset(int value) {#setSheetIndexOffset-int-}
```
public void setSheetIndexOffset(int value)
```
Offset of sheet's index between what used in file path and its actual value([SplitPartInfo.getSheetIndex()](../../com.aspose.cells/splitpartinfo\#getSheetIndex--)).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setSheetIndexPrefix(String value) {#setSheetIndexPrefix-java.lang.String-}
```
public void setSheetIndexPrefix(String value)
```
Prefix for the index of worksheet.
**Remarks**
If there is only one worksheet and [LowCodeSaveOptionsProviderOfAssembling.getBuildPathWithSheetAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getBuildPathWithSheetAlways--) is false, then this prefix and the sheet index(or name) will not be added to the resultant file path.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setSheetNamePrefix(String value) {#setSheetNamePrefix-java.lang.String-}
```
public void setSheetNamePrefix(String value)
```
Prefix for the index of worksheet.
**Remarks**
If there is only one worksheet and [LowCodeSaveOptionsProviderOfAssembling.getBuildPathWithSheetAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getBuildPathWithSheetAlways--) is false, then this prefix and the sheet index(or name) will not be added to the resultant file path.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setSplitPartIndexOffset(int value) {#setSplitPartIndexOffset-int-}
```
public void setSplitPartIndexOffset(int value)
```
Offset of split part's index between what used in file path and its actual value([SplitPartInfo.getPartIndex()](../../com.aspose.cells/splitpartinfo\#getPartIndex--)).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setSplitPartPrefix(String value) {#setSplitPartPrefix-java.lang.String-}
```
public void setSplitPartPrefix(String value)
```
Prefix for the index of split part.
**Remarks**
If there is only one split part and [LowCodeSaveOptionsProviderOfAssembling.getBuildPathWithSplitPartAlways()](../../com.aspose.cells/lowcodesaveoptionsproviderofassembling\#getBuildPathWithSplitPartAlways--) is false, then this prefix and the split part index(0) will not be added to the resultant file path.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### toString() {#toString--}
```
public String toString()
```
**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```
### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |
