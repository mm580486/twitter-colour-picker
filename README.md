# Twitter::Colour::Picker

![alt tag](https://lh3.googleusercontent.com/-cT0tI6qB43M/VweT2VMAk2I/AAAAAAAAAbw/E1BBFI81KkMU2oAxRhcQSS8YoDh78eabwCCo/s144-Ic42/Screen%2BShot%2B1395-01-20%2Bat%2B15.17.26.png)

## Installation

1.Add gem ```ruby gem 'twitter-colour-picker' ``` to your Gemfile.

```ruby
gem 'twitter-colour-picker'
```

2.And then execute:

    $ bundle install

Or install it yourself as(local):

    $ gem install twitter-colour-picker

## Usage
css:
 *= require colour-picker
js:
//= require colour-picker

choice color on controller :
@colors = ["3097d1","1abc9c", "2ecc71","3498db","9b59b6","34495e","f39c12","d35400","c0392b","bdc3c7","7f8c8d","f1c40f"]

views:
```ruby
<select id='theme_color' style="display:none;">
	
<% @colors.each do |color|%>

<option value="<%= color %>"><%= color %></option>
<% end %>
</select>

OR:
 <%= form.select(:theme_color, options_for_select(@colors, selected: 'user selected'),{},{:class=>"...",:id=>'theme_color',:style=>'display:none;'}) %>




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

# twitter-color-picker
