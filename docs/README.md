# How to update Issie website

## Content of pages

- The content of each page is in its markdown (.md) file:
  1. [index.md](index.markdown) (Home Page)
  2. [userGuide.md](userGuide.md)
  3. [devInfo.md](devInfo.md)
  4. [contact.md](contact.md)
  5. [download.md](download.md)

- The images used in the above .md files are placed in the [img](img/) folder.

- The content of `Key Features` in the Home Page is built using the [module.html](_includes/module.html) in the `_includes` folder
  - See pre-existing code in [index.md](index.markdown) for how to use this include.  

## Blog

- To add a new blog post:
  - Add a new file with the format `YYYY-MM-DD-name-with-dashes.md` in the _posts folder
  - Add the necessary information at the header:
    - `---`
    - `layout: post`
    - `title:  "{YOUR TITLE}"`
    - `date: {YYYY-MM-DD HH:MM:SS +TIMEZONE}`
    - `categories: Issie Blog`
    - `--- `
  - Add the content of the post below the header
  - Let Pagination do its magic
- To change number of posts per page in the main blog page:
  - Change `paginate: 3 ` to the number you like in [_config.yml](_config.yml)


## Styling

- Style is based on the GitHub pages `Architect theme`
- Local changes are in the [style.scss](assets/css/style.scss) file

## Layouts

- The 4 layouts used: `default.html` (for home page), `page.html` (for other pages), `blog.html` and `post.html` are all in the [_layouts](_layouts/) folder.
- Images used in layouts are in the [images](assets/images/) folder