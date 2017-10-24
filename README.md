# [Libre Projects](http://libreprojects.net)
**open source hosted web services**

 * **open-source** downloadable free software
 * **web-based & hosted** and with a gratis plan
 * **usable** easy to use for everyone

Collecting them makes it easy to find available projects to use and contribute to – both users and developers profit from that. Everyone can help improve these services, not only by coding or translating but also by using and spreading the word.

Not every project will be listed here, especially not complicated ones. It’s not about giving many choices, it’s about providing the best solutions.

## Adding new projects

When adding new projects, please consider the following guideline:

 * Editing the file `js/data.json`
  * Add project alphabetically within its category
  * Add new line like: ` {"id":"PROJECTNAME","category":"..","name":"..","description":"..","address":"https://..","licenses":["..", ..],"tags":["..", ..],"alternative":["..", ..],"introduction":"..","source":"https://.."},`
  * `id`, `category`, `name`, `description`, `address`, `licenses`, `introduction`, `source` are mandatory
  * For `category`, `licenses` and `alternative`, use names defined in (same) `js/data.json` at the top
   * If the corresponding name isn't defined yet, just add it in the same commmit
   * Keep the `description` very short (possibly less than 20 letters), as it'll be directly displayed on the logo upon mouse-hover; the long description goes in `introduction` (copy some appropriate text from the project site)
 * Adding a logo `logos/PROJECTNAME.png`
  * Always quadratic, transparent png
  * Take the existing logo images as examples
  * Even if there's no logo image provided by the project, a meaningful logo image is necessary, as there's no fall-back feature.
   * You can at least take a screenshot of the project name, if there's a nicely styled website with specific fonts and colors.
  * Ideal size is 160 px×160 px and never bigger
  * (Near-) quadratic or round logos (and everything in-between) shall be best resized to 128 px×128 px and centered in a 160 px×160 px canvas 
  * Sparse (mostly transparent, e. g. letters) logos shall be best resized to the maximum size that fits in 160 px×160 px
  * If the logo is very lengthy (like ratio > 3:1), you can consider:
   * Cutting off the letters and just taking the figure in the logo
   * Cutting the text apart where appropriate and wrapping around
 * One commit message for a new project (so that the history remains slim and esp. the rss feed is kept nice)
  * Don't mix irrelevant changes in the commit, but just add the necessary things for the new project
  * First line of commit message: `New project: PROJECTNAME #THE_CORRESPONDING_ISSUE` (additional notes can be added as appropriate)
  * Optionally write more details in the following lines (source etc.)

