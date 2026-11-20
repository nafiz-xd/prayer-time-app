# Prayer Time — Dhaka

A serene single-page app showing today's five prayer times for Dhaka with a live next-prayer countdown, the Hijri date, and a sun-arc of the day.

Live demo: https://nafiz-xd.github.io/prayer-time-app/

## Features

- Today's five prayers for Dhaka — Fajr, Dhuhr, Asr, Maghrib and Isha — plus Sunrise, from a built-in monthly timetable (12 months of anchor times, linearly interpolated by day-of-month so the times shift smoothly through the year)
- Current prayer highlighted, next prayer marked, with a live countdown ticking every second (after Isha it counts down to tomorrow's Fajr)
- Hijri date shown using the browser's built-in Islamic calendar (`Intl.DateTimeFormat` with `en-u-ca-islamic`) — no library or API needed
- Sun-arc visual: an SVG arc from Fajr to Maghrib with a glowing sun dot positioned by the current time and a daylight-progress percentage
- Ramadan banner that appears automatically when the Hijri month is Ramadan (month 9), showing the Maghrib / Iftar time
- Serene emerald-and-gold design with a mosque-skyline silhouette, soft fade/rise animations, and a fully mobile-responsive layout
- Completely static — no accounts, no API keys, no backend; works from `file://` and GitHub Pages alike

## Tech Used

- HTML5
- CSS3 (custom properties, keyframe animations, inline SVG mosque skyline and sun-arc)
- Vanilla JavaScript (monthly timetable interpolation, `setInterval` countdown, `Intl.DateTimeFormat` Islamic calendar)

Built by Nafiz Bin Azad
