# rajkot-tech-latest

> rajkot-tech-latest

## Build Setup

```bash
# install dependencies
$ npm install

# serve with hot reload at localhost:3000
$ npm run dev

# build for production and launch server
$ npm run build
$ npm run start

# generate static project
$ npm run generate
```

# Sample json data
```
{
  "id":1,
  "date":"October 21, 2018",
  "type":"meetup",
  "categories":[
    "laravel"
  ],
  "name":"Laravel: Chapter 1",
  "registrations":19,
  "attendies":15,
  "event_details_url":"https://in.explara.com/e/laravelive-india-rajkot-meetup",
  "live":false,
  "about":[

  ],
  "gallery":"https://drive.google.com/drive/folders/1BaBeAknHLgNb4xF49KA0EwUgxF-Nq8rh",
  "fileName":"laravel-1",
  "coverimage":"",
  "agenda":[
    {
      "title":"Design Patterns in Laravel",
      "type":"talk",
      "speaker":{
        "name":"Siddharth Ghedia",
        "about":"Laravel Developer"
      },
      "twitter":{
        "image":"https://pbs.twimg.com/profile_images/1102889001130704898/VinLm56k_400x400.pn",
        "profile":"https://twitter.com/siddharthghedia"
      },
      "time":"11:00AM"
    },
    {
      "title":"API Development with Laravel",
      "type":"talk",
      "speaker":{
        "name":"Vishal Sancheti",
        "about":"Sr. Software Developer at EYUVA | Volunteer LaravelLiveIN, LaravelRajko, VueRajkot"
      },
      "twitter":{
        "image":"https://pbs.twimg.com/profile_images/1025750323774644225/ojZaE-4g_400x400.jpg",
        "profile":"https://twitter.com/v1shky"
      },
      "time":"12:00AM"
    },
    {
      "title":"Laravel Package Development",
      "type":"talk",
      "speaker":{
        "name":"Gaurav Makheca",
        "about":"Digital Business Builder | Backend Specialist | Speaker | Laravel, Vue.js, API Development, and open source expert | Side project"
      },
      "twitter":{
        "image":"https://pbs.twimg.com/profile_images/1236336194666893312/1PWzvVie_400x400.jpg",
        "profile":"https://twitter.com/gauravmakhecha"
      },
      "time":"10:00AM"
    }
  ],
  "venue":{
    "place":"EYUVA Internet Pvt Ltd",
    "address":"Eyuva Technologies, 402, Rivera Wave Near McDonald's, Kalavad Rd, Laxmi Nagar, Chandreshnagar, Rajkot, Gujarat 360005"
  },
  "volunteers":[

  ]
}
```

# while adding events details read this

    1. date: date when event is going to be held (required)
    2. type: meetup/seminar/event/gathering
    3. category: which category or type meetup belongs to(required)
    4. name: name of the event(required)
    5. registrations: number of registration for the event
    6. attendies: no of people attended the meetup
    7. events_details_url: details events url
    8. live: if event is being held already false otherwise keep it true(required)
    9. about: write few line about the event. what is it regarding?
    10. fileName: add name of event by adding '-' between words. For Eg. Introduction to laravel should be introduction-to-laravel.(required)
    11. coverimage: cover image of event
    12. agenda: this cover the agenda of all speaker
        -title: topic of speaker, regarding waht he.she os going to speak(required)
        -type: talk/mentor
        -speaker:
            -name: name of speaker(required)
            -about: some info about speaker
        -twitter:
            -image: twitter image url of speaker
            -profile: twitter profile of speaker
        -time: time of when he starts delivering his speach(required)
    13.venue:
        -place: place where meetup is organized(required)
        -address: details address of place
    14. volunteers: volunteer's name who helped in organizing this event
    15. gallery: images of event url

# While adding new chapter and their events

$ in '/events' directory add new chapter and events.
$ while adding events of particular chapter, following fields are to added along with other data
 1. category: which chapter particular event belongs
 2. live: true if event is being organized, update value to false after event is over 
 3. fileName: add title of event by adding '-' between words. For Eg. Introduction to laravel should be introduction-to-laravel
