# Teaching tips and tricks
The main goal is to inspire other teachers and share information about how to give a fun class.

## Contents:
- Energizers:
    + [Unique game](#any-module---energizer-unique-game-can-be-used-as-intro-getting-to-know-each-other)
    + [One lie two truths](#any-module---energizer-one-lie-two-truths-can-be-used-as-intro-getting-to-know-each-other)
- Module specific tips:
    + [CLI - Game: I go on holiday and I take with me](#cli---game-i-go-on-holiday-and-i-take-with-me)
    + [JavaScript: `map` `filter` `=>`](#javascript-map-filter-)
    + [JavaScript OOP: build a IMDB web scraper with real time code collaboration](#javascript-oop-build-a-imdb-web-scraper-with-real-time-code-collaboration)
    + [React - drawing components](#javascript-oop-build-a-imdb-web-scraper-with-real-time-code-collaboration)
    

# Energizers:
> the goal of energizers is to have a small break while seeing similarities between students. And have a quick laugh.

## Any module - Energizer: Unique game (can be used as intro 'getting to know each other')
*By Daan* 

Everybody stands up, has to tell something about himself that is unique, if someone else in the group has the same unique thing the person who said it needs to sit down and does not participate in the game any more. The game is that whoever stands up last wins the game. To make the games shorter you can let the sitting down students still "participate" if they have something in common with one of the students that are still in the game they can still kick someone out of the game.

## Any module - Energizer: One lie two truths (can be used as intro 'getting to know each other')
*By Mauro* 

Everyone stands up. Everyone tells three things about him or herself. Two out of three have to be true, one is a lie. The group has to guess which one of the three is a lie.


# Module specific tips:
> These tips can of course be used in multiple modules, they are more about different ways you can interact with your class and make your students involved and participate. 

## CLI - Game: I go on holiday and I take with me
*By Unmesh*, 

"I go on holiday and I take with me" with CLI commands from the week before. They have to repeat the commands said before them. add a new command and explain what it does. let the round continue twice otherwise the students that went first don't have to repeat all the commands.

## JavaScript: `map` `filter` `=>`
*By Joost* 

All students write a little JSON-object for themselves. for example:

```js
{
  "name": "Joost",
  "age": 34,             // Hierover mochten ze liegen :-)
  "livedIn": [
    {
      "country": "The Netherlands",
      "town": "Groningen"
    },
    {
      "country": "The Netherlands",
      "town": "Delft"
    },
    {
      "country": "Canada",
      "town": "Montreal"
    }
  ]
}
```

you can build a small webapp. where they can send in the JSON. you can download all objects as an array. and than you can procces the array with `map`and `filter`. First you can filter out the invalid input, for example people who have put their age in a string, or people who have only filled in one town.

## JavaScript OOP: build a IMDB web scraper with real time code collaboration
*By Mauro* 

Start of by letting them all install Atom so they can have live screen sharing and editing. make sure everyone has atom [pair installed](https://atom.io/packages/atom-pair)

The teacher can start of with live coding and explanation. In the second part of the day we ask students to participate in pairs. They form a team, one is the driver and the other students tells him what to code. The idea is that they add a piece of functionality to the code made in the first half of the class. All of this is of course shown live on the screen in front of the class.

for example:
```js
class Actor{
  constructor(name = ''){

  }
}
```

```js
class Movie{
  constructor(title ='', actors =[]){
  this.title = title
  this.actors = actors
  this.finish = false
  this.startDate = new Date()

  }
  addActor(actor){
    if (actor instanceof Actor){
      return this.actors.push(actor)
    }
  }
}

const Ocean11 = new Movie('Ocean11', [Clooney])
```

## React - drawing components
*By Joost and Spyros* 

Draw a sketch of the final app on the flipover, and then students took turns in taking a colour pen drawing boxes around what they considered a component. When we were done with that, we draw a component tree hierarchy. This helped a lot when explaining the input (props) and output (prop handlers) of each component with arrows. Also helped a lot with explaining the data flow between components. What we found handy is that one of us was working with the computer, writing code, explaining the concepts by building an example app, while the other was drawing on the flipover explaining mostly the design decisions we made during the class.
