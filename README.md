# px2html

The static site generator for pictures based on [pics2html](https://github.com/danieljakots/pics2html).

## Usage

0. Install dependencies: `pip install Pillow==8.3.2 jinja2 feedgenerator`.
1. Put all pictures in output/pictures/. The name must be yyyy-mm-dd-title.jpg.
Failure to abide will surely make the parser unhappy. And you don't want to
make it unhappy. If you can avoid to use SMALL_IMAGE_WORD (as defined in the
python script) in the title, it's probably better. Better as in otherwise it
may not do what you thought. But the good news is you "can" use dashes instead
of spaces in the title! 😬
2. Edit global var at the top of pics2html.py.
3. Run `python3 pics2tohtml.py` and let the magic happen.
4. It will create smaller pictures if they're bigger than the threshold, so it may
take some time the first time.
5. It will output all the html files so you just have to ship the whole dir.
