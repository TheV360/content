---
title: "FileSystemDirectoryHandle: entries() method"
short-title: entries()
slug: Web/API/FileSystemDirectoryHandle/entries
page-type: web-api-instance-method
browser-compat: api.FileSystemDirectoryHandle.entries
---

{{securecontext_header}}{{APIRef("File System API")}}

The **`entries()`** method of the
{{domxref("FileSystemDirectoryHandle")}} interface returns a new asynchronous iterator
for the iteration of the key-value pairs of the entries within the `FileSystemDirectoryHandle`
on which this method is called. The key-value pairs are
in the form of an array like `[key, value]`.

## Syntax

```js-nolint
entries()
```

### Parameters

None.

### Return value

A new asynchronous iterator containing the key-value pairs of each entry within the `FileSystemDirectoryHandle`.

## Examples

Use the `for await...of` loop can simplify the iteration process.

```js
const dirHandle = await window.showDirectoryPicker();

for await (const [key, value] of dirHandle.entries()) {
  console.log({ key, value });
}
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- [File System API](/en-US/docs/Web/API/File_System_API)
- [The File System Access API: simplifying access to local files](https://developer.chrome.com/articles/file-system-access/)
