# Instructions for admins

To add the [Bird UI theme](https://github.com/ronilaukkarinen/mastodon-bird-ui) to your Glitch-soc instance follow these steps!
(Please note that this only support the "vanilla" flavour as of now)

1. Clone the git repository using `git clone --recurse-submodules https://github.com/jplexer/Bird-UI-Theme-Admins-glitch.git`

2. Add the files from the repos "mastodon" folder into the folder of your Glitch-soc Install:

```
app/
  javascript/
    skins/
      vanilla/
        elephant/                             | **new**
          common.scss                         | **new**
          names.yml                           | **new**
        elephant-contrast/                    | **new**
          common.scss                         | **new**
          names.yml                           | **new**
        elephant-light/                       | **new**
          common.scss                         | **new**
          names.yml                           | **new**
    styles/
    elephant.scss                             | **new**
    elephant-contrast.scss                    | **new**
    elephant-light.scss                       | **new**
      contrast/
        ...
      fonts/
        ...
      elephant/                               | **new**
        contrast.scss                         | **new**
        layout-multiple-columns.scss          | **new**
        layout-single-column.scss             | **new**
        light.scss                            | **new**
```

3. **Compile the theme assets and restart.** Run `RAILS_ENV=production bundle exec rails assets:precompile` and reload mastodon-web for the changes to take effect.


If you want to update the Theme run `git pull --recurse-submodules` in the folder and follow steps 2 and 3 again