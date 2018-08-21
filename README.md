# Paginator : Simple PHP Pagination tool

## Table of Contents

- [Background](#background)
- [Install](#install)
- [Usage](#usage)
- [Contribute](#contribute)
- [License](#license)


## Background

### At Beginning

For a project where I couldn't use framework, I needed a very simple pagination tool for a blog post list. Classic scheme.
My project use a very basic MVC model, with somes class  to manage entities and controllers. ([you can find it here](http://github.com/David-Evan/oc-wdj-project-8))

But when I finished to create my blog, and I wanted to add pagination system for my index page. 

I had 2 problems : 

- **First** : I couldn't find easy tools to paginate my posts, with customize UI facilities
- **Second** : I didn't want to create pagination with SQL Query selection.

 Also, if I'll need to paginate another data, how could I do withn't code duplication, and, with a simple tool to customize my UI, depending pagination (exist before/after ...) ?

 So, I wrote the Paginator.

### The concept

First, we assume that you want a classic pagination system like this one :
 
```
 [<] [...] [c-2] [c-1] [c] [c+1] [c+2] [...] [>]
 (where c = current page)
```

It could be any array, like PDO:FETCH_OBJ / PDO:FETCH_ASSOC or custom data

You can custom this parameters :
- Current page = (default : 1)
- Elements per page = (default : 3)
- Paginator range (default : 2)

Paginator can return data array for current page, page x and answer few question to help in your UI building, like :
- Is current page the last / first one ?
- Can all page before/after range be displayed ?
 So, you just have to put a condition, eg : `if($paginator->nextPageExist())` and it become really easy to customize your UI.

## Install

```
Copy Paginator in your lib folder and add it to your autoloader.
```

## Usage

```

```

## Example of integration

## Contribute

PRs accepted.


## License

[MIT © David Evan.](../LICENSE)
