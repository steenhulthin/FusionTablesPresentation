### "Visualizing data on maps using Googles Fusion Tables and the Google Maps API"

!

Short title:
### How can you use Fusion Tables?

!

### Steen Hulthin Rasmussen

### percipio.dk


***
> `twitter: @steenhulthin`
>
> `blog: steen.hulthin.dk/blog`

!

#### "We added maps to our website ... with no extra maintance cost."

> _official at MBBL*_ 

###### _* Ministry of Housing, Urban and Rural Affairs_

#### "It's Cloud and totally Web Scale!"

> _A hipster on the internet_

!

The 2-minutes Version
---------------------

Google Maps is digital maps...

Fusion tables is a table store with built-in interactions with Google Maps (and Google Chart tools)

Let's see it is action!

!

My story... (1)
===============

MBBL requirements:

1. Visualise data quality of BBR* on maps
2. Low/no server maintance cost

> *BBR is a database containing all building and addresses in Denmark

!

My story... (2)
===============

* Some knowledge of Fusion Tables with Google Maps from abandoned project:
[postnummerkortet.dk](http://postnummerkortet.dk/version2/)
* Quality data available 
* No server cost (for small sites)

Ok ready as can be!

!

Architechture draft
-------------------

<img src="architechture_first_draft.jpg" alt="Drawing" style="width: 100%; height: 100%; "/>

!

Revised architechture
---------------------

<img src="revised_architechture.jpg" alt="Drawing" style="width: 100%; height: 100%; "/>

!

Stumbling Block 1
-----------------

Getting geodata into a Fusion Table

Fusion tables only support one geodata format: kml

> tips: [http://www.shpescape.com/](http://www.shpescape.com/) and Quantum GIS

!

New architechture
-----------------

<img src="new_architechture.jpg" alt="Drawing" style="width: 100%; height: 100%; "/>

!

Stumbling Block 2
-----------------

Signing up for Google APIs. 

Here it is: [http://code.google.com/apis/console](http://code.google.com/apis/console)

Or on [https://developers.google.com/](https://developers.google.com/) find `API Console` under `Developer Tools` (if you can)

For read-only access a `Simple API Access` is fine

For read-write a `client ID` is necessary

Let see that.

!

Stumbling Block 3
-----------------

OAuth is not super simple!

Requires manual interaction the first logon.

Subsequent requests can be made with a refresh token

!




!



!

restrictions 
25000 requests / day BUT boost limit.

! 
Test user 
Prod user
users have their own data.


#. What is Fusion Tables
#. The status of Fusion Tables as being "beta"
#. What is Google Maps api?
#. Spatial data - the simple version. Data with a location.
#. OAuth ....
#. Code 
#. the challanges
#. restriction

# best used for
# don't use for



The case:
customer needs:
	hosting, no
	many users, no
	status of the project, prototype-ish 

Getting the api key. read access vs write access and the quirks around it. 
Setting up accounts (test, prod, whatever). There could be better ways. Use personal account? probably not for any production system. Lifetime.

Importing spatial data
======================
tool for shp import. 
Import into fusion tables. 
Spatial reference.


!

Questions?

!

