---
layout: docs
title: Table Copy Rows
description: Table Copy Rows extension of Bootstrap Table.
group: extensions
toc: true
---

This extension adds functionality for copying selected rows to the clipboard. Currently works on all desktop browsers except safari.

## Usage

{% highlight html %}
<script src="extensions/copy-rows/bootstrap-table-copy-rows.js"></script>
{% endhighlight %}

## Example

[Copy Rows](https://examples.bootstrap-table.com/#extensions/copy-rows.html)

## Options

### showCopyRows

- **Attribute:** `data-show-copy-rows`

- **type:** `Boolean`

- **Detail:**

  Set `true` to show the copy button. This button copy the contents of the selected rows to the clipboard.

- **Default:** `false`

### copyDelimiter

- **Attribute:** `data-copy-delimiter`

- **type:** `String`

- **Detail:**

   This delimiter will be inserted in-between the column values when copying.

- **Default:** `', '`

### copyNewline

- **Attribute:** `data-copy-newline`

- **type:** `String`

- **Detail:**

  This newline will be inserted in between the row values when copying.

- **Default:** `'\n'`

### copyWithHidden

- **Attribute:** `data-copy-with-hidden`

- **type:** `Boolean`

- **Detail:**

  Set `true` to copy with hidden columns.

- **Default:** `false`

### copyRowsHandler

- **Attribute:** `data-copy-rows-handler

- **type:** `Function`

- **Detail:**

  Before copying rows, handle the copying rows data. The parameters object contains:

  * `text`: the copy rows data.

- **Default:** `function(text) { return text }`

## Column options

### ignoreCopy

- **Attribute:** `data-ignore-copy`

- **type:** `Boolean`

- **Detail:**

  Set `true` to ignore this column while copying.

- **Default:** `false`

### rawCopy

- **Attribute:** `data-raw-copy`

- **type:** `Boolean`

- **Detail:**

  Set `true` to copy the raw value instead the formatted one.
  If no formatter is used, this option has no effect.

- **Default:** `false`

## Icons

- copy: 'fa-copy'

## Methods

### copyColumnsToClipboard

* Copy the contents of the selected rows to the clipboard.

## Localizations

### formatCopyRows

- **type:** `Function`

- **Default:** `function () { return "Copy Rows" }`
