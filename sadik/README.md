# Sadik 🌲🚗 (صديق = friend)

Carpooling to USJ: drivers offer their empty seats, classmates find a ride from their area and join in one tap.

## Links
- **App (phones):** https://edwinuniv.github.io/sadik/
- **Big screen (projector):** https://edwinuniv.github.io/sadik/?screen

## The app
- **First visit:** 4 quick questions (first name, area, usual time, do you drive).
- **Find:** rides from your area at your time, plus other times and all areas. No match? *Ask for a ride* and drivers see it.
- **Offer:** pick area, time, free seats and a meeting point, then publish.
- **Ride page:** join or leave (seats can never be double-booked), see who's in the car, and use the car's group chat.
- **My rides / Me:** your rides, your requests, your profile, and Sadik Plus.
- **Sadik Plus ($2/month, demo only, no real payment):** fuel-split calculator, verified-only filter, keep your seat Mon–Fri, ride reminders.

## The big screen (`?screen`)
- **Live board:** QR code, live stats, departures board, a schematic map of where people come from, who's still looking for a ride, and a live activity strip.
- **Join here:** a phone on the screen for anyone without a phone. Tap "↻ Next person" between people.
- **Tools:** *Simulate* adds one realistic action, *Auto demo* runs on its own, *Reset all* (click twice) clears everything.

## Testing tips
- Add `?demo` to run on this computer only, without touching the real database.
- Add `&as=name` to act as a different person in the same browser, e.g. `?demo&as=karim`.

Data is stored in Firebase Realtime Database (project `sadik-1f990`) under `v2/`.
