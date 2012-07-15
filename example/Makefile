define DEFAULT_POST
# My first post! #

Hello! This is your first post.

You can use [standard Markdown syntax][markdown] to edit your posts.

The Atom feed is named [/index.xml][feed] in the configured output directory,
and the archives are at [/archives.html][archives].

Good luck!

[markdown]: http://daringfireball.net/projects/markdown/
[feed]: /index.xml
[archives]: /archives.html
endef
export DEFAULT_POST

DEFAULT_POST_FILE = data/`date '+%Y/%m'`/first-post.mdwn

gen:
	mkdir -p $(shell dirname $(DEFAULT_POST_FILE))
	echo "$$DEFAULT_POST" >$(DEFAULT_POST_FILE)
	../cb5

test:
	cd htdocs; python -c 'import SimpleHTTPServer; SimpleHTTPServer.test()'

.PHONY: gen test
