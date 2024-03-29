ShinobiEssentials Bookshelf Accordion (Objective-C)
=====================

A ShinobiEssentials demo app showing how to use an SEssentialsAccordion to display books on a bookcase. When a book's spine is tapped it opens up to show a UIView representing the book's cover.

![Screenshot](screenshot.png?raw=true)

There's a [blog post](http://www.shinobicontrols.com/blog/posts/2013/11/12/shinobiessentials-an-accordion-off-the-shelf/) to accompany this project.

Building the project
------------------

In order to build this project you'll need a copy of ShinobiEssentials. If you don't have it yet, you can download a free trial from the [ShinobiEssentials website](http://www.shinobicontrols.com/shinobiessentials/price-plans/shinobiessentials/shinobiessentials-trial-form/).

You'll need to add/fix the links to the ShinobiEssentials framework and bundle to the project. Open up the project in Xcode, then open your ShinobiEssentials download in finder, and drag ShinobiEssentials.bundle from finder into Xcode's 'frameworks' group. If you haven't run the ShinobiEssentials installer, you'll also need to do the same for ShinobiEssentials.framework.

If you're using the trial version you'll need to add your license key. To do so, open up **BooksShelfAppDelegate.m**, import `<ShinobiEssentials/SEssentials.h>`, and set the license key inside `application:didFinishLaunchingWithOptions:` as follows:

    #import <ShinobiEssentials/SEssentials.h>

    @implementation BookShelfAppDelegate

    - (BOOL)application:(UIApplication *)application didFinishLaunchingWithOptions:(NSDictionary *)launchOptions
    {
        [ShinobiEssentials setLicenseKey:@"your license key"];
        …
    }

Contributing
------------

We'd love to see your contributions to this project - please go ahead and fork it and send us a pull request when you're done! Or if you have a new project you think we should include here, email info@shinobicontrols.com to tell us about it.

License
-------

The [Apache License, Version 2.0](license.txt) applies to everything in this repository, and will apply to any user contributions.

