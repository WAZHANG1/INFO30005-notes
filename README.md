# INFO30005-notes

### Overview </br>
W02-1-MockupsWithXD </br>
W02-2-Git </br>
W02-2-terminal </br>
W02-HTML </br>
W02-Javascript </br>

W03-1-Node </br>
W03-2-Express </br>

W04-DeployYourApp </br>
W04-AdvancedJS </br>

W05-Mongo </br>
W05-Mongoose </br>

W06-Design </br>
W06-HTML </br>
W06-CSS </br>
W06-Responsive </br>

W07-1-Introduction to Client API </br>
W07-2-IntroToHandlebars-1 </br>

W08-1-Handlebars </br>
W08-2-React </br>

W9-1-Authentication </br>
W9 - Security & Risk part 2 </br>

W10-Testing </br>

W11-1-SEO & Accessibility </br>
W11-2-localisation </br>

## Notes
**Git**</br>
Free and open-source Fast, good for teams Branching, staging Very widely-used</br>

**HTML (HypertextMarkupLanguage)**</br>
•	WWW = HTML + HTTP + URL</br>
•	HTML-Structure; CSS-Presentation; JS-Behaviour</br>
•	HTML4: `<b>bold</b>  <i>italic</i>  <u>underline</u>  <s> strikethrough </s>` </br>
•	HTML 5: `<b>Visual emphasis</b> <i> Alternative voice </i> <u> Non-textual annotation </u> <s> Incorrect </s> <em>Emphasis or stress. <strong>Importance  <mark>Relevance` </br>

**CSS (Cascading stylesheet)**</br>
•	Inline: `<h1 style="color:blue">Hello!</h1>` </br>
• Internal: `<head><style>h1{color:blue;}p {color:green;}</style></head>` </br>
• External file: `<head><link rel="stylesheet"href="styles.css"</head>` </br>

**JS**
•	Where JS runs? web browser (front-end): in HTML and JS files / in the dev-tools console •Node (back-end) •VS Code + Code Runner </br>
•	REPL (read eval print loop) </br>
•	Variables: </br>
  Names can contain letters, digits, underscores, and dollar signs. </br>
  Names must begin with a letter, $ + _  </br>
  Names are case sensitive (y and Y are different variables) </br>
  Reserved words (like JavaScript keywords) cannot be used as names  </br>
<img width="266" alt="image" src="https://user-images.githubusercontent.com/80433256/164609825-aee61467-b07a-4c0f-8d29-ddadc1b19927.png">  </br>
•	DOM (Document Object Model) </br>

**Asynchronous programming in JS**
•	To improve performance in networked applications, (long-running) input/output does not block JS programs. </br>
•	JS handles asynchronous processing in 3 ways: •callbacks•promises•async/await </br>

**Callbacks**  </br>
1.One approach to asynchronous programming  </br>
2.Slow actions take an extra argument, a callback function  </br>
3.After the action finishes, the callback function is called </br>
•	Potential problems using callbacks </br>
1.Untidy code: too many levels of nesting </br>
2.Complex and error-prone </br>

**Promises** </br>
1.Object representing the eventual success or failure of an asynchronous action  </br>
2.Two parameters: resolve and reject(for which you write callbacks!) </br>
•	Promise Chain </br> 
Promise chains: feed the result of one promise to another </br>
Promise all: you can use this to resolve multiple promises </br>

**Async/Await** </br>
This is new to JS (2017) and is becoming popular in a number of programming languages. </br>
Allows us to code as if program was synchronous. </br>
Write async before function definition. </br>
Write await to pause execution until the promise is resolved. </br>

**MongoDB** </br>
•	MongoDB vs relational </br>
collections instead of tables </br>
JSON documents instead of rows </br>
no joins (can link or embed) </br>
no schema-related error checking </br>
developer-friendly (schema can evolve)MongoDB vs relational </br>
•	Object Document Modeler (ODM ) </br>

