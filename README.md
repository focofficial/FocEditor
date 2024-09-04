# FocEditor

FocEditor 是一个基于 Vue.js 的富文本编辑器组件，旨在为你的项目提供一个功能丰富且易于集成的编辑器。该组件提供了类似于 TinyMCE 的编辑功能，支持各种富文本操作，适用于各种应用场景。

## 特性

- **易于集成**：支持通过 CDN 直接引用，无需复杂配置。
- **自定义配置**：允许自定义工具栏和样式。
- **丰富功能**：支持多种文本格式、图片插入等功能。

## 安装

### 通过 CDN 引用

你可以通过 GitHub Pages 提供的 CDN URL 来引用 FocEditor 组件。只需在你的 HTML 文件中添加以下标签：

```html
<link rel="stylesheet" href="https://github.com/focofficial/FocEditor/dist/foc-editor.css">
<script src="https://github.com/focofficial/FocEditor/foc-editor.js"></script>
```
#### 请将 <YOUR_USERNAME> 和 <YOUR_REPOSITORY> 替换为你的 GitHub 用户名和仓库名。

### 在 Vue 项目中使用
如果你希望在 Vue 项目中使用 FocEditor，可以通过以下步骤进行集成：

#### 1.安装组件：
`npm install --save git+https://github.com/focofficial/FocEditor`

#### 2.在 Vue 组件中引入：
在你的 Vue 组件中，按照以下方式引入并注册 FocEditor：
```vue
<template>
  <div>
    <foc-editor v-model="editorContent"></foc-editor>
  </div>
</template>

<script>
import FocEditor from 'foceditor';

export default {
  components: {
    FocEditor
  },
  data() {
    return {
      editorContent: ''
    };
  }
};
</script>

<style>
@import '~foceditor/dist/foc-editor.css';
</style>
```
#### 3.使用组件：

你可以在模板中使用 <foc-editor> 标签来引入编辑器，并使用 v-model 绑定数据。

### 使用说明

1. **在 HTML 文件中引用**：如果你通过 CDN 提供静态文件，只需在 HTML 中引入 CSS 和 JS 文件。
2. **在 Vue 项目中安装**：如果你通过 npm 安装，可以按照示例代码在 Vue 组件中引入并使用。
