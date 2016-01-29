# corlate

A theme created of from the bootstrap template Corlate. All credits goes to https://shapebootstrap.net/

Setting it up:
There is a theme.yml file containing some info. Tweak these to your needs

Also, add a footer to the app/config/menu.yml file like this
```
footer:
  label: Home
  title: This is the first menu item.
  path: homepage
  class: first
  label: About Us
  path: page/About
  label: Faq
  path: page/faq
  label: Contact Us
  path: page/contact
  class: last
```

For the silder to work, add a contenttype like
```
slides:
    name: Slides
    singular_name: Slide
    fields:
        text1:
            type: text
            class: large
            required: true
        slug:
            type: slug
            uses: text1
        text2:
            type: text
            class: large
            required: true
        bgimage:
            type: image
            attrib: title # Note: retrieve this in your template with {{ record.values.image.title }}
            extensions: [ gif, jpg, png ]
        fgimage:
            type: image
            attrib: title # Note: retrieve this in your template with {{ record.values.image.title }}
            extensions: [ gif, jpg, png ]
    default_status: published
    show_on_dashboard: false
    searchable: false
    viewless: true
```
