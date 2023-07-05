# Instructions for admins

To add the [Bird UI theme](https://github.com/ronilaukkarinen/mastodon-bird-ui) to your Glitch-soc instance follow these steps!
(Please note that this only support the "vanilla" flavour as of now)

1. Add the files from the repos "mastodon" folder into the folder of your Glitch-soc Install:

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

2. **Compile the theme assets and restart.** Run `RAILS_ENV=production bundle exec rails assets:precompile` and reload mastodon-web for the changes to take effect.