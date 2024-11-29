# How to maintain this website

## Source 

Jekyll theme based on [landing-page bootstrap theme ](http://startbootstrap.com/templates/landing-page/), V1.0.1. Most documentation will be there.
For more Jekyll details, read [documentation](http://jekyllrb.com/).
The landing page theme used [Freelancer Jekyll theme](https://github.com/jeromelachaud/freelancer-theme/) as reference.

## How to use

Most configuration parameters are stored in [_config.yml](_config.yml), and its use is privileged over hardcoding information. 

The front page is composed of "[posts](_posts)", which are pulled in by [_includes/page_content.html](_includes/page_content.html) in reverse chronological order (as per the fake date in the post name). They alternate between left and right layout. 

No other pages are created or used, though of course Jekyll allows for that.

To add items to the top of the page, add a "post" with a higher date. See the examples among the existing posts.

## Other configuration

The website domain name is configured in [CNAME](CNAME). 

## Building the website

The website is built automatically using Github Actions, see [Settings/Pages](settings/pages), using the "Deploy from Branch" functionality, with a custom domain configured.

## License

The pre-defined contents (layout, css, etc.) of this repository are licensed under the [Apache
2.0](http://www.apache.org/licenses/LICENSE-2.0.html).

The content is licensed under CC-BY-NC.

