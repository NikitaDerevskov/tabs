# tabtabtab

Make tabs easily in your html.

> Tab is a part that sticks out of something and that you can pull in order to make something happen  
> see https://www.macmillandictionary.com/dictionary/british/tab_1?q=tabs  

## JS only

This package does not contain neither styles nor html. Everyone is supposed to write their own styles and markup.

When tab is clicked, it becomes active. That means:
1. Active tab is marked with `active` class
2. According block with content is shown

## Flexible

There are no assumptions about your html. Tab buttons could be placed anywhere, and could be presented as any type of html element.

## Usage

There are two things to specify:
1. Mapping from the tab tip to it's content
2. Which tab is active by default

#### JavaScript
```js 
tabs([
  {tab: '#tab1', content: '#content1'},
  {tab: '#tab2', content: '#content2'},
  {tab: '#tab3', content: '#content3'},
], {active: '#tab2'})
```

#### HTML
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title></title>
</head>
<body>

  <main>
    <div class="tabs">
      <ul>
        <li id="tab1"></li>
        <li id="tab2"></li>
        <li id="tab3"></li>
      </ul>
      <div id="content1"></div>
      <div id="content2"></div>
      <div id="content3"></div>
    </div>
  </main>

</body>
</html>

```

## ToDo: Now

    - [ ] rename repo according to the title
    - [ ] example project in a separate directory
    - [ ] example project: test

## To Do: Some Day

    - [ ] custom styles for content 
    - [ ] short syntax support `tabs({}, {active: '#tab2'})`
