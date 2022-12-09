# Aaron's Home Assistant config files

If you're here, it's probably because you're vaguely interested in how I deal with the .yaml files that Home Assistant still uses in Some Places.

I do have a lot; I just put **domains** into [**configuration.yaml**](./configuration.yaml), and then use `!include domain.yaml` in order to split them out.

So for the `media_player` domain, [**configuration.yaml**](./configuration.yaml) has a line: 

```media_player: !include media_player.yaml``` 

This tells Home Assistant to look in [**media_player.yaml**](./media_player.yaml) for the media player config.