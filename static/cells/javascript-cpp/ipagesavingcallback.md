##IPageSavingCallback
ControlIndicate progress of page saving process.
## IPageSavingCallback interface
Control/Indicate progress of page saving process.
## Methods
| Method | Description |
| --- | --- |
| [pageStartSaving(PageStartSavingArgs)](#pageStartSaving-pagestartsavingargs-)| Control/Indicate a page starts to be output. |
| [pageEndSaving(PageEndSavingArgs)](#pageEndSaving-pageendsavingargs-)| Control/Indicate a page ends to be output. |
### pageStartSaving(PageStartSavingArgs) {#pageStartSaving-pagestartsavingargs-}
Control/Indicate a page starts to be output.
```javascript
pageStartSaving(args: PageStartSavingArgs) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| args | [PageStartSavingArgs](../pagestartsavingargs/) | Info for a page starts saving process. |
### pageEndSaving(PageEndSavingArgs) {#pageEndSaving-pageendsavingargs-}
Control/Indicate a page ends to be output.
```javascript
pageEndSaving(args: PageEndSavingArgs) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| args | [PageEndSavingArgs](../pageendsavingargs/) | Info for a page ends saving process. |
