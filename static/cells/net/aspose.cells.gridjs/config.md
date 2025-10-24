##Class Config
Aspose.Cells.GridJs.Config class. Represents all the static settings for GridJs
## Config class
Represents all the static settings for GridJs
```csharp
public class Config
```
## Constructors
| Name | Description |
| --- | --- |
| [Config](config/)() | The default constructor. |
## Properties
| Name | Description |
| --- | --- |
| static [AutoOptimizeForLargeCells](../../aspose.cells.gridjs/config/autooptimizeforlargecells/) { get; set; } | Gets/Sets whether to automatically optimize the load performance for worksheet with large cells. it will ignore some style /borders to reduce the load time. the default value is true. |
| static [BaseRouteName](../../aspose.cells.gridjs/config/baseroutename/) { get; set; } | Gets/Sets the base route name for GridJs controller URL. the default is "/GridJs2". |
| static [CustomPdfSaveOptions](../../aspose.cells.gridjs/config/custompdfsaveoptions/) { get; set; } | Gets/Sets the custom PdfSaveOptions for PDF export. If set, this will be used instead of the default options. the default value is null. |
| static [EmptySheetMaxCol](../../aspose.cells.gridjs/config/emptysheetmaxcol/) { get; set; } | Gets/Sets default max column for an empty worksheet. the default value is 15. |
| static [EmptySheetMaxRow](../../aspose.cells.gridjs/config/emptysheetmaxrow/) { get; set; } | Gets/Sets default max row for an empty worksheet. the default value is 12. |
| static [FileCacheDirectory](../../aspose.cells.gridjs/config/filecachedirectory/) { get; set; } | Gets/Sets the cache directory for storing spreadsheet file. We need to set it to a specific path before we use GridJs. |
| static [IgnoreEmptyContent](../../aspose.cells.gridjs/config/ignoreemptycontent/) { get; set; } | Gets/Sets whether to show the max range which includes data ,style, merged cells and shapes. if the last row or column contains cells with no value and formula but has custom style then we will not show this row/column when this vlaue is true。 the default value is true . |
| static [IsCollaborative](../../aspose.cells.gridjs/config/iscollaborative/) { get; set; } | Gets/Sets whether to support collabrative editing,the default is false. |
| static [IslimitShapeOrImage](../../aspose.cells.gridjs/config/islimitshapeorimage/) { get; set; } | Gets/Sets whether to limit the total display shape/image count in one worksheet ,if set to true, GridJs will limit the total count of the display shapes or images in one worksheet to MaxShapeOrImageCount the default value is true. |
| static [LazyLoading](../../aspose.cells.gridjs/config/lazyloading/) { get; set; } | Gets/Sets whether to load active worksheet only,the default is false. |
| static [MaxPdfSaveSeconds](../../aspose.cells.gridjs/config/maxpdfsaveseconds/) { get; set; } | Gets/Sets the max timed out seconds when save to PDF. the default value is 10. |
| static [MaxShapeOrImageCount](../../aspose.cells.gridjs/config/maxshapeorimagecount/) { get; set; } | Gets/Sets the total count of the display shapes or images in the active sheet,it takes effect when IslimitShapeOrImage=true. the default value is 100. |
| static [MaxShapeOrImageWidthOrHeight](../../aspose.cells.gridjs/config/maxshapeorimagewidthorheight/) { get; set; } | Gets/Sets the max width or height for a shape or an image ,GridJs will ignore the shape or image with the width or height larger than this, it takes effect when IslimitShapeOrImage=true. the default value is 10000. |
| static [MaxTotalShapeOrImageCount](../../aspose.cells.gridjs/config/maxtotalshapeorimagecount/) { get; set; } | Gets/Sets the total count of the display shapes or images in the workbook,it takes effect when IslimitShapeOrImage=true. the default value is 300. |
| static [MessageTopic](../../aspose.cells.gridjs/config/messagetopic/) { get; set; } | Gets/Sets the websocket destinations prefixed with "/topic". the default is "/topic/opr".used in collaborative mode only. |
| static [PictureCacheDirectory](../../aspose.cells.gridjs/config/picturecachedirectory/) { get; set; } | Gets/Sets the cache directory for pictures.(this takes effect when GridJsWorkbook.CacheImp is null) the default path will be "_piccache" inside the FileCacheDirectory. |
| static [SameImageDetecting](../../aspose.cells.gridjs/config/sameimagedetecting/) { get; set; } | Gets/Sets whether to check if images have same source,the default is true the default value is true. |
| static [SaveHtmlAsZip](../../aspose.cells.gridjs/config/savehtmlaszip/) { get; set; } | Gets/Sets whether to save html file as zip archive,the default is false. |
| static [ShowChartSheet](../../aspose.cells.gridjs/config/showchartsheet/) { get; set; } | Gets/Sets whether to show chart worksheet. the default value is false . |
| static [SkipInvisibleShapes](../../aspose.cells.gridjs/config/skipinvisibleshapes/) { get; set; } | Gets/Sets whether to skip shapes that are invisble to UI ,the default value is true. |
| static [UsePrintArea](../../aspose.cells.gridjs/config/useprintarea/) { get; set; } | Gets/Sets whether to use PageSetup.PrintArea for the UI display range when the worksheet has PageSetup setting for PrintArea. the default value is false . |
## Methods
| Name | Description |
| --- | --- |
| static [SetFontFolder](../../aspose.cells.gridjs/config/setfontfolder/)(string, bool) | Sets the fonts folder |
| static [SetFontFolders](../../aspose.cells.gridjs/config/setfontfolders/)(string[], bool) | Sets the fonts folders |
### See Also
* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)
