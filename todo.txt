# Reaction Widget

##API:

- https://public.radio.co/stations/[radio-station-id]/status?v=1753630092000
- https://public.radio.co/api/v2/[radio-station-id]/track/current

## Status:
- submitted

## Description:
Enabling the listeners and creators to interact, sending emoji and comments together with timestamp of reaction to a backend and showing that info on the website.
 
## Future improvements:
- start time detection
  - as we are polling the api to detect title changes, it could also be used to the start time, improving the reaction time value
- instant reactions by clicking just emoji ?
- animated/highlighted reaction list depending on reaction time
- super reactions (?)
- using the current-track api to detect title changes
  - https://public.radio.co/api/v2/[radio-station-id]/track/current
- the way the widget is embedded into the page is suboptimal as it is inside an iframe.
  - better: include it directly into the website
    - could hook into player events referring to their api here:
      - https://www.radio.co/api?srsltid=AfmBOoqBQ22gsCzdGEU_felv-XKkOs3g-d_Df4gOGhx2HixuzK9Ur1JC
  - if not possible, we could move the code completely to the backend server. As it is an iframe already, that should be no problem and enables updates of the widget without changes on the actual radio website.

--------------------------

# History Widget

## Status:
 - draft

## Description: 
Showing the titles of played songs as history (max 19)

## API: 
https://public.radio.co/stations/[radio-station-id]/status?v=1753630092000


--------------------------

Upcoming Widget

API: https://public.radio.co/api/v2/[radio-station-id]/track/next

Status:
- draft

Description:
It would be nice to see, which title comes next.
Sadly the API delivers no info about that currently.


--------------------------

Embeddable Radio status widget for other websites or streams

Status:
- draft

Description:
I would like to show whats playing on the radio on my twitch stream or my homepage to promote aiu.fm  .. The idea is to create a little Website which contains just some info about the current status (onair or not), the current playing song title and maybe a bit of history of the former played songs, maybe 1-3 titles.
With OBS broadcasting app one could include a browser element into the stream that shows this little website.
