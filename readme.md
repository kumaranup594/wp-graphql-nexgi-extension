# wp-graphql-nexgi-extension

I develop headless wordpress blogs using nextjs & gatsby and use graphQL as flexible data fetching. For that I'm using wp-graphQL official plugin.

## Dependiencies 
- <a href="https://github.com/wp-graphql/wp-graphql" target="_blank">wp-graphql wordpress plugin github</a>

## Features
### Total number of posts, pages count in graphQL wordpress

#### feature information
Added an options to get total number of posts, pages or any custome post type of wordpress using grpahQL. This originally given <a href="https://gist.github.com/jasonbahl/d2dfe0c56390e9c9c8b0c25d7d6c4bd2" target="_blank"> here </a>. But here I coveted into wordpress graphQL plugin.

#### How to use it
Total number of pages

```graphql
{
  pages{
    pageInfo{
      total
    }
  }
}

```
Response

```yaml
{
  "data": {
    "pages": {
      "pageInfo": {
        "total": 14
      }
    }
  }
}
```



Total number of posts

```graphql 
{
  posts{
    pageInfo{
      total
    }
  }
}
```

Response

```yaml
{
  "data": {
    "posts": {
      "pageInfo": {
        "total": 14
      }
    }
  }
}
```


