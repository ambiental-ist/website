# AmbientalIST website
Website for AmbientalIST, made with the Hugo generator.

**PULL REQUESTS ARE WELCOME!**

## Credits
The stylesheet files `bootstrap.css` and `hugo-theme-cleanwhite.css`, which correspond to most of the CSS, were taken from Zhao Huabing's [Clean White Theme for Hugo](https://github.com/zhaohuabing/hugo-theme-cleanwhite), with some slight modifications made afterwards.

Although the layout itself is largely an original work, it borrows some code from the same repository. Every file with shared code is identified as such with a comment notice at the beginning.

## Development
The only software you need to have installed is [Hugo](https://gohugo.io). If you have the permission to change the site, it is recommended that you also install rsync.

To decouple contributions to this repository from regular content updating, subpage data is kept in a separate repository (the templates themselves being here).

**If you don't have access to the separate repository, you can still contribute.**  Simply type either of these commands on the root of the cloned git repo:

`hugo new content sobre/_index.md`

`hugo new content carta-aberta/_index.md`

`hugo new content open-letter/_index.md`

`hugo new content artigos/name-of-your-article.md`

`hugo new content noticias-e-iniciativas/name-of-your-article.md`

And fill in the blank fields of the Markdown file you created, adding images to the `static/img` folder if you plan to use them. That should allow you to do all the testing you want.

If you have access to the separate repository and want to update content, be sure to merge it in your machine with this cloned repository, so you can have all the pages when you add your new one. Then build the website and upload the `public` folder.

For the uninitiated:

* The localhost testing command is `hugo serve` (or `hugo server`).
* The build command is `hugo`.
* The official site update command is (replace `rsync -rc` with `scp -r` if you don't have rsync): `rsync -rc public/* istXXXXXX@sigma.ist.utl.pt:/afs/ist.utl.pt/groups/ambientalist/web`.
