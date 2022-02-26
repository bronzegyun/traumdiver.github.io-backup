How to create a new Jekyll site based on a set theme(e.g. [just-the-docs](https://github.com/pmarsceill/just-the-docs)).

# Creating new site

1. Open Terminal.
1. To create a new Jekyll site, use the jekyll new command in the folder:
    ```
    $ jekyll new --skip-bundle .
    ```
1. Open the `Gemfile` that Jekyll created.
1. Delete all lines, and set it like below:
    ```
    source "https://rubygems.org"
    gem "github-pages", "~> GITHUB-PAGES-VERSION", group: :jekyll_plugins
    gem "just-the-docs"
    ```
    Replace *GITHUB-PAGES-VERSION* with the latest supported version of the github-pages gem.  
    You can find this version here: "[Dependency versions](https://pages.github.com/versions/)".
1. Save and close the `Gemfile`.

# Building your site locally

1. Open Terminal.
1. Run `bundle install`.
1. To run your Jekyll site locally, run `bundle exec jekyll serve`.
1. To preview your site, in your web browser, navigate to `http://localhost:4000`.

# Updating the GitHub Pages gem

1. Open Terminal.
1. Update the `github-pages` gem.
    - If you installed Bundler, run `bundle update github-pages`.
    - If you don't have Bundler installed, run `gem update github-pages`.