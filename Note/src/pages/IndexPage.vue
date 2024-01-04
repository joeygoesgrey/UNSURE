<template>
  <div ref="editor">
    <form autocorrect="off" autocapitalize="off" autocomplete="off" spellcheck="false" class="">
      <q-editor v-model="qeditor" :dense="$q.screen.lt.md" @paste="evt => pasteCapture(evt)" height="100vh"
        @drop="evt => dropCapture(evt)" :definitions="{
          save: {
            tip: 'Save your work',
            icon: 'save',
            label: 'Save',
            handler: saveWork
          },
          upload: {
            tip: 'Upload to cloud',
            icon: 'cloud_upload',
            label: 'Upload',
            handler: uploadIt
          }
        }" :toolbar="[
  [
    {
      label: $q.lang.editor.align,
      icon: $q.iconSet.editor.align,
      fixedLabel: true,
      list: 'only-icons',
      options: ['left', 'center', 'right', 'justify']
    },
    {
      label: $q.lang.editor.align,
      icon: $q.iconSet.editor.align,
      fixedLabel: true,
      options: ['left', 'center', 'right', 'justify']
    }
  ],
  ['bold', 'italic', 'strike', 'underline', 'subscript', 'superscript'],
  ['token', 'hr', 'link', 'custom_btn'],
  ['print', 'fullscreen'],
  ['upload', 'save'],
  [
    {
      label: $q.lang.editor.formatting,
      icon: $q.iconSet.editor.formatting,
      list: 'no-icons',
      options: [
        'p',
        'h1',
        'h2',
        'h3',
        'h4',
        'h5',
        'h6',
        'code'
      ]
    },
    {
      label: $q.lang.editor.fontSize,
      icon: $q.iconSet.editor.fontSize,
      fixedLabel: true,
      fixedIcon: true,
      list: 'no-icons',
      options: [
        'size-1',
        'size-2',
        'size-3',
        'size-4',
        'size-5',
        'size-6',
        'size-7'
      ]
    },
    {
      label: $q.lang.editor.defaultFont,
      icon: $q.iconSet.editor.font,
      fixedIcon: true,
      list: 'no-icons',
      options: [
        'default_font',
        'arial',
        'arial_black',
        'comic_sans',
        'courier_new',
        'impact',
        'lucida_grande',
        'times_new_roman',
        'verdana'
      ]
    },
    'removeFormat'
  ],
  ['quote', 'unordered', 'ordered', 'outdent', 'indent'],

  ['undo', 'redo'],
  ['viewsource']
]" :fonts="{
  arial: 'Arial',
  arial_black: 'Arial Black',
  comic_sans: 'Comic Sans MS',
  courier_new: 'Courier New',
  impact: 'Impact',
  lucida_grande: 'Lucida Grande',
  times_new_roman: 'Times New Roman',
  verdana: 'Verdana'
}" />
    </form>
  </div>
</template>

<script>
import EditorJS from '@editorjs/editorjs';
// import Header from '@editorjs/header'; // Importing the Header tool
// import List from '@editorjs/list';
// import CheckList from '@editorjs/checklist';
// import Quote from '@editorjs/quote';
// import Marker from '@editorjs/marker';
// import Delimiter from '@editorjs/delimiter';


import { defineComponent, ref } from 'vue';

export default defineComponent({
  mounted() {
    this.editor = new EditorJS({
      holder: this.$refs.editor,

      // Editor.js configuration
      tools: {
        // header: Header, // For headers
        // list: List, // For lists
        // checklist: CheckList, // For checklists
        // quote: Quote, // For blockquotes
        // marker: Marker, // For highlighting text
        // delimiter: Delimiter, // For visual breaks in content
        // inlineCode: InlineCode, // For inline code snippets
        // image: SimpleImage, // For images
        // ...add other tools as needed
      },

      // Initial data to load into the editor
      // data: {
      //   // Your data here
      // },



      // Callbacks for handling events
      // onReady: () => {
      //   console.log('Editor.js is ready to work!');
      // },
      // onChange: () => {
      //   console.log('Now I know that Editor\'s content changed!');
      // } 
    });
  },
  beforeUnmount() {
    this.editor.destroy();
  },
  setup() {
    return {
      qeditor: ref(
        '<pre>Check out the two different types of dropdowns' +
        ' in each of the "Align" buttons.</pre> '
      )
    }
  }
});
</script>
 
