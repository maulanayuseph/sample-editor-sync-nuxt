<template>
  <div id="app">
    <ejs-documenteditor
      id="container6"
      height="1123px"
      style="width: 100%"
      :service-url="serviceUrl"
      :is-read-only="false"
      :enable-print="true"
      :enable-sfdt-export="true"
      :enable-selection="true"
      :enable-context-menu="true"
      :enable-search="true"
      :enable-options-pane="true"
      :enable-word-export="true"
      :enable-text-export="true"
      :enable-editor="true"
      :enable-image-resizer="true"
      :enable-editor-history="true"
      :enable-hyperlink-dialog="true"
      :enable-table-dialog="true"
      :enable-bookmark-dialog="true"
      :enable-table-of-contents-dialog="true"
      :enable-page-setup-dialog="true"
      :enable-style-dialog="true"
      :enable-list-dialog="true"
      :enable-paragraph-dialog="true"
      :enable-font-dialog="true"
      :enable-table-properties-dialog="true"
      :enable-borders-and-shading-dialog="true"
      :enable-table-options-dialog="true"
    />
  </div>
</template>
<script>
import Vue from 'vue'

import {
  DocumentEditorPlugin,
  Print,
  SfdtExport,
  WordExport,
  TextExport,
  Selection,
  Search,
  Editor,
  ImageResizer,
  EditorHistory,
  ContextMenu,
  OptionsPane,
  HyperlinkDialog,
  TableDialog,
  BookmarkDialog,
  TableOfContentsDialog,
  PageSetupDialog,
  StyleDialog,
  ListDialog,
  ParagraphDialog,
  BulletsAndNumberingDialog,
  FontDialog,
  TablePropertiesDialog,
  BordersAndShadingDialog,
  TableOptionsDialog,
  CellOptionsDialog,
  StylesDialog
} from '@syncfusion/ej2-vue-documenteditor'

Vue.use(DocumentEditorPlugin)

export default {
  provide: {
    DocumentEditor: [
      Print,
      SfdtExport,
      WordExport,
      TextExport,
      Selection,
      Search,
      Editor,
      ImageResizer,
      EditorHistory,
      ContextMenu,
      OptionsPane,
      HyperlinkDialog,
      TableDialog,
      BookmarkDialog,
      TableOfContentsDialog,
      PageSetupDialog,
      StyleDialog,
      ListDialog,
      ParagraphDialog,
      BulletsAndNumberingDialog,
      FontDialog,
      TablePropertiesDialog,
      BordersAndShadingDialog,
      TableOptionsDialog,
      CellOptionsDialog,
      StylesDialog
    ]
  },
  data () {
    return {
      serviceUrl:
        'https://ej2services.syncfusion.com/production/web-services/api/documenteditor/'
    }
  }
}
</script>
<style>
@import "../node_modules/@syncfusion/ej2-vue-documenteditor/styles/material.css";
</style>
