## What is this

Repo for custom code used in Hidden Reach issues. May be maps, charts, etc. Some code may be better used inline in the issue, but for something with JavaScript interactivity, deploying here and embedding with an `iframe` may work best (e.g. the interactive map in Issue 1).

## To contribute

The `main` branch is deployed to the `github.io` site that is used in production. For development, create a new branch with your initials and the topic:

> `github checkout -b mad/cool-map`

When you're done, create a PR to document what you did and why, squash and merge your changes, and delete your branch.

## Shorthand notes

Once you have the `iframe` in the HTML block, you may need to adjust breakpoints and local styles. You can do that by giving your iframe an `id` and adding some CSS inside a `style` tag in the same HTML block.

## Map notes

Mapbox styles that use data from Mapbox and/or Open Street Maps will require [text attribution](https://docs.mapbox.com/help/getting-started/attribution/#text-attribution) which must appear _in_ the map view (i.e. it cannot be placed at the bottom of the website page). Mapbox will generate this for you and add it to the map. The Mapbox logo is required if you are using Mapbox software and cannot be removed.

If you do _not_ want the text attribution to appear on your map, you can create a map style entirely from scratch using non-Mapbox data. [Natural Earth](https://www.naturalearthdata.com/) is a great place to start. The download will be a `.zip` folder - it's a Shapefile that should be uploaded as-is as a new [tileset](https://docs.mapbox.com/help/glossary/tileset/).
