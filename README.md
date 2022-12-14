<h1>Brief Explanation about the Web Services Used</h1>
<p><span>I have used a total of <strong>7 OpenAPIs</strong>, 1 Informative Website, 1 special node-red module, and 2 special node-red nodes for the successful implementation of this service:</span></p>
<p><strong><span>Node-red-node-ui-iframe</span></strong><span>: - It allows one to embed other web pages within the node-red dashboard. It can also be used to embed images from other sites.&nbsp;</span></p>
<p><strong><span>Node-Red-chart-node</span></strong><span>:- It can be used for displaying input information in the form of charts.&nbsp;</span></p>
<p><strong><span>Node-red-dashboard:&nbsp;</span></strong><span>It allows the swift creation of webpages without the necessity of using HTML. Furthermore, it allows the use of other nodes within it to provide different features.</span></p>
<p><strong><span>Nationalize API</span></strong><span>:- It takes in the name of an individual and predicts the nationality of the individual. It outputs the ISO3166-1 2-digit code of the country.</span></p>
<p><strong><span>Flagpedia API:&nbsp;</span></strong><span>It takes in the ISO3166-1 2-digit code of a country in lowercase and gives out the image of a flag of the country.&nbsp;</span></p>
<p><strong><span>NewsData API</span></strong><span>: It takes in the ISO3166-1 2-digit code of a country and outputs the headline news information of the input country with a reference webpage and short description for the headline news.</span></p>
<p><strong><span>Geoapify API:-&nbsp;</span></strong><span>I utilized 2 different functions of the API:</span></p>
<ol start="1">
    <li><strong><span>Geoapify Geocoding API:</span></strong><span>- It receives the country name as input and gives out the latitudinal and longitudinal information of the country.</span></li>
    <li><strong><span>Geoapify StaticMap API:- &nbsp;</span></strong><span>It receives the latitudinal and longitudinal information of a country and outputs a static map that displays the country on a map.&nbsp;</span></li>
</ol>
<p><strong><span>WeatherStack API</span></strong><span>:- It takes in the latitudinal and longitudinal information of a country and outputs the weather description of the country. Furthermore, it outputs an image link describing the weather condition of the country.</span></p>
<p><strong><span>Covid19.mathdro.id API</span></strong><span>:- It takes in the country name and outputs the country&rsquo;s COVID-19 info.&nbsp;</span></p>
<p><strong><span>Bilingua.io Website:&nbsp;</span></strong><span>A page I found helpful for starting conversations with new people. Reference:&nbsp;</span><span><a href="https://bilingua.io/100-simple-fun-conversation-exchange-topics"><span>https://bilingua.io/100-simple-fun-conversation-exchange-topics</span></a></span></p>
<h1>Explanation about the Mashup Application</h1>
<p>This mashup application is designed to assist in starting a conversation with a foreigner. Various pieces of research show that students studying abroad and ex-pats are at a very high risk of experiencing depression, and suggest interacting with others as the best way to beat depression. As a foreigner studying in Korea, I and many of my foreign friends experience difficulty beginning a conversation with a fellow foreigner, especially during our initial days after coming. This mashup application exactly tries to solve this problem by assisting in brainstorming various conversation starting points with a foreigner.</p>
<p>The application takes in the name of an individual through its UI, probably the name of a foreigner you just encountered. Then it predicts the country the individual came from based on his name using the nationalize.io API. Next, it uses the country name to display the flag and headline news of the country using the Flagpedia and Newsdata API, respectively. Then, it utilizes the Geoapify Geocoding API to get the longitudinal and latitudinal information of the country and displays the location of the country on a static map by using the Geoapify StaticMap API. The Geoapify StaticMap API accepts the longitudinal/latitudinal information from the Geocoding API to display the country???s geographical location on the static map, while the WeatherStack API displays the weather information using those inputs. Furthermore, the mashup also displays the Covid-19 information of the country graphically by making use of the covid19.mathdro.id API and the chart node of node-red. Finally, it frames another site with a list of interesting conversation topics.</p>
<p>The main aim of this mashup is to facilitate a smooth conversation with a foreigner you just met and only know his/her name and help fight depression, one of the main problems experienced in KAIST.</p>
<h2>Sample Results:</h2>
<p>Input Sample#1: <strong>Feven</strong>, a common Ethiopian female name. The result can be seen below:</p>
<img src='ethio.png'><img>
<p>Input Sample#2: <strong>Park</strong>, a common Korean name. The result can be seen below:</p>
<img src='korea.png'><img>
<p>Input Sample#3: <strong>Haruto</strong>, a common Japanese name. The result can be seen below:</p>
<img src='japan.png'><img>
<h2>References:</h2>
<p>Enhancing Social Interaction in Depression: https://bmjopen.bmj.com/content/8/9/e020448</p>	
<p>Prevalence and correlates of mental health symptoms and disorders among international college students: https://www.ncbi.nlm.nih.gov/pmc/articles/PMC8677361/</p>	
<p>The Dark Side of Living Abroad: https://www.dailysabah.com/life/health/the-hushed-up-dark-side-of-living-abroad-expat-depression</p>
<p>The Expat life: https://www.apa.org/monitor/2019/2019-05-monitor.pdf</p>
<p>Documentations for each API</p>
<em>This assignment is done as part of KAIST Introduction to Services Computing course CS459.</em>