**Mongoose** </br>
	Features: </br>
•	makes various MongoDB tasks easier </br>
•	manage data using object-like methods </br>
•	use schemas to validate user data </br>
•	maintain database schemas in app code </br>
•	types, ranges, enum, required, unique, defaults </br>
•	custom / npm validators (email etc) </br>
•	population (similar to 'join', without ref. integrity) </br>

**API** (APPLICATION PROGRAMMING INTERFACE) </br> 
•	APIs are available with every programming language </br>
•	Collection of interfaces or functions </br>
•	RULES of communication between components to access data or services </br>
•	ABSTRACT or hides implementation details </br>
**BROWSER API** </br>
Built into the browser that allows you do several things, such as: </br>
•	Manipulate the page content (you saw examples last week) </br>
•	Play audio or video </br>
•	Store data on the client (browser) </br>
**THIRD- PARTY API** </br>
•	External providers </br>
•	You can request data by accessing the appropriate API server </br>
•	Examples include: – Map Quest and Google Maps API– Twitter </br>
**XML Http Request(XHR) vs Fetch** </br>
Fetch API is basically a modern replacement for XHR; returns Promise object </br>

**HandleBars** </br>
CLIENT VS SERVER SIDE RENDERING </br>
SERVER-SIDE RENDERING </br>
Server-side rendering is when the web pages are populated with data and resources on the server.  </br>
Faster: avoids round-trips to server to fetch data </br>
Previous lectures on Handlebars is server-side rendering </br>
CLIENT-SIDE RENDERING </br>
Server sends skeleton HTML page and JS. </br>
JS fetches all resources, assembles page, displays page – all on the client </br>

**React** </br>
**JSX** </br>
Looks like HTML and turned into JavaScript code by a compiler. </br>
Babel transpiles JSX to essentially JavaScript </br>
Learn JSX syntax by writing yourself. </br>

**COMPONENTS** </br>
reusable units with information and behavior </br>
Two type of components: classes or functions–Function based components–Class based components </br>

**FUNCTIONAL COMPONENTS AND HOOKS** </br>
What is a hook? </br>
–special function to “hook into” React features </br>
–Enable us to use states </br>
Two types: </br>
–State – manage component state </br>
–Effect – for other React features, e.g.fetching and loading data </br>
USEEFFECT HOOK </br>
Perform side effects </br>
E.g. loading and displaying data after component has been rendered. </br>

**AUTHENTICATION** </br>
The process of verifying the identity of a user who wants to access our app. </br>

**SESSIONS** </br>
•	HTTP is stateless – server does not remember the client (browser) between subsequent requests.  </br>
•	Sessions simulate persistence – server and client can use session data to simulate a persistent connection.   </br>
•	We will use Express session to get started with using sessions with our express apps. </br>

**CLIENT SIDESTORAGE** </br>
Local Storage </br>
Session Storage </br>

**DEFINE PASSPORT.JS STRATEGIES** </br>
•	To use passport, we need to define strategies </br>
•	There are many types (see information link) </br>
– We will learn to use LocalStrategy </br>
--authenticate users using username and password </br>
•	We can define Passport strategies to signup and login user </br>


**JWT (JSON Web Tokens)** </br>
– We define strategies </br>
– Use them to authenticate  </br>
– Secure routes </br>

**Security** </br>

**HTTP vs HTTPS** </br>
•	HTTP =  Hypertext Transfer Protocol, and it is a protocol </br>
•	Browsers and Web Servers use it to communicate  </br>
•	HTTP message types: requests and responses. </br>
•	HTTP requests : messages from client/browser to server.  </br>
•	HTTP responses: data/resources sent in response to to HTTP requests. </br>

