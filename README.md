# zam
hugo theme for photo gallery

---

## about this theme

- require hugo 0.58 or later
- use hugo module to mount content into site
- best for photo gallery site/blog
- fixed entry text width, everything else is responsive
- explain predefined settings in config.toml

---

## how to use

step 1: folk this to your local computer

```shell
git clone https://github.com/chuadangky/zam.git
```

step 2: `cd` into downloaded folder and edit settings in `config.toml`

step 3: run `hugo server` in your terminal

---

## content page bundles

use page bundle for your content, see https://gohugo.io/content-management/page-bundles/

content files/folders should look like this

```txt
.
└── gallery # mount this folder into hugo eg. content/content-primary
    |
    ├── _index.md # title, menu...
    |
    ├── gallery-sample-name-01 # post name
    │   ├── 01.jpg
    │   ├── 02.jpg
    │   ├── 03.jpg
    │   ├── 97.jpg
    │   ├── 98.jpg
    │   ├── 99.jpg
    │   ├── cover.jpg # post cover
    │   └── index.md # post content
    |
    └── gallery-sample-name-02 # another post bundle
        └── # content and it's resources
```

---

## primary and secondary mount point

The `content-primary` mount point is for primary content section *(eg. blog)*. Your post should have a `cover.jpg` (or `.png`) within post folder. This image would be your post cover image.

The `content-secondary` mount point is for secondary content section *(eg. collective)*. You don't need `cover.*` image. It uses the first image in folder for post cover.

---

## preview

### home page

![](https://res.cloudinary.com/khongdangky/image/upload/v1571914352/blog/nghichngom/home1_osppov.jpg)

### primary content list style

![](https://res.cloudinary.com/khongdangky/image/upload/v1571914352/blog/nghichngom/page1_vv6qyy.jpg)

---

## near future plan

- ~~content mount point options (config)~~ done
- ~~define cover image size on config file~~ done
- slideshow for gallery photo with some predefine layout

## later

- google analytic, robot.txt, sitemap, etc...
- collapsable section for disqus
- share button (facebook, twitter, pinterest)
- shortcode to insert image
