# first-vue-proj

> first project

## Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build
```

## Guide
 - **Vue Instance 'Options'**:
   - ***el*** *{string | HTMLElement}*
     - provide the Vue instance with an existing DOM element
   - ***template*** *{string}*
     - a string template to be used as the markup for the Vue instance.
     - by default, it will replace the mounted element
   - ***render*** *{(createElement: () => VNode) => VNode}*
     - alternative to templates, instead using javascript
   - ***renderError*** *{(createElement: () => VNode) => VNode}*
     - alternative to render when render function encounters an error
   - ***data*** *{Object | Function}*
     - only accepts function when used in Vue.extend()
   - ***props*** *{Array<string> | Object}*
   - ***propsData*** *{ [key: string]: any }*
     - pass props to an instance during its creation
   - ***methods*** *{ [key: string]: Function }*
     - standard methods/functions that get run everytime any data is updated
   - ***computed*** *{ [key: string]: Function | { get: Function, set: Function } }*
     - same as methods, but only run when specified data within functions is updated
   - ***watch*** *{ [key: string]: string | Function | Object | Array}*
     - an object where keys are expressions to watch and values are the callbacks