•	HTTPS =  Hypertext Transfer Protocol Secure (URL: https://.....) </br>
•	All messages between client and server are encrypted </br>
•	Two keys: public and private </br>
•	Public key is shared with everyone; any message encrypted with public key can only be decrypted by server with private key </br>

•	Server’s need an SSL Certificate </br>
•	SSL = Secure Sockets Layer; encryption-based protocol. </br>
•	SSL Certificate: contains the server’s public key and identity </br>

**Injection**  </br>
vulnerabilities are often found in SQL, LDAP, XPath, or NoSQL queries, OS commands, XML parsers, SMTP headers, expression languages, and ORM queries. </br>
Injection flaws are easy to discover when examining code. Scanners and fuzzerscan help attackers find injection flaws. </br>
XSS (Cross-Site Scripting) </br>
Due to including untrusted data in a new web page without proper validation or escaping </br>
Sanitise anything that gets output to the browser  </br>
Escape HTML, CSS, JS (escape-html) </br>
SCRF (Cross-Site Request Forgery) </br>
Use csurf middleware to protect against cross-site request forgery (CSRF) </br>
Cookie Thief  </br>
Assume cookies are visible Http Only Non-sensitive data in cookies Set cookie expiration, domain & path </br>

**Security principles**  </br>
1) Expect the worst: Focus on prevention instead of reaction </br>
2) Least Privilege: Minimum necessary to get the job done </br>
3) Simple is more secure: The more complex the system, the harder it is to secure </br>
4) Defense in depth: Use layered security mechanisms </br>
5) No security in obscurity: Secrets are hard to keep </br>
6) FAIL SECURELYL: Don’t help your hackers </br>

**Best practice** </br>
•	Regulate requests </br>
•	Validate input  </br> 
•	Sanitise data </br>
•	Keep code private </br>
•	Vague security errors </br>
For example, check size of the data, only allow expected data in, set good default values. Presence/length, type, format, within a set of values, uniqueness. </br>

**Risk Assessment** </br>
risk: An undesirable event with the potential to have a negative impact on the project </br>
Trigger: An event that provides noticeable signs for the group that the risk may actually be happening </br>
Likelihood: Chance of the risk occurring, rated on a scale of likely, possible, or unlikely </br>
impact: Extent to which the group will suffer as a result of the risk occurring, rated as major, moderate, or minor </br>
contingency plan: What to do in the event of the risk actually happening </br>

**Managing risk** </br>
Prevention </br>
Detection </br>
Response </br>
Recovery and Remediation </br>

**SEO (Search Engine Optimisation)** </br>
SEO are strategies and techniques to persuade search engines such as Google, Bing, etc, to   recommend your website to users by obtaining a higher rank. </br>

**SEO Trend** </br>
VISUAL SEARCH: Use descriptive file names and write alt text for every image. </br>
VEDIO: Use descriptive title, description and tags; Upload transcripts </br>
VOICE SEARCH OPTIMIZATION: include FAQ </br>

**Accessibility** </br>
Our web apps should be accessible to users with diverse abilities </br>
•	Define the language </br>
•	Use semantic tags: These tags help screen readers navigate your page, e.g. Screen reader can skip footer or header every time the page is clicked.</br>
•	Create hierarchies with heading levels </br>
•	Markup links: Add more metadata to your HTML, e.g. title for `<a>`Screen readers can allow users to reads headings and help skim the page </br>

**l10n Localisation** </br>
Adaptation to meet the language, cultural, and other requirements of a specific target market </br>

**I18n internationalisation**  </br>
Design and development that support localization– implementation efforts to make it easy to localise a website. </br>
•	Displaying prices in local currency </br>
•	Following local tax regulations </br>
•	Localising your pricing structure </br>
Localisation > Translation </br>
Localisation goes beyond than simple translation. Website designed for UK, American and Australian may be localised based on spelling differences, currency, culture. </br>

**Others** </br>
Locale=parameters that define language + region + preferences] </br>

`app.delete(‘/:id’, function (req,res) { 
people = people.find(x => x.id != req.params.id)
res.send(people)
})` </br>

`app.get(‘:/id’, function (req.res) {res.send(people.find(x => x.id == req.params.id))})`
