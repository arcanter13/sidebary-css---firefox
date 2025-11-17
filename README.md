Enable Firefox features

Go to about:config and set all of the following to true:

    toolkit.legacyUserProfileCustomizations.stylesheets
    layers.acceleration.force-enabled
    gfx.webrender.all
    gfx.webrender.enabled
    layout.css.backdrop-filter.enabled
    svg.context-properties.content.enabled
    
    # LINUX ONLY - WORKAROUND FOR BAR HIDING ON DRAG EVENT
    widget.gtk.ignore-bogus-leave-notify = 1

Write your userChrome.css

    Find your Firefox profile folder (about:support --> "Profile Directory")
    Create a folder named chrome inside it.
    Create a file named userChrome.css inside the chrome folder you just created.
    Paste in userChrome.css whatever you like from above
    Restart Firefox for changes to take effect. If nothing changes, try going to about:profiles and click the "Restart Normally" button in the upper right portion of the screen. Thanks @kr1s7ian for pointing this out.
