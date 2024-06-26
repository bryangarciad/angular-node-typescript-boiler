After cloning, run `npm install`

Run `npm run post-dev` to start the Node server in development mode

Run `npm run start` to spin front end code in a different terminal instance

Navigate to `http://localhost:4200/`. 

You can now seamlessly watch your changes reflect in realtime everytime you hit save (Client + Server code).

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via [Protractor](http://www.protractortest.org/).

## Instructions for the challenge

1. create and endpoint GET /rickandmortyapi/character?page={pageNumber} that retrieve data from https://rickandmortyapi.com, make sure to receive query param page
NOTE: don't call directly from Angular API use node server

Example api call and response

GET https://rickandmortyapi.com/api/character/?page=19
{
  "info": {
    "count": 826,
    "pages": 42,
    "next": "https://rickandmortyapi.com/api/character/?page=20",
    "prev": "https://rickandmortyapi.com/api/character/?page=18"
  },
  "results": [
    {
      "id": 361,
      "name": "Toxic Rick",
      "status": "Dead",
      "species": "Humanoid",
      "type": "Rick's Toxic Side",
      "gender": "Male",
      "origin": {
        "name": "Alien Spa",
        "url": "https://rickandmortyapi.com/api/location/64"
      },
      "location": {
        "name": "Earth",
        "url": "https://rickandmortyapi.com/api/location/20"
      },
      "image": "https://rickandmortyapi.com/api/character/avatar/361.jpeg",
      "episode": [
        "https://rickandmortyapi.com/api/episode/27"
      ],
      "url": "https://rickandmortyapi.com/api/character/361",
      "created": "2018-01-10T18:20:41.703Z"
    },
    // ...
  ]
}

2. Create one or more components to display results (paginated) use images ui folder for UI reference