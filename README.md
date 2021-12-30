# github-page-demo
This is the one that show CI/CD and does webservice demo using "github pages"
- Based on source : https://www.youtube.com/watch?v=QyFcl_Fba-k

```html
<p>host : github/your_repo</p> 
``` 
  - make github repository named "github-page-demo"  // any name you want
  - copy url 

```html
<p>host : your local host</p> 
```
  - $clone it into your local(working) host computer  or open repository using VScode 
  - make index.html   // easy way  : copy context from w3school
  - $git add .
  - $git commit "Initial commit"

```html
<p>host : your_repo</p> 
```
- job : make "web host" working settings
  - select your repo and check index.html file exists
  - menu: "Settings"=>"GitHub Pages" =>
       select "Branch:main", "/root" and save 
  - your site url : https://your_if_of_github.github.io/your_repo
  -                 ex> my site :   https://manulsan.github.io/github-page-demo

```html
<p>DONE, YOU CAN SEE THE WEB SITE</p> 
```

```html
<p>Additional information for git branches managements</p> 
```

```html
<p>host : local host</p> 
```
  - $git checkout -b styling
  - do file working
    - make styless.cs
    - modify index.html with css style
  -$ git add .
  -$ git commit -m "Styling commit"
  -$ git push origin styling

```html
<p>host : github/your_repo</p> 
```
- select branch named "styling"
  - "Compare and pull request"
  - click "Create pull request"
  - select branch named "main"
    => check that branch is merged , access web service that the modified css is applied

```html
<p>DONE</p> 
```

```html
<p>Additional information : make another branch for services</p> 
```

```html
<p>host : local host</p> 
```
  - $git checkout -b site
  - $git push origin site

```html
<p>host : github/your_repo</p> 
```
 - job : make "web host" working settings
   - select your repo and check index.html file exists
   - menu: "Settings"=>"GitHub Pages" =>
       select "Branch:site", "/root" and save 

```html
<p>host : local host</p> 
```
  - html file job
    - make contact.html
    - add link to index.html
