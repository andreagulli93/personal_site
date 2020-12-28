# Project: Personal site [(link)](https://antoniosfiala.github.io/personal_site/)
Making a little website, a digital business card, that can connect people to various social networks where people can find more information or get in touch.

## Approach & purpose of project
- Use open-source templates and resources
- Amend only what is required to make it 'my own'
- Generalise code to allow for easy extendability in the future
- Create detailed documentation here on GitHub
- Practice using GitHub
- More documentation [here](#Documentation)

## Mini architecture
The interaction of the various components and code-bases of the project.
[Image link](https://viewer.diagrams.net/?highlight=0000ff&edit=_blank&layers=1&nav=1&title=Site_architecture.drawio#R7ZjJbtswEIafxscG2qMcHdmJUSRtURVoemSksUSUFgWK3vL0HVrU7jgL0jhFbR%2FM%2BTlcxO8nRXhkB4vNtSB5estjYCPLiDcjezKyLNM0PPxRyrZULi7OSyERNNZJjRDSB9CiodUljaHoJErOmaR5V4x4lkEkOxoRgq%2B7aXPOuqPmJIGBEEaEDdWfNJZpqfrWeaPPgCapHtk19LwXpMrVQpGSmK9bkj0d2YHgXJalxSYAptauWpay3dUjtfW8BGTyOQ224cOXr1Nq%2BUUxnbrB9ys5WX%2Fyy15WhC31844sj2F%2Fl%2FdYSFThmsrZEiMj5YWkWVIl4Eh1jn5Cua1WTfBlFoMa2cTqdUolhDmJVO0afYJaKhdMV895JjV401ExZSzgjItdX%2FbcVV%2FUCyn4b2jVeLuP7qGllx%2FUCaNJhlqEawRYebkCISnCHesKyfN6%2BqoONo%2BurlkzQ68DX4AUW0zRDSzbKZtom%2Fua%2BrrxjO1pLW35xa58TrRPk7rrhiUWNM4XoDUHaMdnGM9%2B3N68MS4V677MIb7YBT929uHzrXt7h6%2FCxGCu3FTg0Gi0m100wQV6G0Jul1B9wrQQmdYeRN7fImQNCAWKUBCG%2FyUg58MBsgeALhWgz2RFwkjQXL4vJwL%2BPNp7DkY%2B3M%2BPxck8OidnwGmiOI2LAmRx2kvt18zRGLl7bho9MJDFY3VjUy9sRoqCRl0WsKHyDsuGLv9S5TNXR5NNq2qyrYIMJ39XdaCCVisVNs12UdXuMPfdzCEe3Bx7ePDp%2BFJE8LR1JREJyKfe5kPcLZzuHpqVJoARSVfd6e5DrEf4xik%2BSOMmo%2Bsmp%2B%2BS8jF1q%2FYdtN9Rz5ZO%2F%2FZTrsOgI7QF2bbScpVQHJiw2bO%2FYxyeVy%2Ff6uZjoZxBY%2F%2Bawet3hHfaEQduRR98R3g9g7mv3BG233Nev6MX74jOKf0GNj0%2F2fTA3fDfsunAXcez6fMOYvN9D24Mmz9kyvTmXy17%2Bgc%3D)
<div class="mxgraph" style="max-width:100%;border:1px solid transparent;" data-mxgraph="{&quot;highlight&quot;:&quot;#0000ff&quot;,&quot;nav&quot;:true,&quot;resize&quot;:true,&quot;toolbar&quot;:&quot;zoom layers lightbox&quot;,&quot;edit&quot;:&quot;_blank&quot;,&quot;xml&quot;:&quot;&lt;mxfile host=\&quot;Electron\&quot; modified=\&quot;2020-12-28T21:00:17.832Z\&quot; agent=\&quot;5.0 (Macintosh; Intel Mac OS X 10_16_0) AppleWebKit/537.36 (KHTML, like Gecko) draw.io/13.9.9 Chrome/85.0.4183.121 Electron/10.1.5 Safari/537.36\&quot; etag=\&quot;yl3-u_FQoUe4-0UW3qq2\&quot; version=\&quot;13.9.9\&quot; type=\&quot;device\&quot;&gt;&lt;diagram id=\&quot;GoY1BE-ZTT2bAoibkE7Q\&quot; name=\&quot;Page-1\&quot;&gt;7ZjJbtswEIafxscG2qMcHdmJUSRtURVoemSksUSUFgWK3vL0HVrU7jgL0jhFbR/M+TlcxO8nRXhkB4vNtSB5estjYCPLiDcjezKyLNM0PPxRyrZULi7OSyERNNZJjRDSB9CiodUljaHoJErOmaR5V4x4lkEkOxoRgq+7aXPOuqPmJIGBEEaEDdWfNJZpqfrWeaPPgCapHtk19LwXpMrVQpGSmK9bkj0d2YHgXJalxSYAptauWpay3dUjtfW8BGTyOQ224cOXr1Nq+UUxnbrB9ys5WX/yy15WhC31844sj2F/l/dYSFThmsrZEiMj5YWkWVIl4Eh1jn5Cua1WTfBlFoMa2cTqdUolhDmJVO0afYJaKhdMV895JjV401ExZSzgjItdX/bcVV/UCyn4b2jVeLuP7qGllx/UCaNJhlqEawRYebkCISnCHesKyfN6+qoONo+urlkzQ68DX4AUW0zRDSzbKZtom/ua+rrxjO1pLW35xa58TrRPk7rrhiUWNM4XoDUHaMdnGM9+3N68MS4V677MIb7YBT929uHzrXt7h6/CxGCu3FTg0Gi0m100wQV6G0Jul1B9wrQQmdYeRN7fImQNCAWKUBCG/yUg58MBsgeALhWgz2RFwkjQXL4vJwL+PNp7DkY+3M+Pxck8OidnwGmiOI2LAmRx2kvt18zRGLl7bho9MJDFY3VjUy9sRoqCRl0WsKHyDsuGLv9S5TNXR5NNq2qyrYIMJ39XdaCCVisVNs12UdXuMPfdzCEe3Bx7ePDp+FJE8LR1JREJyKfe5kPcLZzuHpqVJoARSVfd6e5DrEf4xik+SOMmo+smp++S8jF1q/YdtN9Rz5ZO//ZTrsOgI7QF2bbScpVQHJiw2bO/YxyeVy/f6uZjoZxBY/+awet3hHfaEQduRR98R3g9g7mv3BG233Nev6MX74jOKf0GNj0/2fTA3fDfsunAXcez6fMOYvN9D24Mmz9kyvTmXy17+gc=&lt;/diagram&gt;&lt;/mxfile&gt;&quot;}"></div>
<script type="text/javascript" src="https://viewer.diagrams.net/js/viewer-static.min.js"></script>


## List of tools
- [The Noun Project](https://thenounproject.com) for icons used in the rectangles and the line dividers
- [Pixelmator Pro](https://www.pixelmator.com/pro/) availabe on [MacOS Appstore](https://apps.apple.com/us/app/pixelmator-pro/id1289583905?mt=12)
- [Atom.io](https://atom.io) text editor
  - [Chromo package](https://atom.io/packages/chromo-color-previews) to preview hex colours [GitHub here](https://github.com/Vertagon-Softworks/Chromo)
- [Google Chrome (MacOS)](https://www.google.com/intl/en_uk/chrome/) and Safari (Mac & iOS) for desktop and mobile testing
- Generate colour palette using [coolors.co](https://coolors.co/)
- GitHub markdown cheatsheet [here](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)

---
**Colour-scheme**
- Dark orange: #E36414 ![alt text](https://github.com/antoniosfiala/personal_site/blob/new_code/assets/img/Colours/Dark_orange.png "Dark orange")
- Light Orange: #FB8B24 ![alt text](https://github.com/antoniosfiala/personal_site/blob/new_code/assets/img/Colours/Light_orange.png "Light orange")
- Light Green: #A8C256 ![alt text](https://github.com/antoniosfiala/personal_site/blob/new_code/assets/img/Colours/Green.png "Light green")
- Light Blue: #86BBD8 ![alt text](https://github.com/antoniosfiala/personal_site/blob/new_code/assets/img/Colours/Light_blue.png "Light blue")
- Pacific Blue: #004F62 ![alt text](https://github.com/antoniosfiala/personal_site/blob/new_code/assets/img/Colours/Pacific_blue.png "Pacific blue")

**References**
1. _'Freelance' bootstrap theme [GitHub repository](https://github.com/startbootstrap/startbootstrap-freelancer) under MIT licence_
2. _Base colour based on iPhone 12 Pro, 'Pacific Blue' hex codes found [here](https://colorswall.com/palette/27294/)_
3. _Social network icons using existing code and adding more using raw data at [fontawesome](https://fontawesome.com/icons?d=gallery)_
4. _Colours in GitHub markdown [stackoverflow](https://stackoverflow.com/questions/11509830/how-to-add-color-to-githubs-readme-md-file)_
5. _Centering fixed position text in a div [stackoverflow](https://stackoverflow.com/questions/2861247/center-aligning-a-fixed-position-div)_
---

## Documentation
**A. HTML**
  - Removed code from template that was not required
  - Amended content (text, titles, images (found in 'D. Assets'))
  - Added different line break with icons
  - Amended hover over box behaviour
  - Added extra favicon lines of code

**B. JavaScript**
  - Removed references to unnecessary libraries for contact form
  - Aside from that, code left as is

**C. CSS**
  - Spent majority of my time here
  - Generalised references with variables, particularly for colours
  - Added some new classes for custom text over the interest boxes

**D. Assets**
  - Created a profile picture
  - Downloaded and prepared assets (mainly in .svg) for line breaks
  - Downloaded and created icons for areas of interest using the defined colour pallet only
  - Colours to show in markdown documentation
  - Saved favicon elements here
  - Work_in_progress folder contains the Pixelmator files
