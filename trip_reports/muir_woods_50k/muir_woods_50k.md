---
layout: default
title: Muir Woods 50k
---

# Muir Woods 50k (May '23)

<figure class="center-figure-big">
    <img src="muir_6.png" alt="Muir Woods 50k Hero Shot">
    <figcaption></figcaption>
</figure>

<p>&nbsp;</p>

Muir woods chill was an impropmtu 50k I ran starting and ending in Muir Woods National Monument in California (~30 min north of San Francisco). The route was great: water along the way, a nice store to stop at half way through (in Stinson Beach), and ocean/forest views the whole way.

Would 100% recommend to anyone looking for a gentle intro to ultrarunning.

## Route

<div id="run-map" style="height: 400px; border-radius: 8px;"></div>

<script>
  // ❶ Create a basic Leaflet map
  const map = L.map('run-map', { scrollWheelZoom: false });

  // ❷ Nice looking base layer (Stamen Toner Lite, free & no key needed)
  L.tileLayer('https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
    attribution:
      '© <a href="https://www.openstreetmap.org/">OpenStreetMap</a> contributors'
  }).addTo(map);

  // ❸ Load the GPX (copy the file into /assets/gpx/)
  new L.GPX('muir_woods_50k.gpx', {
    async: true,
    marker_options: {
      startIconUrl: 'https://unpkg.com/leaflet-gpx@2.1.2/pin-icon-start.png',
      endIconUrl:   'https://unpkg.com/leaflet-gpx@2.1.2/pin-icon-end.png',
      shadowUrl:    'https://unpkg.com/leaflet-gpx@2.1.2/pin-shadow.png'
    },
    polyline_options: {
      color: '#e63946',
      weight: 4,
      opacity: 0.9
    }
  })
    .on('loaded', e => map.fitBounds(e.target.getBounds())) // auto-zoom
    .addTo(map);
</script>

I started at the Muir Woods visitor center and ran through the main park area. There's about 1 mile of nice wood-plank walkways and big redwoods. If you go early in the morning there shouldn't be many people around but after about 10am it's pretty busy. There's also lots of turns and trails in the first mile so it's super easy to take the wrong trail; just follow your map and you should be fine. The next ~5-6 miles are classic Bay Area trail running, with lots of coastal woods and good amount of elevation (~1500 feet of climbing). 

Mile 7.0 is the top of cardiac hill. There's a water fountain up here, and great views of the ocean. I circled back here later in the run. 

Mile 7 to ~10 is mostly cutting across open grassy hills. When I ran it there was thick fog so I couldn't see more than a few hundred feet, but if you hit it on a sunny day you can see all the way back to SF.

Mile 11 to 14 is a steep descent down into Stinson Beach, the one and only town on the route. There is a general store on the corner of the main street in town where. They've got lots of sandwiches and premade food if that's your style. There is a short amount of road running to get out of the town before you're back on trails. I'd actually recommend **not** filling up on water here; instead refill at the top of cardiac hill. 

Mile 14 to 17.5 is  healthy climb back up to cardiac hill (~1000 feet). There's lots of stairs along the route. It's a pretty popular trail so expect lots of traffic. 

Miles 17 to 25 were classic Bay Area trail running. For the later part of this segment, the trail hugs a cliff/hill right above the ocean which is a nice change of pace from the higher ridges from earlier.  

At mile 24.8 I stopped at Pirates Cove for some food I had bought at the general store. If you are willing to hike down a little you can reach the beach. 

The next two miles is wide open pasture; the trail turns into wide fire roads and there's panoramic views. This section of the run is what I picture when I look back on the run.

Mile 27 to 32 is just a slog. The views mostly dissapear; you have to go up and down several small ravines, and spend a lot of time on a nondescript fire road. There's also a brutal ~300 foot hill right at mile 31 which is the last little bit of suffering before the end.

## Getting There

I parked and started my run at the [Muir Woods Visitor Center](https://www.nps.gov/muwo/planyourvisit/index.htm). The drive is ~30 min from SF, ~1 hour from the peninsula. You will lose cell once you get close so make sure you have the adress in navigation before you get too close. 

A few important things to know about parking at muir woods
- You **must** reserve parking ahead of time, no matter when you plan on going. You can purchase passes [here](https://gomuirwoods.com/).
- They are really good about parking. When you show up they'll direct you where to park
- I recommend getting the earliest possible slot (usually 8am). They'll park you right next to the visitor center which is super convinent
- There are public bathrooms and a waterfountain at the visitor center
- I've never been able to get cell anywhere in Muir Woods, so plan on being offline for much of the run. Download your parking ticket ahead of time

## Other Advice

- Weather is generally quite temperate along the coast. Expect fog in the morning which burns off by the afternoon. I've done sections of this route several times and often cardiac hill and the upper ridges are free of fog, while Stinson is totally socked in. Bring a jacket or puffy just in case
- You could also modify this route and start/end in Stinson if you don't want to deal with parking at Muir woods (I thought it was cool to start and finish under the park entrance sign)
- The figure-8 route means if you are hurting at mile 7 or 17 you have a nice, 7 mile down-hill return to the car. This is why I'd recommend this route to anyone looking to get into ultrarunning; there's lots of places to chop mileage off if needed.

## Photos

<figure class="center-figure">
    <img src="muir_1.png" alt="">
    <figcaption>Muir Woods entrance (start/end)</figcaption>
</figure>

<figure class="center-figure">
    <img src="muir_2.png" alt="">
    <figcaption>Trail climbing up to Cardiac Hill (~5 miles in)</figcaption>
</figure>

<figure class="center-figure">
    <img src="muir_3.png" alt="">
    <figcaption>Foggy hillside above Stinson</figcaption>
</figure>

<figure class="center-figure">
    <img src="muir_4.png" alt="">
    <figcaption></figcaption>
</figure>

<figure class="center-figure">
    <img src="muir_5.png" alt="">
    <figcaption></figcaption>
</figure>

<figure class="center-figure">
    <img src="muir_6.png" alt="">
    <figcaption>Trail on the way to Pirate's Cove</figcaption>
</figure>

<figure class="center-figure">
    <img src="muir_7.png" alt="">
    <figcaption>Second stop</figcaption>
</figure>