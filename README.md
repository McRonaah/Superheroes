# Getting started

Clone this repository to your machine: git clone git@github.com:McRonaah/Superheroes.git

Change the directory into the project directory: cd Superheroes

To open in your code editor run: code .

To install all dependencies run: bundle install

To test the routes open your server by running :rails s

# Deliverables
Routes are setup to the following routes and return JSON data in the format below:

[  

{ "id": 1, "name": "Kamala Khan", "super_name": "Ms. Marvel" },  

{ "id": 2, "name": "Doreen Green", "super_name": "Squirrel Girl" },  

{ "id": 3, "name": "Gwen Stacy", "super_name": "Spider-Gwen" }

]


GET /heroes/:id
If the `Hero` exists, return JSON data in the format below:


{
  "id": 1,
  "name": "Kamala Khan",
  "super_name": "Ms. Marvel",
  "powers": [
    {
      "id": 1,
      "name": "super strength",
      "description": "gives the wielder super-human strengths"
    },
    {
      "id": 2,
      "name": "flight",
      "description": "gives the wielder the ability to fly through the skies at supersonic speed"
    }
  ]
}


If the `Hero` does not exist, return the following JSON data, along with
the appropriate HTTP status code:

{   "error": "Hero not found" }

 GET /powers
Return JSON data in the format below:


[
  {
    "id": 1,
    "name": "super strength",
    "description": "gives the wielder super-human strengths"
  },
  {
    "id": 1,
    "name": "flight",
    "description": "gives the wielder the ability to fly through the skies at supersonic speed"
  }
]


 GET /powers/:id
If the `Power` exists, return JSON data in the format below:

```
{
  "id": 1,
  "name": "super strength",
  "description": "gives the wielder super-human strengths"
}
```

If the `Power` does not exist, return the following JSON data, along with
the appropriate HTTP status code:

```
{
  "error": "Power not found"
}
```

 PATCH /powers/:id
This route should update an existing `Power`. It should accept an object with
the following properties in the body of the request:

```
{
  "description": "Updated description"
}
```

If the `Power` exists and is updated successfully (passes validations), update
its description and return JSON data in the format below:

```
{
  "id": 1,
  "name": "super strength",
  "description": "Updated description"
}
```

If the `Power` does not exist, return the following JSON data, along with
the appropriate HTTP status code:

```
{
  "error": "Power not found"
}
```

If the `Power` is **not** updated successfully (does not pass validations),
return the following JSON data, along with the appropriate HTTP status code:

```
{
  "errors": ["validation errors"]
}
```

 POST /hero_powers
This route should create a new `HeroPower` that is associated with an
existing `Power` and `Hero`. It should accept an object with the following
properties in the body of the request:

```
{
  "strength": "Average",
  "power_id": 1,
  "hero_id": 3
}
```

If the `HeroPower` is created successfully, send back a response with the data
related to the `Hero`:

```
{
  "id": 1,
  "name": "Kamala Khan",
  "super_name": "Ms. Marvel",
  "powers": [
    {
      "id": 1,
      "name": "super strength",
      "description": "gives the wielder super-human strengths"
    },
    {
      "id": 2,
      "name": "flight",
      "description": "gives the wielder the ability to fly through the skies at supersonic speed"
    }
  ]
}
```

If the `HeroPower` is **not** created successfully, return the following
JSON data, along with the appropriate HTTP status code:

```
{
  "errors": ["validation errors"]
}
```

# Interactivity with the user
-One is able to go through the railway schedule.

-One is able to order for train tickets.

-one is able to like, comment to our services provided.

# Support or Contribution
For any suggestions or contributions please do not hesitate to contact the owner of this repository.

Contributions to this project are welcomed by all, If you need to contribute send your github profile to contacts below and follow the steps below

-Fork the repository

-Follow the procedure as explained earlier.

-Create a branch off develop for the feature you wish to add

-Make neccessary changes, commit and raise a pull request against develop,

-Note when making contributions, please endevour to follow good coding practice.

# Contacts.
Below you will find our contact information:

WhatsApp; +254702233145

Call / Message; +254111310907

E-mail; ronaldcheruiyot342@gmail.com

Fax; +1(001122698791)