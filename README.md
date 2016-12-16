# Installing PyGame on MacOS Sierra

Unfortunately the main website of PyGame only offers packages compatible with Python 2. To get access to PyGame for Python 3, follow the steps below.



1. Install the [Homebrew package manager](http://brew.sh)
2. Run the command ```brew install python3 sdl sdl_image sdl_mixer sdl_ttf smpeg portmidi mercurial git```
3. Run the command ```pip3 install hg+http://bitbucket.org/pygame/pygame```
4. That's it! Have fun!

## Verify installation

```
$ python3
>>> import pygame
>>> pygame.init()
(6, 0)
>>> pygame.display.set_mode((800, 600))
<Surface(800x600x32 SW)>
>>> raise SystemExit
```



## Troubleshooting

If you get errors relating to permissions, try the following command: ```sudo chown -R $(whoami) /usr/local/share```

That should fix the permissions.



Special thanks to [Florian Berger](http://florian-berger.de/en/articles/installing-pygame-for-python-3-on-os-x/) for his excellent article.