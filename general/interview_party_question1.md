# Party Question 1
## Intro
This series of questions has been used to squeeze a technical assessment out of as little as 25 minutes.

## Question Sequence
1. implement a function to detect if a submitted string is a palandrome. Whitespace, capitalization, and punctuation to be ignored.
1. "Now that we have our 'cool' string processing IP, discuss we might go about making it available to the world as a web service". Specificially, we want a RESTful API endpoint. 
1. Given that we now have an endpoint to our service, what data might our business and engineering leaders want us to capture? What entities do you foresee, what storage tools would you use, and what schema's(data archetypes) would you capture.
1. Now that we have our cool string processing tool, and the ability to capture 'interesting' metadata, how should we deploy? What tools, strategies, techniques to you envision being a part of our developement pipeline and deployment strategy?
1. We now have a successful service, as part of our monitization plan, we need to introduce security. What steps do you foresee as needed inorder to "lock down" our endpoint to valid users?
1. We now have a *wildly* successful service, and need to rate limit requests. How would we go about implementing ratelimitting for our API? (What strategies, tools, ect do you anticipate using as part of this effort?)

## Evalutaion Criteria
### STring processing
In whatever language we are evaluating, where are looking for strong:
1. string processing skills
1. understanding of scalability
1. correct iteration
1. problem decomp.
   1. cleaning the input
   1. palandrome dectection on cleaned input

### API Design
there are multiple ways to exposing this string processing algorithm as an service. Top candidates will mention several, with some pros and cons for each, and settle on one.

Ideally, candidates will discuss serialization strategies, eg:
- using a GET, url-encode the query string a la: api/ispal/<uslencoded str>
- using a POST to api/ispal, with a body in JSON similar to: ....

### Schema Design, Data Modeling
Which such a general question we are really looking for a candidate who can put on their business analysis hat, and try to empathize with the business.

Entities we expect a reasonable candidates to work with include:
- user
- search term
- performance data

Top candidates will suggest new features, or business value that can be derived from the accumiatled data. eg:
- historical queries
- trend extraction
- "did you mean..."

For what ever tools they suggest, they should be able to suggest queries that would be useful and efficient.

### API security
### Deployment
should probably mention "containers" to be anything other than a junior candidate

more advanced candidates should discuss testing, CI/CD, orcestration, possibly kubernetes. 

### Rate Limitting

