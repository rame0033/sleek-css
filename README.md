# Sleek CSS Stylesheet

Lightweight CSS framework for minimal designs.

## Installation Guide
The Github pages is enabled in this repository so this will generate a public URL:

`https://rame0033.github.io/sleek-css/css/style.css`


### Option 1 - The public URL should be included in your HTML as

`<link rel ="stylesheet" href="https://rame0033.github.io/sleek-css/css/style.css">`

### Option 2 - Download and Use locally
- You may download directly the CSS file from:
https://github.com/rame0033/sleek-css/blob/main/css/style.css
- Once downloaded, you can import it into your project folder and link to your HTML.

Note: A CSS Reset is also included in this stylesheet so you don't have to link another reset stylesheet regarding this matter.

## Basic Usage

### Container
The container has a width of 70% and a default position of `margin: 0 auto`. To apply the container spacing, include the class name `container` regardless if it is in an HTML tag such as `<main>`, `<section>` or even a `<div>`. 

### Headings
The heading must be enclosed first in a container classified as `heading-container` to apply the styling. 

The example is being shown as follows

```
<div class="heading-container">
    <h1 class="h4-bold"> This is a Heading </h1>
</div>
```
*This applies to `<h1>` to `<h4>` HTML tags*

### Font Weights and Text Syles
ONLY applies to headings inside the heading-container as shown earlier. The following are the classes that one you can use for font-weights such as:
- `h4-reg`
- `h4-bold`
- `h4-italic`
- `h4-hyper`

### Color boxes
With this stylesheet, user can add background colors on their container with the following class names:
- `color-container color-pri`
- `color-container color-sec`
- `color-container color-info`
- `color-container color-success`
- `color-container color-danger`

### Cards
There are several types of cards that users can make as component in the HTML file. One may copy the following HTML code to make the component

- Full card component that includes the picture, and the card body with heading, paragraph and link

```
<div class="card">
    <img src="https://placehold.co/600x400" class="card-img-top" alt="Placeholder Image">
        <div class="card-body">
            <h4 class="card-title">Card Title</h4>
               <p class="card-text">Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam, quod.</p>
               <a href="#" class="btn btn-primary">Read More</a>
        </div>
</div>

```

- Card component that only includes the photo and body paragraph

```
<div class="card">
    <img src="https://placehold.co/600x400" class="card-img-top" alt="Placeholder Image">
        <div class="card-body">
            <p class="card-text">Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam, quod.</p>
        </div>
</div>
```
- Card component that only includes heading, paragraph, and link

```
<div class="card">
    <img src="https://placehold.co/600x400" class="card-img-top" alt="Placeholder Image">
        <div class="card-body">
            <p class="card-text">Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam, quod.</p>
        </div>
</div>

```

### Lists
There are several list styles that user can add in their HTML.

#### For `<ul>` and `<ol>`
One may classify the container first as `.list-container` and include either `<ol>` or `<ul>` inside the div.

It shall be written like the example below

```
<div class="list-container">
  <h4>This is a list</h4>
    <ol>
      <li>Item 1</li>
      <li>Item 2</li>
      <li>Item 3</li>
      <li>Item 4</li>
    </ol>
</div>
```

#### Description List
User may add a desscription list in HTML file written as

```
 <div class="list-container">
    <h4>Description List</h4>
            <dl>
                <dt>Item 1</dt>
                <dd>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore
                    et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut
                    aliquip ex ea commodo consequat.
                </dd>
                <dt>Item 2</dt>
                <dd>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore
                    et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut
                    aliquip ex ea commodo consequat.
                </dd>
                <dt>Item 3</dt>
                <dd>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore
                    et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut
                    aliquip ex ea commodo consequat.
                </dd>
                <dt>Item 4</dt>
                <dd>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore
                    et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut
                    aliquip ex ea commodo consequat.
                </dd>
            </dl>

</div>

```
### Buttons and Links
There are several stylings that can be applied for buttons and links

#### For links
- One may include in the `<a>` tag the class `btn btn-primary`

#### For buttons
One may include several classes to style respective buttons
- `btn-primary`
- `btn-secondary`
- `btn-info`
- `btn-success`
- `btn-danger`

### Forms
The user may include the form as HTML tag written as follows

```
 <form action="">
                <div class="form-group">
                    <label for="full-name">Full Name</label>
                    <input id="full-name" type="text" placeholder="John Doe"/>
                </div>
    
                <div class="form-group">
                    <label for="email">Email</label>
                    <input type="email" id="email" placeholder="johndoe@gmail.com"/>
                </div>
    
                <div class="form-group">
                    <label for="message">Message</label>
                    <textarea name="message" id="message" placeholder="Type in the message you want to send"></textarea>
                </div>
                
                <button type="submit">Submit</button>
            </form>
```