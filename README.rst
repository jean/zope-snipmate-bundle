Zope support for Vim's snipMate plugin
======================================

Tired of typing in endless boilerplate code when writing Zope applications?

This bundle will ease the pain in your fingertips and make development in Vim
a more enjoyable and smooth experience... hopefully.

Introduction
------------
What is Zope?
    Zope is a free and open-source object-oriented Python framework.
    See: http://www.zope.org

What is snipMate?
    snipMate is a snippets extension for Vim. It is inspired by
    TextMate's popular 'code snippets' feature.
    See: http://www.vim.org/Scripts/script.php?script_id=2540

What is zope-snipmate-bundle?
    This is a bundle of 'snipMate compatible' snippets generated from
    Tom Lazar and Witsch's excellent Zope snippets for TextMate.
    See: https://github.com/tomster/zope.tmbundle

What is provided by this bundle?
    * snipMate snippets for TAL, ZCML and common Zope and Plone code blocks.
    * A conversion script

Where can I get updated versions of this bundle?
    I mantain the snippets and the conversion script on Github.
    See: http://github.com/zedr/zope-snipmate-bundle

Requirements
------------
* Vim
* snipMate plugin
* Python >=2.6

Installation
------------
* Copy the snippets in your $HOME/.vim/snippets/ directory
* Add the following lines in your $HOME/.vimrc::

    au BufNewFile,BufRead *.pt set filetype=html.pt
    au BufNewFile,BufRead *.zcml set filetype=xml.zcml

Usage
-----
Snippets
    See snipMate's homepage, or this screencast: http://vimeo.com/3535418

Conversion script
    This conversion script will read all TextMate compatible snippets
    in a directory and convert them to snipMate's format.

    Run with::

        ./tm2snip.py <TextMate snips directory> <Target directory>

Maintainer
----------
zedr (Rigel Di Scala) <zedr@zedr.com>

Credits
-------
- Tom Lazar and Witsch for their TextMate snippets
