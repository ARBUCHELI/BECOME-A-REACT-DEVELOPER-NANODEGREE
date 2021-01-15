# BECOME-A-REACT-DEVELOPER-NANODEGREE

## This repository contains exercises from Become a React Developer Udacity's Nanodegree Program. 

# REACT FUNDAMENTALS

## Lesson 01: Why React?

### What is Declarative Code?

Is the following code imperative or declarative?

```html
const people = ['Amanda', 'Geoff', 'Michael', 'Richard', 'Ryan', 'Tyler']
const longNames = people.filter(name => name.length > 6)
```

SOLUTION:
Declarative

### Unidirectional Data Flow

A FlightPlanner component stores the information for booking a flight. It also contains DatePicker and DestinationPicker as child components. Here's what the code might look like:

```
<FlightPlanner>
  <DatePicker />
  <DestinationPicker />
</FlightPlanner>
```
If this were a React application, which component(s) should be in charge of making updates to the data? Check all that apply.

 
* FlightPlanner

 
* DatePicker

 
* DestinationPicker

SOLUTION:
`FlightPlanner`
_________________________________________________________________________________________________________________________________________________________________________________

If the following sample code were a React application, which of the following components should be in charge of making updates to data? Check all that apply.

```
<FlightPlanner>

  <LocationPicker>
    <OriginPicker />
    <DestinationPicker />
  </LocationPicker>

  <DatePicker />

</FlightPlanner>
```
 
* FlightPlanner

 
* DatePicker

 
* LocationPicker

 
* OriginPicker

 
* DestinationPicker

SOLUTION:
`FlightPlanner`
`LocationPicker`


### React is just JavaScript

### .map() Quiz
Use the provided music data array and the .map() method to create a new array that contains items in the format:

<album-name> by <artist> sold <sales> copies
Store the new array in an albumSalesStrings array. So the first item in the albumSalesStrings array should be "25 by Adele sold 1731000 copies"

```
/* Using .map()
 *
 * Using the musicData array and .map():
 *   - return a string for each item in the array in the following format
 *     <album-name> by <artist> sold <sales> copies
 *   - store the returned data in a new albumSalesStrings variable
 *
 * Note:
 *   - do not delete the musicData variable
 *   - do not alter any of the musicData content
 *   - do not format the sales number, leave it as a long string of digits
 */

const musicData = [
    { artist: 'Adele', name: '25', sales: 1731000 },
    { artist: 'Drake', name: 'Views', sales: 1608000 },
    { artist: 'Beyonce', name: 'Lemonade', sales: 1554000 },
    { artist: 'Chris Stapleton', name: 'Traveller', sales: 1085000 },
    { artist: 'Pentatonix', name: 'A Pentatonix Christmas', sales: 904000 },
    { artist: 'Original Broadway Cast Recording', 
      name: 'Hamilton: An American Musical', sales: 820000 },
    { artist: 'Twenty One Pilots', name: 'Blurryface', sales: 738000 },
    { artist: 'Prince', name: 'The Very Best of Prince', sales: 668000 },
    { artist: 'Rihanna', name: 'Anti', sales: 603000 },
    { artist: 'Justin Bieber', name: 'Purpose', sales: 554000 }
];

const albumSalesStrings = musicData.map(album => `${album.name} by ${album.artist} sold ${album.sales} copies`);

console.log(albumSalesStrings);

```

### .filter() Quiz

Use the provided music data array and the .filter() method to create a new array that only contains albums with names between 10 and 25 characters long. Store the new array in a variable called results.

/* Using .filter()
 
 Using the musicData array and .filter():
   - return only album objects where the album's name is
     10 characters long, 25 characters long, or anywhere in between
   - store the returned data in a new `results` variable
 
   Note:
   - do not delete the musicData variable
   - do not alter any of the musicData content
 */

```
const musicData = [
    { artist: 'Adele', name: '25', sales: 1731000 },
    { artist: 'Drake', name: 'Views', sales: 1608000 },
    { artist: 'Beyonce', name: 'Lemonade', sales: 1554000 },
    { artist: 'Chris Stapleton', name: 'Traveller', sales: 1085000 },
    { artist: 'Pentatonix', name: 'A Pentatonix Christmas', sales: 904000 },
    { artist: 'Original Broadway Cast Recording', 
      name: 'Hamilton: An American Musical', sales: 820000 },
    { artist: 'Twenty One Pilots', name: 'Blurryface', sales: 738000 },
    { artist: 'Prince', name: 'The Very Best of Prince', sales: 668000 },
    { artist: 'Rihanna', name: 'Anti', sales: 603000 },
    { artist: 'Justin Bieber', name: 'Purpose', sales: 554000 }
];

const results = musicData.filter(data => data.name.length >= 10 && data.name.length <=25);

console.log(results);
```




# Adaptation as a repository: Andrés R. Bucheli.
