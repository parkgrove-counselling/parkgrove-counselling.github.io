
- use landscape background photo for mobile

- fix width issue
- change colour of "KATIE THOMPSON" at top of page
- alter hover over links colour
- add qualification icons
- remove links at bottom


To run hugo on local network:

```shell
hugo server --bind=0.0.0.0 --baseURL=http://192.168.1.95:1313 -D
```

convert image size
https://imagemagick.org/Usage/resize/#noaspect
```shell
convert katie-left-orig.jpg  -resize 800x533 katie-left.jpg
# convert a square image to rectangular
convert online-counsellor-150x150.png -resize 150x150^ -gravity center -extent 300x150 online-counsellor-350x150.png
```

https://github.com/parkgrove-counselling/hugo.git

Hosted
: https://app.netlify.com/sites/eclectic-capybara-5e75c2/settings/deploys


