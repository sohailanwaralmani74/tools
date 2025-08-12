---
layout: default
title: Convert JSON To SQL Offline Free
description: Converter and metadata scrubber, Along with png to jpeg, wav to mp3, Recet Image & Much more;
keywords: 
---
<script src="https://cdn.jsdelivr.net/npm/sql-formatter@12.2.0/dist/sql-formatter.min.js"></script>
<script src="https://code.jquery.com/jquery-3.6.0.min.js"></script>
<script src="https://cdn.jsdelivr.net/npm/jsonview@1.2.0/dist/jquery.jsonview.min.js"></script>
<link href="https://cdn.jsdelivr.net/npm/jsonview@1.2.0/dist/jquery.jsonview.min.css" rel="stylesheet">



<h1>Convert JSON To SQL | Preview, Edit And Export To SQL</h1>
<!-- Tool section -->
<section class="tool-section container">
    <div class="upload-section">
        <label for="json-file" class="upload-label">Upload JSON File</label>
        <input type="file" id="json-file" accept=".json">
    </div>

<div id="loader" style="display:none;">⏳ Loading file...</div>
    <div style="width: 99%; justify-content: flex-end; margin-top: 1rem; position: sticky; display:none;"
        id="exportOptions">
        <label class="export-label" onclick="convertToSQL()"><u>Convert JSON To SQL</u></label>
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
 <label class="export-label" onclick="exportToSQL()"><u> Export To SQL</u></label>
 <label class="export-label" onclick="showJson()"><u>Show JSON</u></label>
</div>
   <textarea id="sql-viewer" placeholder="Data Will Be Displayed Here" style="display:none; width: 98%; margin-left: 1rem; height: 68vh;"></textarea>

<script src="/assets/js/json-to-sql.js"></script>

