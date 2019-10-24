# zam
hugo theme for photo gallery

---

## about this theme

- require hugo 0.58 or later
- use hugo module to mount content into site
- best for photo gallry site/blog
- fixed entry text width
- almost setting predefined in config.toml

---

## how to use

step 1: folk this to your local computer

step 2: edit `config.toml` (below is mine, you should change to your own source)

```toml
# Use hugo module to mount content from local folder
# Change below source to your content path (relate to your hugo folder)
# you can even use your github/gitlab repositories
[module]
[[module.mounts]]
source = "../content/blog"
target = "content/content-primary"
[[module.mounts]]
source = "../content/insp"
target = "content/content-secondary"
```

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

## future plan

- define image size on config file
- slideshow for gallery photo with some predefine layout
- google analytic
- collapsable section for disqus
- share button (facebook, twitter, pinterest)
- shortcode to insert image