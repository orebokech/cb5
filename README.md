## cb5
### mimimalist static site/blog generator

cb5 is a small (200 lines) Python script to generate a static blog. It
is the engine behind [blog.orebokech.com][ia]. Each post is stored as a
UTF-8 encoded Markdown file, from which an HTML page is created. cb5
also generates an Atom feed and an archives page.

[ia]: http://blog.orebokech.com/

Each post's timestamp is taken from the file's mtime. The title is taken
from the first line of the Markdown file, which must be an H1 header.

## Dependencies

cb5 uses the following libraries:

* [python-markdown][python-markdown], `python-markdown` in Debian/Ubuntu
* [PyRSS2Gen][PyRSS2Gen], `python-pyrss2gen` in Debian/Ubuntu
* [Mako Templates][mako], `python-mako` in Debian/Ubuntu

[python-markdown]: http://freewisdom.org/projects/python-markdown/
[PyRSS2Gen]: http://www.dalkescientific.com/Python/PyRSS2Gen.html
[mako]: http://www.makotemplates.org/

## How to use

The repository includes an example site in the `example` directory. Run
`make gen` in this directory to generate the example site. You can then
run `make test` to start a web server on port 8000 to see the site.

The configuration file, `cb5.conf`, should be pretty self-explanatory.

## License

MIT:

    Permission is hereby granted, free of charge, to any person
    obtaining a copy of this software and associated documentation files
    (the "Software"), to deal in the Software without restriction,
    including without limitation the rights to use, copy, modify, merge,
    publish, distribute, sublicense, and/or sell copies of the Software,
    and to permit persons to whom the Software is furnished to do so,
    subject to the following conditions:
    
    The above copyright notice and this permission notice shall be
    included in all copies or substantial portions of the Software.
    
    THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
    EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
    MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
    NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS
    BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN
    ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
    CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
    SOFTWARE.
