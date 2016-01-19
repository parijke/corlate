# corlate

A theme created of from the bootstrap theme Corlate. All credits goes to https://shapebootstrap.net/

Setting it up:
There is a theme.yml file containing some info. Tweak these to your needs

Also, add a footer to the app/config/menu.yml file like this
footer:
    - label: Home
      title: This is the first menu item.
      path: homepage
      class: first
    - label: About us
      path: entry/1
    - label: Faq
      path: pages/
    - label: Contact us
      link: http://bolt.cm
      class: last
