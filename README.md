# srl.io

[![Join the chat at https://gitter.im/jeffmcneill/zns.io](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/jeffmcneill/zns.io?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

meteor-based url shortening service

## Main Features

- No linkrot
- Changeable shorturl or longurl
- Private analytics
- Random or user set URL
- Use own domain (using DNS record A)
- Downloadable links
- Can run on own server (open source)
- Reasonable hosting fee
- Plugins for browsers (like goo.gl button)
- Apps for mobile
- API for programmers to use the service

## Caching Features

- Can serve as a cache engine as well (for qualified users)
- For those who want, a URL will create a cached copy (html, js, css, png, jpg, gif, etc.)
- Items will then be cached at four locations (Tokyo, London, Newark, Fremont) Linode locations using Pound/Varnish, and served using geoscaling DNS at http/s://c.srl.io/xyz
- Need some way of refreshing/flushing the cached objects programmatically (e.g., control Varnish from the shortening app, such as c.srl.io/usr/flush and c.srl.io/xyz-flush)

## Notes

- Aha! Found it <https://github.com/npvn/meteor-url-shortener>
- User account creation/authentication
- Track URLs by user
- Count clicks, and referrers by URL
- Display clicks over time, and also by referrer
- Allow for ?parameters to distinquish URL (and track)
- Ensure unique URL
- Allow (for certain users) manual URL creation and change
- Default behavior is random human-readable creation, using numbers and letters (no il1I,o0O for legibility)
- Maybe look at this one <https://github.com/dotzero/node-url-shortener>
