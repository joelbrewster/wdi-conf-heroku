# WDIConf 2016

## [Working Link 01/08/2016](https://wdi7-conf.herokuapp.com/)

### Team Members

It was a pleasure working with these gents:
- [Chris McCorry](https://github.com/ctrlaltchris)
- [Jason Low](https://github.com/jasonlow90)
- [Joel Brewster](https://github.com/joelbrewster)
- [Peter Daniel](https://github.com/peterdaniel-fewd)
- [Will Guan](https://github.com/guanwill)

My profile:
- [Niall O'Callaghan](https://github.com/noccer)

## Workload
### Pre rails (Partials and Static Layout).
- Divided up sections for the hero, information, booking, project sections and a booking page.
- Drew up layouts on whiteboard, and divided up partials to work on.

#### Whiteboard brainstorming
![Role deligation](./app/assets/images/layout1.jpg)
![Initial layout overview](./app/assets/images/layout2.jpg)
![Booking page idea](./app/assets/images/layout3.jpg)
![Model brainstorm](./app/assets/images/layout4.jpg)
![Model brainstorm](./app/assets/images/layout5.jpg)
![File tree](./app/assets/images/layout6.jpg)
![Bootstrap style layout](./app/assets/images/layout7.jpg)
![Booking page ideas](./app/assets/images/layout8.jpg)
- Layout done in Balsamiq.

#### Balsamiq layout
![Balsamiq layout](./app/assets/images/balsamiq.jpg)

### Git control
- Decided on having a gitlord with forked projects that would send pull requests to minimize merge problems.
- Added rails project.
- Added partials.
- Fixed up gitignore.
- Added css.
- Added javascript libraries.

### Rails, database and backend
- Added presenter models, routes and database.
- Added date information to the databse.
  - We added a countdown timer to the event from a date set in the database
```
puts Time.new(2016, 07, 17, 10, 0, 0, "+10:00")
```
- Added gem annotate.
```
Annotates Rails/ActiveRecord Models, routes, fixtures, and others based on the database schema.
```
- Project time examples from [Stack overflow](http://stackoverflow.com/questions/5474164/rails-seeding-database-data-and-date-formats).

```
startDate  => DateTime.new(2009,9,1,17)
```
- For the countdown timer we used [Countdown.js](http://countdownjs.org/).
- Used [this reference](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date/parse) to parse a string into a date object.
- Rails doesnt render the line breaks automatically. We used a [text helper](http://api.rubyonrails.org/classes/ActionView/Helpers/TextHelper.html).

```
<td> <%= simple_format(project.project_description) %></td>
```

`simple_format`
allows you to take line breaks from database (`\n`) and it renders `<br>` tags instead.

### Google Maps integration
- Created a hardcoded address map with google maps from [google developers documentation](https://developers.google.com/maps/documentation/distance-matrix/intro#DistanceMatrixResponses).
- Wanted to remove the [map navigation elements](https://developers.google.com/maps/documentation/javascript/examples/control-disableUI) and add the map direction section to the bottom of the page.

### CSS Frontend
- Added a carousel at the top of the page to display different parts of each project.
- Added hero css.
- First version wifreframes done up in bootstrap.
- Used css keyframes to make neon heading
- Decided to change the sponsors icons to load from grayscale initially to colored on mouse hover.
- Changed using wider logos with text (different width too) to just using squared logos.
- Added some images from [here](https://www.behance.net/laylow) to link with the synthwave/synthpop/cyberpunk theme.
- Added [https://codepen.io/simeydotme/pen/jgcvi](glitter) style overlay to player image profiles because glitter is awesome.
- Added a [http://codepen.io/SitePoint/pen/MwNPVq](javascript countdown clock) in the navbar partial.
- Added a countdown clock to the hero page.

#### Project Quips

##### Queuer
```
Queuer is a restauraunt & cafe waiting app taking the catering and hospitality world by storm.

The average person will spend 6 months of their life in some form of a queue, from traffic lights to supermarkets to cafes.

With over 28,000 venues across 43 countries, people of the world are finally winning back their precious time thanks to Queuer.

A Melbourne based success story, Queuer is a Queue Cure™ that waits in line for you, so you can get busy doing other fun stuff!
```

##### Pulse Express
```
With Pulse express, it's easy to find the right music to sex up your screen. Just press play!

There are millions of sexy singles near you using Pulse Express. So whether you're working out in front of your computer, partying or relaxing in front of your computer, the sexy screen and music is always at your fingertips. Choose what you want to listen to and like, just look at the screen...

You can also browse through the music collections of friends because we haven't got oath working with that.

Soundtrack your life with Pulse App. Log in with github.
```


### Layouts
- Opted for a single page layout (minus the booking page) with a static header.
- Divided the index page into partials and divvied up the front end to a few members.

### Resources
- Took profile pictures, resized, compressed and converted to black and white.
- First logo done in Sketch.

### Technologies
- Rails
- Javascript
- CSS

### Resources
- Added profile pictures.
- Added project carousels with profile overlays.


## Seed brainstorming
- Had the presenters as arrays initially then changed them to objects.
- Thought about changing the presenter_skills to seperate objects later if we have time.

## Branding brainstorming
![First logo](./app/assets/images/WDICONF.png)
