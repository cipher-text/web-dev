# web-dev
In this repository i will put whatever i learn in web development for reference purpose


### React
###### environment setup (windows)
>install node to manage packages
>install vs code
> open terminal(command prompt) and type following to install react package glbally
``` 
npm i -g create-react-app
```
>install following extension in vscode
1. Simple React Snippet https://marketplace.visualstudio.com/items?itemName=burkeholland.simple-react-snippets
2. Prettier https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode
>now make some changes in vscode setting so that it can format code every time when you save 
>go to   preferences->setting> ( or ctrl+,)
>now search  ---     editor.formatonsave  mark it true
### css

![picture](https://content.linkedin.com/content/dam/me/learning/blog/2016/september/CSS.jpg)

#### basic
> css makes your page look good
> css can be applied in three different ways
1. inline    => 
ex. ```<h1 style="background:red;padding:4px;">Heading</h1>```
2. internal  => 
ex. add inside the head tag  ```<style> h1{color:white;} </style>```
3. external  => 
ex. write css into different page and link it with html  add link in head section 
```<link rel="stylesheet" href="path of file">```
###### types of selector
![picture](https://github.com/cipher-text/web-dev/blob/master/readme-images/selector-img1.png)
![picture](https://github.com/cipher-text/web-dev/blob/master/readme-images/selector-img2.png)
###### different types of combinator
note:- here in picture only combined two selector but you can combine multiple
ex-   ```div p a{
      color:red;
         }```
![picture](https://github.com/cipher-text/web-dev/blob/master/readme-images/combinator-img1.png)
![picture](https://github.com/cipher-text/web-dev/blob/master/readme-images/combinator-img2.png)
![picture](https://github.com/cipher-text/web-dev/blob/master/readme-images/combinator-img3.png)
![picture](https://github.com/cipher-text/web-dev/blob/master/readme-images/combinator-img4.png)
![picture](https://github.com/cipher-text/web-dev/blob/master/readme-images/combinator-img5.png)
![picture](https://github.com/cipher-text/web-dev/blob/master/readme-images/combinator-img6.png)
![picture](https://github.com/cipher-text/web-dev/blob/master/readme-images/specificity.png)
![picture](https://github.com/cipher-text/web-dev/blob/master/readme-images/shorthand-prop.png)
![picture](https://github.com/cipher-text/web-dev/blob/master/readme-images/margin-collapsing.png)
![picture](https://github.com/cipher-text/web-dev/blob/master/readme-images/Screenshot%20(453).png)
![picture](https://github.com/cipher-text/web-dev/blob/master/readme-images/Screenshot%20(458).png)
![picture](https://github.com/cipher-text/web-dev/blob/master/readme-images/Screenshot%20(459).png)
![picture](https://github.com/cipher-text/web-dev/blob/master/readme-images/Screenshot%20(460).png)
![picture](https://github.com/cipher-text/web-dev/blob/master/readme-images/Screenshot%20(462).png)
![picture](https://github.com/cipher-text/web-dev/blob/master/readme-images/Screenshot%20(465).png)
###### position property
> position property can be applied in different ways following are the ways
1. ```position: static ```
2. ```position: fixed  ```
3. ```position: absolute ```
4. ```position: relative ```
5. ```position: sticky ```

 ```
 top 
 left
 right
 bottom
 ```
 
 
>static : it is the default position of element where element follow the document flow
>fixed : in case of fixed positioning the element taken out of document flow and it refer to the view port
>absolute: in case of absolute the element is taken out of document flow and it refer to any parent where position property applied but >if there is no such parent then it refer to html
>relative: in case of relative the document is not taken out of document flow and it refer to itself
####### z-index
>to position element along z axis  we can apply z-index property
>note: z-index property can be applied only if element have position property applied
```
z-index: (+/-)
```


####### overflow:hidden
>it hides the element if it get out of parent
>note: if you apply ```overflow:hidden``` in body element it won't work because it will simply plass the ```overflow:hidded``` to the html element
> so what you made
```
body{
overflow:hidden;
}
```
> but what will happen
```
html{
overlow:hidden;
}

body{
}
```
>to overcome this problem you should apply overflow property in both html and body
```
html{
overflow:hidden;
}
body{
overflow:hidden;
}
```
###### position:sticky
> it is the hybrid of position fixed and relative

###### stacking context
> each element have stacking context and element inside it can be stacked only relative to element inside it
![picture](https://github.com/cipher-text/web-dev/blob/master/readme-images/Screenshot%20(467).png)

##### Variable in css
> to use variable in css that helps to get rid of multiple changes if more than one palces have same value
![picture](https://cdn-media-1.freecodecamp.org/images/XjRjOOsd5x9tj7-HtCx5CxhWQqfS-Ih9brdo)


> notice that these variable are just for presentation purpuse they are not visible in document
> property: (var(--variable-name, a, b, c);   // a, b, c are fallback values that will be considered in case of custom value not work
