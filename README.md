# Code Refactor HTML project

## Technologies Used

- HTML
- CSS
- VS Code
- Git
- GitHub

## Summary

This project was used to teach myself about semantic HTML tags and how to properly use them. Much of the starting code was using non-semantic tag such as div, so switching those to tags such as header, footer, section, aside, and article make the code far more readable for a developer. Along with the tag changes, I had to change those tags in the CSS style sheet so the selectors would match up with the tags in HTML. Along with changing these tags, I ensured that all images had alt texts for screen readers as well as consolidated code in the CSS to remove much of the repetition in styling elements in that file.

## Code Snippet

### HTML changes

```HTML
 <div class="hero"></div>
    <div class="content">
        <div class="search-engine-optimization">
```

above the non-semantic div tags were changed to semantic tags below, Also a image alt text was added here for an image that was placed in the CSS file.

```HTML
 <figure class="hero" title="background meeting image"></figure>
    <section class="content">
      <article class="mainBlock">
```

### CSS changes

```CSS
.header div {
  padding-top: 15px;
  margin-right: 20px;
  float: right;
  font-family: "Gill Sans", "Gill Sans MT", Calibri, "Trebuchet MS", sans-serif;
  font-size: 20px;
}

.header div ul {
  list-style-type: none;
}

.header div ul li {
  display: inline-block;
  margin-left: 25px;
}
```

The code above was changed to the code below to account for the semantic HTML changes from div to section.

```CSS
.header section {
  padding-top: 15px;
  margin-right: 20px;
  float: right;
  font-family: "Gill Sans", "Gill Sans MT", Calibri, "Trebuchet MS", sans-serif;
  font-size: 20px;
}

.header section ul {
  list-style-type: none;
}

.header section ul li {
  display: inline-block;
  margin-left: 25px;
}
```

### CSS optimization

```CSS
.search-engine-optimization {
    margin-bottom: 20px;
    padding: 50px;
    height: 300px;
    font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
    background-color: #0072bb;
    color: #ffffff;
}

.online-reputation-management {
    margin-bottom: 20px;
    padding: 50px;
    height: 300px;
    font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
    background-color: #0072bb;
    color: #ffffff;
}

.social-media-marketing {
    margin-bottom: 20px;
    padding: 50px;
    height: 300px;
    font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
    background-color: #0072bb;
    color: #ffffff;
}
```

above code was changed to .mainBlock to consolidate the repetitive CSS in our file

```CSS
.mainBlock {
  margin-bottom: 20px;
  padding: 50px;
  height: 300px;
  font-family: "Gill Sans", "Gill Sans MT", Calibri, "Trebuchet MS", sans-serif;
  background-color: #0072bb;
  color: #ffffff;
}
```

## Author Links

[LinkedIn](https://www.linkedin.com/in/kevin-xu-4672a7215/)
[GitHub](https://github.com/KevinPXu)
