# Week In Review

Custom theme for [Ghost](http://github.com/tryghost/ghost/), for use on week-in-review.com

### Development

Recommend commands while in development:

    rsync -azP --delete --exclude ".*/" --exclude ".*" --exclude "tmp/" ~/work/wir-theme ghost@week-in-review.com:/var/www/week-in-review.com/content/themes/
    fswatch -o ~/work/wir-theme | while read f; do wirsync_once; done


