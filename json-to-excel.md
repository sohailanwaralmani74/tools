---
layout: default
title: Convert JSON To Excel Offline Free
description: Converter and metadata scrubber, Along with png to jpeg, wav to mp3, Recet Image & Much more;
keywords: 
---

<script src="https://code.jquery.com/jquery-3.6.0.min.js"></script>
<script src="https://cdn.jsdelivr.net/npm/jsonview@1.2.0/dist/jquery.jsonview.min.js"></script>
<link href="https://cdn.jsdelivr.net/npm/jsonview@1.2.0/dist/jquery.jsonview.min.css" rel="stylesheet">

<script src="https://cdnjs.cloudflare.com/ajax/libs/xlsx/0.18.5/xlsx.full.min.js"></script>


<h1>Convert JSON To Excel | Preview, Edit And Export To Excel</h1>
<!-- Tool section -->
<section class="tool-section container">
    <div class="upload-section">
        <label for="json-file" class="upload-label">Upload JSON File</label>
        <input type="file" id="json-file" accept=".json">
    </div>

<div id="loader" style="display:none;">⏳ Loading file...</div>
    <div style="width: 99%; justify-content: flex-end; margin-top: 1rem; position: sticky; display:none;"
        id="exportOptions">
        <label class="export-label" onclick="convertJSONToExcel()"><u>Convert JSON To Excel</u></label>
    </div>
</section>
<div id="json-tool-wrapper">
  <div id="json-editor-container">
   <textarea id="json-editor" placeholder="Paste your JSON here... or upload file"></textarea>
  </div>
  <div id="json-viewer-container" style="display: flex; justify-content:start;">
   <div id="json-tree-viewer" style="display: flex; justify-content:start;"></div>
  </div>
</div>
<div style="min-width: 100%; display:none; justify-content: flex-end; margin-top: 1rem; margin-bottom: 1rem;" id="exportButtons">
 <label>You can edit below excel file. Just click cell and edit</label>
 <label class="export-label" onclick="exportToXLSX()"><u> Export To XLSX</u></label>
 <label class="export-label" onclick="exportToXLS()"><u>Export To XLS</u></label>
 <label class="export-label" onclick="showJson()"><u>Show JSON</u></label>
</div>
<div id="table-container" style="  max-height: 70vh; overflow: auto; margin: 1rem;" contenteditable></div>

<script src="/assets/js/json-to-excel.js"></script>

