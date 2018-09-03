# Carnegie Mellon University Humanist League Test Website

This is the repository for testing content on the Carnegie Mellon University
Humanist League Website. We use jekyll to build the static website using our
[own gem based
theme](https://github.com/cmu-humanists/jekyll-theme-cmu-humanists).

Follow the instructions in the README in
https://github.com/cmu-humanists/cmu-humanists.github.io
to get setup editing the website locally.

Clone this repository in the same directory you have `cmu-humanists.github.io`
cloned.

    $ git clone https://github.com/cmu-humanists/test-site.git

Edit `cmu-humanists.github.io/_config.yml` so that it has

```yaml
url: https://cmuhl.org/test-site
```

Then in the `cmu-humanists.github.io` directory, run

    $ bundle exec jekyll build

Then change directories to the test site

    $ cd ../test-site/
    
And commit then push the changes

    $ git commit -am "update website"
    $ git push
    
Github will automatically start the jekyll build of the website and your changes
should be viewable in a few minutes at https://cmuhl.org/test-site/

Remember to change the `url` in `cmu-humanists.github.io/_config.yml` back to

```yaml
url: https://cmuhl.org
```

before making and pushing any commits in your `cmu-humanists.github.io`
repository, otherwise github will get confused and bad things will happen.

