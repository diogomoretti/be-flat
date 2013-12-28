#Be Flat
Convert any color to a flat-color.

##Demo
[Demo Page](http://diogomoretti.github.io/Be-Flat/)

##Usage
**Sass** function:

    @function flat($color)
      @return darken(lighten(desaturate(saturate(lighten(desaturate($color, 25%), 10%), 20%), 30%), 26%), 25%)

**Stylus** mixin:

    flat(c)
      if dark(c)
        darken(saturate(lighten(desaturate(lighten(desaturate(c, 40%), 10%), 20%), 20%), 20%), 20%)
      else
        darken(saturate(lighten(desaturate(lighten(desaturate(c, 30%), 10%), 10%), 30%), 20%), 20%)
## Contributing
 
1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request :D

OR:

1. Just edit this README file.

## History
 
* **2013-10-24:** First version.

## Credits
 
* [Diogo Moretti](http://github.com/diogomoretti)
