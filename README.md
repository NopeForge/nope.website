# README

This is the repository for the website https://www.nopeforge.org.

## Technical summary

- Static website generated with [Hugo](https://gohugo.io)
- No Hugo theme, we are using a vanilla [Bootstrap](https://getbootstrap.com/)
  and setting various classes in the HTML templates

## Common operations

### Testing the website locally

```sh
hugo server -D
```

### Adding a news

1. Create a news file: `hugo new news/my-breaking-news.md`
2. Remove the `draft: true` front-matter entry when satisfied
3. Add the markdown file to git and open a PR

### Deploying the files in production

Generate the files with `hugo` and upload them.

## External assets source and credits

- `features/automation.jpg`:
    + author: Alex Knight
    + https://unsplash.com/photos/2EJCSULRwC8
- `features/cinema-strip.jpg`:
    + author: Павло Павлюк
    + https://unsplash.com/photos/2WAJOSZ4JUE
- `feaatures/code.jpg`:
    + author: Chris Ried
    + https://unsplash.com/photos/ieic5Tq8YMk
- `features/devices.jpg`:
    + author: Mariakray
    + https://pixabay.com/photos/technology-devices-electronics-6801334/
