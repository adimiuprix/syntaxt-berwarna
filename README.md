## Membuat syntax highlight

Ini adalah tutorial membuat agar code memiliki penyorotan warna agar tidak monoton.
Proyek ini menggunakan salah satu library javascript yaitu [Highlight.js v11.7.0](https://highlightjs.org/)

## Getting started

- Jika kalian ingin mengunduh library ini silahkan pergi ke [highlightjs][https://highlightjs.org/]
- salin di root atau di mana proyek kalian berada.
- panggil file [highlinght.js] dan [styles] ada banyak style yang dapat di gunakan, semua ada di folder [styles]

## Small example

```
<!DOCTYPE html>
<html>
    <head>
        <link rel="stylesheet" href="styles/tokyo-night-dark.min.css">
    </head>
    <body>
        <pre>
            <code>
                # The Greeter class
                class Greeter
                  def initialize(name)
                    @name = name.capitalize
                  end
                
                  def salute
                    puts "Hello #{@name}!"
                  end
                end
                
                g = Greeter.new("world")
                g.salute
            </code>
        </pre>
        <script src="highlight.min.js"></script>
        <script>
            hljs.highlightAll();
        </script>
    </body>
</html>
```

- semua yang ada di dalam tagg ```<code>``` akan di ubah dengan javascript