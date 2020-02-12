# Website For Cambridge Science Park CoderDojo

This is the GitHub Pages repo for the [Science Park CoderDojo website](https://sciencepark-coderdojo.github.io) 
The files stored in this repo are automatically converted into a set of HTML pages that make up 
the website.

## Organization

The key parts of the site are:
- `_config.yml`: main configuration for the site
- `_pages/`: holding infrequently-changing pages (like the About page)
- `_posts/`: holding periodically updating events and articles

## Resources

The metadata and naming conventions in this repo follow those required by the jekyll site generator.
Refer to the jekyll documentation to learn how to create new [posts](https://jekyllrb.com/docs/posts/)
and [pages](https://jekyllrb.com/docs/pages/).

The site currently uses the [Minimal Mistakes](https://mmistakes.github.io/minimal-mistakes/) 
jekyll theme. The theme offers a number of configuration and layout options, which are described in the 
[theme documentation](https://mmistakes.github.io/minimal-mistakes/docs/configuration/)

## Get added as a collaborator

If you are a Science Park CoderDojo champion or mentor, you can become a collaborator.
As a collaborator, you gain access to the content and tools in this repository. Contact Nicholas Chen to be added.

## Making Changes To the Site

### If you are a collaborator

The simplest way to make quick edits on any content is to use GitHub's web interface to create new files
or by selecting an existing file and clicking the Edit button. 

Note: any changes you make to the 'master' branch of the repository will show up immediately. To see
a preview of your changes as a webpage you have the following options:

- Clone a copy of the repo to your local PC and [test with a local preview](https://help.github.com/en/github/working-with-github-pages/testing-your-github-pages-site-locally-with-jekyll).

- Fork a copy into your own GitHub account. Create a branch called 'gh-pages' and visit your version of the website
  at https://<username>.github.io/<name-of-your-forked-repo>. You can submit pull-requests (see below) to bring any
  changes you make back to the actual site.

### If you are not a collaborator

You can fork this site to your own GitHub account and make and preview edits there. Submit a pull request to
get your changes re-incorporated into the official page.

## Tips and Tricks

### Image Galleries

To create an image gallery, use the [gallery helper included with the theme](https://mmistakes.github.io/minimal-mistakes/docs/helpers/#gallery). In the YAML metadata in the front matter of the page/post that needs a photo gallery,
add the images that you wish to include in the gallery. By default, only `image_path` is required, but the `url`
property can be used to point to an enlarged version of the photo.

As a convention, full-size photos should be put in the `/assets/images/gallery` directory and thumbnails in the `/assets/images/gallery/thumbs` directory.

[ImageMagick](https://imagemagick.org/index.php) can be used to quickly create thumbnails. 
To resize and crop to a square, the following command can be used:

```
convert filename.jpg -thumbnail '300x300^' -gravity center -extent 300x300 filename-th.jpg
```
