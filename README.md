# therealcurlsport
## Oscarg933
### Skip to content
 
Search or jump to…

Pull requests
Issues
Marketplace
Explore
 @therealvenenoiot Sign out
0
1 193 1010101012101/jarvis
forked from zouhir/jarvis
 Code  Pull requests 0  Projects 0  Insights  Settings
A very intelligent browser based Webpack washboard https://live com
 155 commits
 8 branches
 2 releases
 24 contributors
 JavaScript 63.3%	 CSS 34.5%	 Shell 1.3%	 HTML 0.9%
 Pull request   Compare This branch is 1 commit ahead of zouhir:master.
@therealvenenoiot
therealvenenoiot Create therealcurlsport
Latest commit 9bd3b67  a minute ago
Type	Name	Latest commit message	Commit time
.github	Added PR template, addresses some issues in zouhir#79 (zouhir#113)	11 months ago
config	fix brokrn package and some cleanup (zouhir#130)	10 months ago
https/github.com/therealvenenoiot	Create therealcurlsport	a minute ago
scripts	Added basic favicons that show state (closes zouhir#68) (zouhir#74)	a year ago
src	Add table sort feature (zouhir#137)	7 months ago
.all-contributorsrc	Add all code contributors to readme (zouhir#95)	a year ago
.editorconfig	batch#1: webpack emitting to client, dash kickoff	a year ago
.gitignore	Make an explicit dist folder, rather than using lib (zouhir#124)	11 months ago
README.md	Ability to set custom package.json path (zouhir#116)	10 months ago
package-lock.json	fix brokrn package and some cleanup (zouhir#130)	10 months ago
package.json	fixed borken images \ assets (zouhir#131)	10 months ago
 README.md


 version  version  License: MIT
About the Project
J.A.R.V.I.S. (Just A Rather Very Intelligent System) will put in your browser all the relevant information you need from your webpack build whether in dev or in prod.

Tons of features are on the roadmap but still, this beta version will improve the way you look at webpack-dev-server or webpack production build bundle, chunks and other output assets.

It is hugely inspired by other webpack dashboards and the core idea is not original, but here are some features:

Original Features:

Shows you the count of ES Harmony module imports which can be treeshakable and the CJS ones which are not.
Shows you how well your assets perform in 12 different connection types.
Google or Stackoverflow Search for programming errors in 1 button click.
Other Features:

Runs in the browser.
Beautified errors output.
Easy way figure out total assets size and individual bundles and chunks.
It's very beautiful.
Tech Stack:

Preact with Sass pre-processor.
Socket IO.
Polka Server.
Screenshot:



Installation
$ npm i -D webpack-jarvis
In your webpack config file:

const Jarvis = require("webpack-jarvis");

/* the rest of your webpack configs */

plugins: [
  new Jarvis({
    port: 1337 // optional: set a port
  })
];
In your browser open:

localhost:1337
and you are all set!

Options
Options are (optionally) passed in to the constructor

new Jarvis(options);
options.port
Type: Number
Default: 1337

The Jarvis dashboard will open on a localhost server at this port.

options.host
Type: String
Default: localhost

The Jarvis dashboard will attach to this host, e.g. 0.0.0.0.

options.watchOnly
Type: Boolean
Default: true

If set to false, then Jarvis will also run for non-watch builds, and keep running after the build completes.

options.packageJsonPath
Type: String
Default: process.cwd()

Jarvis will look inside this directory for your package.json.

Help & Contribute
Setting up the dev environment

Install Dependencies:

$ npm install
Run Jarvis in your browser, Jarvis root:

$ npm run watch
Finally, open a browser to http://localhost:1337!

On the roadmap:

Cleanup the hacky code in the client app, it's embarassing, I'm sorry!
Enforce best practices, structure and higher code quality standards.
Bundle size analyzer like feature in the table.
Build snippets page.
Build Oppurtunities Section to suggest loaders, plugins, etc. that can improve your build and bundle.
Note:

I am not entirely sure how many bugs you will catch while it's in beta, but what I know for sure is the whole app, especially the client Preact app can be dramatically improved, JS & CSS and structure wise as the whole thing has been built in a rush in a very hacky way.

Contributors
Thanks goes to these wonderful people (emoji key):


Zouhir zap
computer thinking	
Luke Edwards
computer	
Ari Picker
computer	
Marius Niveri
computer	
Gagan
book	
石发磊
book	
ZiYingMai
computer

rachmulvey
computer	
Stephan Schneider
book	
Christopher Peng
computer	
Francesco Soncina
computer	
Jeremy Monson
computer	
Gusten
computer	
Tamas Sule
computer

remmy hume
computer	
Michael Persson
book	
Zach Gawlik
computer book	
Khachatur
computer	
Timo M. Staudinger
computer		
This project follows the all-contributors specification. Contributions of any kind are welcome!

Credits
Webpack Dashboard by Formidable Labs
License
MIT © Zouhir

© 2019 GitHub, Inc.
Terms
Privacy
Security
Status
Help
Contact GitHub
Pricing
API
Training
Blog
About
Press h to open a hovercard with more details.
