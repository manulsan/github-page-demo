# github-page-demo
This is the one that show CI/CD and does webservice demo using "github pages"
- Based on source : https://www.youtube.com/watch?v=QyFcl_Fba-k

// host : your_repo --------------------------------------------------------// 
- make github registory named "githug-page-demo"  // any name you want, check "Add a README file"
- copy url 

// host : your local host-------------------------------------------------// 
- $clone it into your local(working) host computer  or open repository using VScode 
- make index.html   // easy way  : copy context from w3school
- $git add .
- $git commit "Initial commit"

// host : your_repo --------------------------------------------------------// 
* job : make "web host" working settings
- select your repo and check index.html file exists
- menu: "Settings"=>"GitHub Pages" =>
       select "Branch:main", "/root" and save 
- your site url : https://your_if_of_github.github.io/your_repo
-                 ex> my site :   https://manulsan.github.io/github-page-demo

//------------ DONE, YOU CAN SEE THE WEB SITE ---------------------//

// Additional information for git branches managements//
// host : local host --------------------------------------------------------// 
$git checkout -b styling
- do file working
   make styless.cs
   modify index.html with css style
$git add .
$git commit -m "Styling commit"
$git push origin styling

// host : github/your_repo --------------------------------------------------------// 
* host : github/your_repo,  
- select branch named "styling"
- "Compare and pull request"
- click "Create pull request"
- select branch named "main"
      => check that branch is merged , access web service that the modified css is applied

//---------------------- DONE ----------------------//
      
// Additional information : make another branch for services //

// host : local host --------------------------------------------------------// 
$git checkout -b site
$git push origin site

// host : github/your_repo --------------------------------------------------------// 
* job : make "web host" working settings
  - select your repo and check index.html file exists
  - menu: "Settings"=>"GitHub Pages" =>
       select "Branch:site", "/root" and save 

// host : local host --------------------------------------------------------// 
* html file job
  - make contact.html
  - add link to index.html
