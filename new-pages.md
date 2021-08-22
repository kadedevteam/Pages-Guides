## Creating New Pages!

Go To `assets/` and you should find files known as `tab1`, `tab2` and so on. These Tabs are the website pages! to create a new page, make a folder and call it `tab<numberofpage>` and inside create a `.md` file and name it `tab<number>_stuff_here` and whatever you right will be whats on the page!

### Adding Custom URL Sparks

Create a config.yml file inside of the tab file and write `link: {{ site.url }}/<nameOfUrl>/`!

**NOTE**: You can add more pages to your site by creating more new files. Each file will be available on your site in the same directory structure as your publishing source. For example, if the publishing source for your project site is the gh-pages branch, and you create a new file called `/about/contact-us.md` in the tab file branch, the file will be available at `https://<user>.github.io/<repository>/about/contact-us.html.`

To customize your page even more! Check out the [Assets Guide](https://kadedevteam.github.io/Pages-Guides/assets)
