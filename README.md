# Minicurso Rails Coninfa

## Ruby

### Interactive Ruby

No terminal, execute:

```shell
irb
```

### Tudo é objeto

- Monkey Patch
- Ancestors

```ruby
class Integer
  def odobro
    self * 2    
  end
end
```

```ruby
Integer.class
Integer.class.ancestors
```

## Ruby on Rails

Criando um novo projeto Ruby on Rails.

```shell
rails new nome_do_projeto
```

Nosso projeto será assim:

```shell
rails new contentmaster --css tailwind -d postgresql --skip-kamal
```

- PostgreSQL
- TailwindCSS
- Flags para não adicionar determinadas "peças"

### Criando CRUDS com Scaffolds

- CREATE
- READ
- UPDATE
- DELETE

```shell
rails generate scaffold Publication title content:text
```

### Executar o projeto Rails

Arquivo Procfile.dev

```ruby
web: rails server
css: rails tailwindcss:watch
```

```shell
foreman start -f Procfile.dev
```
