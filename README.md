# Arquivo JSON- Assunto Villagers from Animal Crossing New Horizon 



JSON 1

![img](https://static.wikia.nocookie.net/animalcrossing/images/c/c1/Coach_NH.png/revision/latest/scale-to-width-down/309?cb=20200817163652)

{
    "_id" : ObjectId("6101b787ad5377c81a8c451f"),
    "acnh" : {
        "name" : "Coach",
        "type" : "Bull",
        "birthday" : "29 de Abril-Touro",
        "nitialPhrase" : "LET'S GO TEAM! WOOOOOOOOO!",
        "skill" : "eating quickly",
        "goal" : "fisherman",
        "favoriteSong" : "Mr.K.K"
    },
    "personality" : {
        "personality" : "jock",
        "interests" : "great interest in sports and bodybuilding",
        "relationship" : " get along with peppy, cranky and sisterly villagers"
    },
    "house" : "A gym for athletic contests"
}

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------



JSON 2 

![img](https://static.wikia.nocookie.net/animalcrossing/images/5/5d/Cyd_NH.png/revision/latest/scale-to-width-down/268?cb=20200319212643)

{
    "_id" : ObjectId("6101b8fcad5377c81a8c4563"),
    "acnh" : {
        "name" : "Cyd",
        "type" : "Elephant",
        "birthday" : "June 9th (Gemini)",
        "nitialPhrase" : "Y'know, I do believe I recognize a few of these folks from back in the day! Gahaha!",
        "skill" : "guitar playing",
        "goal" : "rock star",
        "favoriteSong" : "K.K.metal"
    },
    "personality" : {
        "personality" : "cranky",
        "interests" : "great interest in sports and bodybuilding",
        "relationship" : "get along with jock, snooty and other cranky villagers, and occasionally lazy and normal villagers"
    },
    "house" : "punk/metal theme"
}

--------------------------------------------------------------------------------------------------



JSON 3

![img](https://static.wikia.nocookie.net/animalcrossing/images/f/f9/Drago_NH.png/revision/latest/scale-to-width-down/340?cb=20200802062031)



{
    "_id" : ObjectId("6101b9b2ad5377c81a8c458b"),
    "acnh" : {
        "name" : "Drago",
        "type" : "Alligator",
        "birthday" : "February 12th (Aquarius)",
        "nitialPhrase" : "This might sound kind of weird, but I really love the smell of dirt, burrrn.",
        "skill" : "blowing bubbles",
        "goal" : "pilot",
        "favoriteSong" : "imperial K.K."
    },
    "personality" : {
        "personality" : "lazy",
        "interests" : "a love of food and relaxing",
        "relationship" : "get along well with other villagers"
    },
    "house" : "many furniture pieces from the Imperial set"
}

----------------------------------------------------------------------------------

JSON 4

![img](https://static.wikia.nocookie.net/animalcrossing/images/d/d1/Mira_NH.png/revision/latest/scale-to-width-down/247?cb=20200719093646)

{
    "_id" : ObjectId("6101bb92ad5377c81a8c45e7"),
    "acnh" : {
        "name" : "Mira",
        "type" : "rabbit",
        "birthday" : "July 6th (Cancer)",
        "nitialPhrase" : "You can wear it and show me how to make it look good! Thanks for the delivery! Cottontail!",
        "skill" : "telling jokes",
        "goal" : "make up artist",
        "favoriteSong" : "go K.k. rider"
    },
    "personality" : {
        "personality" : "sisterly",
        "interests" : "care deeply about her appearance",
        "relationship" : "get along with jock villagers who share her love of sports, lazy villagers for how laid-back they are, and peppy villagers."
    },
    "house" : "A futuristic space"
}

----------------------------------------------------------------------------------------

JSON 5

![img](https://static.wikia.nocookie.net/animalcrossing/images/2/25/Gruff_NH.png/revision/latest/scale-to-width-down/350?cb=20200803120221)

{
    "_id" : ObjectId("6101bcc3ad5377c81a8c4623"),
    "acnh" : {
        "name" : "Gruff",
        "type" : "goat",
        "birthday" : "August 29th (Virgo)",
        "nitialPhrase" : "How about this weather, huh? It's like the sun's taken a...shine...to us! You get it? Bleh eh eh!",
        "skill" : "staying up late",
        "goal" : "musician",
        "favoriteSong" : "K.K. Rockabilly"
    },
    "personality" : {
        "personality" : "cranky",
        "interests" : "often challenge the player to various competitions",
        "relationship" : "get along with jock, snooty and other cranky villagers, and occasionally lazy and normal villagers as well"
    },
    "house" : "Gruff owns four different kinds of guitars, a piano, a jukebox, and a bass, which gives his house a rather musical appearance"
}

-------------------------------------------------------------

JSON 6

![img](https://static.wikia.nocookie.net/animalcrossing/images/7/70/Croque_NH.png/revision/latest/scale-to-width-down/315?cb=20200718080111)

{
    "_id" : ObjectId("6101bde3ad5377c81a8c4659"),
    "acnh" : {
        "name" : "Croque",
        "type" : "frog",
        "birthday" : "July 18th (Cancer)",
        "nitialPhrase" : "Hey, you smell that fresh air? Yeah, you should savor that for as long as possible. No, I mean it. I had tacos for lunch. So enjoy the fresh air while you can.",
        "skill" : "staying up late",
        "goal" : "achitect",
        "favoriteSong" : "K.K. Folk"
    },
    "personality" : {
        "personality" : "cranky",
        "interests" : "enjoy spreading rumors about other villagers.",
        "relationship" : "get along with jock, snooty and other cranky villagers, and occasionally lazy and normal villagers as well"
    },
    "house" : "looks much like an autumnal forest"
}

# Passo a passo de manipulação de dados (MongoDB)

## updateDocument

### comandos:

db.getCollection('consultas').update(

​	{

​		"personality.personality":"crancky"

​     },

​	{ $set:

​		{

​			"opinion":"good friend"

​		}

​	},

​	{

​			"multi":true

​	}

)





![updateDocument](https://user-images.githubusercontent.com/82849390/127581457-5ea58f0a-d109-45af-8c5a-36274792a58b.gif)

### 

---------------------------------------------------------

## deleteDocument

### comandos:

db.getCollection('consultas').remove({'acnh.goal':'make up artist'});



![deleteDocument](https://user-images.githubusercontent.com/82849390/127581551-95ac65f8-d3a2-474c-8a31-2059dcc10654.gif)



------------------------------------------------------------

## Projection

### comandos:

db.getCollection('consultas').find({},("acnh.birthday":1,"_id":0))



![projection](https://user-images.githubusercontent.com/82849390/127581584-56fdb759-ea25-4d10-8992-b55786d34b78.gif)







------------------------------------------

## Combinação entre seletores

### comandos:

db.getCollection('consultas').find({ "personality.relationship" : /.*along with jock.*/})

![Igualdade](https://user-images.githubusercontent.com/82849390/127581562-82578933-9b2c-4a72-abbb-13207590bc57.gif)



### comandos:

db.getCollection('consultas').find({$or:[{"personality.personality":/.*cra*./}]})



### comandos:

db.getCollection('consultas').find({"personality.personality":"cranky",
    "villagers":{$gte:3}})



![gte](https://user-images.githubusercontent.com/82849390/127581570-94746186-a27b-421d-9b1f-d607d99c9e85.gif)



--------------------------------------

## Skip, limit e sort

### comandos: 

db.getCollection('consultas').find().skip(2)

![skip](https://user-images.githubusercontent.com/82849390/127581589-66c3a328-0eec-43b2-87b4-562cce78352b.gif)



### comandos:

db.getCollection('consultas').find({}).limit(2)



![limitDocument](https://user-images.githubusercontent.com/82849390/127581578-6886e884-19b5-40cc-982e-46954749a88b.gif)

## comandos:

db.getCollection('consultas').find().sort({"acnh.name":1})



![sortDocument](https://user-images.githubusercontent.com/82849390/127581591-f0869b72-0519-419a-8cce-22a4767e2134.gif)

