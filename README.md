vue2-ace-editor
====================
A packaging of [ace](https://ace.c9.io/)

Demo here: https://github.com/chairuosen/vue-ace-editor-demo/tree/vue2

## How to use

1. Install

    ```
    npm install --save-dev https://github.com/lh4111/vue2-ace-editor.git
    ```
    
2. Require it in `components` of Vue options

    ```
    import editor from 'vue2-ace-editor'
    
    // import some mode if you need it
    import 'brace/mode/graphqlschema'
    import 'brace/mode/json'
    import 'brace/theme/chrome'
    
    ...
    
    {
        data,
        methods,
        ...
        components: {
            editor,
        },
    }
    ```
    
3. Use the component in template

    ```
    <editor v-model="content" lang="html" theme="chrome" width="500" height="100"></editor>
    ```
    
    prop `v-model`  is required
    
    prop `lang` and `theme` is same as [ace-editor's doc](https://github.com/ajaxorg/ace)
    
    prop `height` and `width` could be one of these:  `200`, `200px`, `50%`
    
