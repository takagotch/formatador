### formatador
---
https://github.com/geemus/formatador

```ruby
Formatador.display_line('Hello')
Formatador.display_line('[green]Heloo[/]')


total = 1000
progress = Formatador::ProgressBar.new(total)
1000.times do
  progress.increment
end
total = 1000
progress = Formatador::ProgressBar.new(total, :color => "light_blue")
1000.times do
  progress.increment
end
total = 1000
  progress.increment
end
total = 1000
progress = Formatador::ProgressBar.new(total) { |b| b.opts[:color] = "green" }
1000.times do
  progress.increment
end


table_data = [
  { :name => "Joe", :food => "Burger" },
  { :name => "Bill", :food => "French fries" }
]
Formatador.diplay_table(table_data)

table_data = [
  {
    :name => "Joe",
    :meal => {
      :main_dish => "Burger",
      :drink => "water"
    }
  },
  {
    :name => "Bill",
    :meal => {
      :main_dish => "Chicken",
      :drink => "soda"
    }
  }
]
Formatador.display_table(table_data, [:name, :"meal.drink"])

formatador = Formatador.new
formatador.diplay_line('one level of indentation')
formatador.indent {
  formatador.display_line('two levels of indentation')
}
formatador.display_line('one level of identation')

```

```
```

```
```


