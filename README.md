# Twitter::Colour::Picker
<p align="center">
![alt tag](https://lh3.googleusercontent.com/-cT0tI6qB43M/VweT2VMAk2I/AAAAAAAAAbw/E1BBFI81KkMU2oAxRhcQSS8YoDh78eabwCCo/s144-Ic42/Screen%2BShot%2B1395-01-20%2Bat%2B15.17.26.png = 250x250)
</p>
## Installation

1.Add gem 'twitter-colour-picker' to your Gemfile.

```ruby
gem 'twitter-colour-picker'
```

2.And then execute:
```bash
    $ bundle install
```
Or install it yourself as(local):
```bash
    $ gem install twitter-colour-picker
```
## Usage


| Format | Require |
| --- | --- |
| CSS |  *= require colour-picker |
| JS | //= require colour-picker |


choice color on controller :
```ruby
#flat colors , source https://flatuicolors.com/
@colors = ["3097d1","1abc9c", "2ecc71","3498db","9b59b6","34495e","f39c12","d35400","c0392b","bdc3c7","7f8c8d","f1c40f"]
```
views:
```html
<select id='theme_color' style="display:none;">
<% @colors.each do |color|%>
<option value="<%= color %>"><%= color %></option>
<% end %>
</select>

```
OR:
```ruby
 <%= form.select(:theme_color, options_for_select(@colors, selected: 'user selected'),{},{:class=>"...",:id=>'theme_color',:style=>'display:none;'}) %>
```


```javascript
<script>
$(document).ready(function(e){
$('#theme_color').colorpicker({
size: 35,
label: 'Theme Color: ',
hide: false
});
});
</script>
```

## Contributing

For reporting bug, contact me on [twitter](https://twitter.com/mm580486)


## License

Copyright (c) 2015 [Mohammad Mahmoudi](https://twitter.com/mm580486).